# angular2-esperimenti
pianificazione degli esperimenti da fare

- obiettivo: creare un blog usando github come repository dei post

- utilizzeremo un repository per ogni post, gli allegati serviranno come allegati del post:
 https://api.github.com/users/flwblog/repos 
 
 per ogni blog devo leggere:
    "name": "angularconnect-la-mia-prima-conferenza-angularjs",
    "description": "flwblog/angularconnect-la-mia-prima-conferenza-angularjs",
    
  - una volta entrato sul singolo post, devo utilizzare il file readme ed elencare gli allegati:
  https://api.github.com/repos/flwblog/angularconnect-la-mia-prima-conferenza-angularjs/readme
  - decodificare il content in base 64:
  - devo trasformare il file MD in html
  - mostrare il contenuto
  - devo scaricare gli allegati che non iniziano per:
 -  https://api.github.com/repos/flwblog/angularconnect-la-mia-prima-conferenza-angularjs/contents
  - name 
  - download_url



-- cominciamo da alcuni pezzi chiave:
- lista dei repository
- 

     http:Http;
     this.http
     .get('https://api.github.com/repos/flwblog/blog/contents')
     .map(
         res=> res.json()
         )
      .subscribe(
         res => this.posts = res
      );


http://solutionoptimist.com/2013/12/28/awesome-github-tricks/
