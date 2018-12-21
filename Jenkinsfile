pipeline 
{
  agent any
   stages 
  {      
  stage ('OWASP analyze')
            {
              steps
              {
              pipeline 
{
  agent any
   stages 
  {      
  stage ('OWASP analyze')
            {
              steps
              {
              dependencyCheckAnalyzer datadir: '', hintsFile: '', includeCsvReports: true, includeHtmlReports: true, includeJsonReports: true, includeVulnReports: true, isAutoupdateDisabled: false, outdir: '', scanpath: '', skipOnScmChange: false, skipOnUpstreamChange: false, suppressionFile: '', zipExtensions: ''

           
              }
            }
    stage ('OWASP result check')
    {
         steps
         {
         dependencyCheckPublisher canComputeNew: false, defaultEncoding: '', failedTotalHigh: '1', healthy: '', pattern: '', thresholdLimit: 'high', unHealthy: '', unstableTotalHigh: '1'
         }
       }
   
       }
}

           
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
