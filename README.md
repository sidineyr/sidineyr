<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meu Portfólio</title>
    <link rel="stylesheet" href="styles.css">
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
</head>
<body>
    <header>
        <h1>Bem-vindo ao meu Portfólio!</h1>
        <p>Desenvolvedor apaixonado por tecnologia e inovação</p>
    </header>

    <main>
        <section id="about-me">
            <h2>Sobre Mim</h2>
            <p>Sou um desenvolvedor com experiência em diversas linguagens de programação e ferramentas. Aqui você encontrará informações sobre meus projetos, habilidades e desempenho.</p>
        </section>

        <section id="performance-metrics">
            <h2>Métricas de Desempenho</h2>
            <canvas id="performanceChart" width="400" height="200"></canvas>
        </section>

        <section id="programming-languages">
            <h2>Linguagens de Programação</h2>
            <div class="icons">
                <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" alt="JavaScript" title="JavaScript">
                <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" alt="Python" title="Python">
                <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg" alt="Java" title="Java">
                <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" alt="HTML5" title="HTML5">
                <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" alt="CSS3" title="CSS3">
            </div>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 Desenvolvido por Sidineyr</p>
    </footer>

    <script>
        const ctx = document.getElementById('performanceChart').getContext('2d');
        const performanceChart = new Chart(ctx, {
            type: 'bar',
            data: {
                labels: ['JavaScript', 'Python', 'Java', 'HTML5', 'CSS3'],
                datasets: [{
                    label: 'Nível de Proficiência (%)',
                    data: [90, 85, 80, 95, 90],
                    backgroundColor: [
                        'rgba(255, 99, 132, 0.2)',
                        'rgba(54, 162, 235, 0.2)',
                        'rgba(255, 206, 86, 0.2)',
                        'rgba(75, 192, 192, 0.2)',
                        'rgba(153, 102, 255, 0.2)'
                    ],
                    borderColor: [
                        'rgba(255, 99, 132, 1)',
                        'rgba(54, 162, 235, 1)',
                        'rgba(255, 206, 86, 1)',
                        'rgba(75, 192, 192, 1)',
                        'rgba(153, 102, 255, 1)'
                    ],
                    borderWidth: 1
                }]
            },
            options: {
                scales: {
                    y: {
                        beginAtZero: true
                    }
                }
            }
        });
    </script>
</body>
</html>
