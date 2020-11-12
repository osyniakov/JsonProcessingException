Sample project to reproduce https://github.com/jeremylong/DependencyCheck/issues/2947
 
 
     [osyniakov@osyniakov-linux JsonProcessingException (master)]$ ./mvnw clean site:site
     [INFO] Scanning for projects...
     [INFO] 
     [INFO] -----------------< de.oleksii:JsonProcessingException >-----------------
     [INFO] Building JsonProcessingException 1.0-SNAPSHOT
     [INFO] --------------------------------[ jar ]---------------------------------
     [INFO] 
     [INFO] --- maven-clean-plugin:2.5:clean (default-clean) @ JsonProcessingException ---
     [INFO] Deleting /home/osyniakov/projects/JsonProcessingException/target
     [INFO] 
     [INFO] --- maven-site-plugin:3.9.1:site (default-cli) @ JsonProcessingException ---
     [WARNING] Input file encoding has not been set, using platform encoding UTF-8, i.e. build is platform dependent!
     [INFO] configuring report plugin org.owasp:dependency-check-maven:6.0.3
     [INFO] 1 report configured for dependency-check-maven:6.0.3: aggregate
     [WARNING] Report plugin org.apache.maven.plugins:maven-project-info-reports-plugin has an empty version.
     [WARNING] 
     [WARNING] It is highly recommended to fix these problems because they threaten the stability of your build.
     [WARNING] 
     [WARNING] For this reason, future Maven versions might no longer support building such malformed projects.
     [INFO] configuring report plugin org.apache.maven.plugins:maven-project-info-reports-plugin:3.1.1
     [INFO] 15 reports detected for maven-project-info-reports-plugin:3.1.1: ci-management, dependencies, dependency-info, dependency-management, distribution-management, index, issue-management, licenses, mailing-lists, modules, plugin-management, plugins, scm, summary, team
     [INFO] Rendering site with default locale English (en)
     [WARNING] No project URL defined - decoration links will not be relativized!
     [INFO] Rendering content with org.apache.maven.skins:maven-default-skin:jar:1.3 skin.
     [INFO] Generating "dependency-check:aggregate" report --- dependency-check-maven:6.0.3:aggregate
     [INFO] ------------------------------------------------------------------------
     [INFO] BUILD FAILURE
     [INFO] ------------------------------------------------------------------------
     [INFO] Total time:  2.295 s
     [INFO] Finished at: 2020-11-12T09:45:19+01:00
     [INFO] ------------------------------------------------------------------------
     [ERROR] Failed to execute goal org.apache.maven.plugins:maven-site-plugin:3.9.1:site (default-cli) on project JsonProcessingException: Error generating dependency-check-maven:6.0.3:aggregate report: NullPointerException -> [Help 1]
     [ERROR] 
     [ERROR] To see the full stack trace of the errors, re-run Maven with the -e switch.
     [ERROR] Re-run Maven using the -X switch to enable full debug logging.
     [ERROR] 
     [ERROR] For more information about the errors and possible solutions, please read the following articles:
     [ERROR] [Help 1] http://cwiki.apache.org/confluence/display/MAVEN/MojoExecutionException
