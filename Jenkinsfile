pipeline 
{
  agent any
   stages 
  {      
    stage ('OWASP analyze')
     {     
        steps
         {
          dependencyCheckAnalyzer datadir: '', hintsFile: '', includeCsvReports: false, includeHtmlReports: false, includeJsonReports: false, includeVulnReports: false, isAutoupdateDisabled: false, outdir: '', scanpath: '', skipOnScmChange: false, skipOnUpstreamChange: false, suppressionFile: '', zipExtensions: ''

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
  post { always{ emailext attachmentsPattern: 'dependency-check-report.csv', body: '', subject: 'owasp', to: 'narambhatla.mahathi@chubb.com'
               }}
}

           
    
    
