import com.efluid.jenkinsfile.Jenkinsfile

// variables globales
scriptParams = [:]
scriptParams['scriptPath'] = 'groovy/workflow/application/build/Jenkinsfile.groovy'
activeNode = false
scriptParams['application'] = 'gerritCli'
scriptParams['applicationVersion'] = '1.0.0-SNAPSHOT'
scriptParams['nodeLabel'] = params['nodeLabel'] != null ? params['nodeLabel'] : env.nodeLabel
scriptParams['nodeLabel'] = scriptParams['nodeLabel'] != null ? scriptParams['nodeLabel'] : 'socle-jenkins-maven-graalvm-docker-14-2G'
scriptParams['destinatairesMail'] = params['destinatairesMail'] != null ? params['destinatairesMail'] : env.destinatairesMail
scriptParams['destinatairesMail'] = scriptParams['destinatairesMail'] != null ? scriptParams['destinatairesMail'] : 'usinelogicielle@efluid.fr'
scriptParams['skipAllocationNodeInJenkinsfile'] = params['skipAllocationNodeInJenkinsfile'] != null ? params['skipAllocationNodeInJenkinsfile'] : env.skipAllocationNodeInJenkinsfile
scriptParams['forceJobExec'] = false

new Jenkinsfile(this, scriptParams).runJenkinsfile()

return this;
