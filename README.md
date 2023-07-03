👋 Hi there

I'm Enzzo, a 20-year-old student of Software Engineering with 2 semesters of experience, including internships and several projects. I have a strong interest in software engineering, utilizing algorithms, web systems, and services. My goal is to continuously learn and grow professionally, following best practices to build high-quality web applications.
Throughout my projects and courses, I have acquired extensive knowledge in database management and the software development process. This enables me to participate in the entire project lifecycle, from conception to the delivery of the final product. Additionally, I excel in teamwork, problem-solving, and effective communication with all team members, ensuring quality work within established deadlines.
As a future software engineer, I am always seeking new challenges and opportunities to advance in my career. I am excited to contribute to projects involving web application and service development, utilizing technologies such as Java, JavaScript, Git, GitHub, Node.js, HTML, CSS, Bootstrap, MySQL, and APIs.
As a future software engineer, I am always seeking new challenges and opportunities to advance in my career. I am excited to collaborate on projects involving software development.

📊 GitHub Stats:

💻 Techs:

🌐 Socials:
LinkedIn

document.addEventListener("DOMContentLoaded", function() {
    var url = encodeURIComponent(window.location.href); //url
    var titulo = encodeURIComponent(document.title); //título
    var linkedinLink = "https://www.linkedin.com/shareArticle?mini=true&url="+url+"&title="+titulo;
     
    //tenta obter o conteúdo da meta tag description
    var summary = document.querySelector("meta[name='description']");
    summary = (!!summary)? summary.getAttribute("content") : null;
     
    //se a meta tag description estiver ausente...
    if(!summary){
        //...tenta obter o conteúdo da meta tag og:description
        summary = document.querySelector("meta[property='og:description']");
        summary = (!!summary)? summary.getAttribute("content") : null;
    }
    //altera o link do botão
    linkedinLink = (!!summary)? linkedinLink + "&summary=" + encodeURIComponent(summary) : linkedinLink;
    document.getElementById("linkedin-share-btt").href = linkedinLink;
}, false);
