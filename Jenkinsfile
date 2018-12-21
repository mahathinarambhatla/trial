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
       
  }
  post { always{ emailext attachmentsPattern: 'dependency-check-report.xml', body: '', subject: 'owasp', to: 'narambhatla.mahathi@chubb.com'
               }}
}

           
    
    
