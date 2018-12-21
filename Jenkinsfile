pipeline 
{
  agent any
   stages 
  {      
  stage ('OWASP analyze')
            {
              steps
              {
              dependencyCheckAnalyzer datadir: '', hintsFile: '', includeCsvReports: true, includeHtmlReports: true, includeJsonReports: true, includeVulnReports: true, isAutoupdateDisabled: true, outdir: '', scanpath: ' ${WORKSPACE}', skipOnScmChange: false, skipOnUpstreamChange: false, suppressionFile: '', zipExtensions: ''
           
              }
            }
    stage ('OWASP Publish')
    {
         steps
         {
         dependencyCheckPublisher canComputeNew: false, defaultEncoding: '', failedTotalHigh: '1', healthy: '', pattern: '', thresholdLimit: 'high', unHealthy: '', unstableTotalHigh: '1'
         }
       }
       }
}
