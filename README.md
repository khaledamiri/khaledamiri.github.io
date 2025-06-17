<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Khaled AMIRI - Senior FullStack Java Developer</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        .header {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 2rem;
            margin-bottom: 2rem;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .header::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: linear-gradient(90deg, #667eea, #764ba2, #f093fb, #f5576c);
            background-size: 200% 100%;
            animation: gradient 3s ease infinite;
        }

        @keyframes gradient {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .profile-name {
            font-size: 3rem;
            font-weight: 700;
            background: linear-gradient(135deg, #667eea, #764ba2);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-bottom: 0.5rem;
        }

        .profile-title {
            font-size: 1.5rem;
            color: #666;
            margin-bottom: 1rem;
        }

        .profile-summary {
            font-size: 1.1rem;
            color: #555;
            max-width: 800px;
            margin: 0 auto 2rem;
        }

        .contact-info {
            display: flex;
            justify-content: center;
            gap: 2rem;
            flex-wrap: wrap;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 0.5rem;
            padding: 0.5rem 1rem;
            background: rgba(102, 126, 234, 0.1);
            border-radius: 25px;
            transition: all 0.3s ease;
        }

        .contact-item:hover {
            background: rgba(102, 126, 234, 0.2);
            transform: translateY(-2px);
        }

        .section {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 2rem;
            margin-bottom: 2rem;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
        }

        .section:hover {
            transform: translateY(-5px);
        }

        .section-title {
            font-size: 2rem;
            font-weight: 600;
            margin-bottom: 1.5rem;
            color: #333;
            position: relative;
            padding-bottom: 0.5rem;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 50px;
            height: 3px;
            background: linear-gradient(90deg, #667eea, #764ba2);
            border-radius: 2px;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
        }

        .skill-category {
            background: rgba(102, 126, 234, 0.05);
            border-radius: 15px;
            padding: 1.5rem;
            border-left: 4px solid #667eea;
        }

        .skill-category h3 {
            color: #667eea;
            margin-bottom: 1rem;
            font-size: 1.2rem;
        }

        .skill-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
        }

        .skill-tag {
            background: linear-gradient(135deg, #667eea, #764ba2);
            color: white;
            padding: 0.3rem 0.8rem;
            border-radius: 20px;
            font-size: 0.9rem;
            transition: all 0.3s ease;
        }

        .skill-tag:hover {
            transform: scale(1.05);
            box-shadow: 0 5px 15px rgba(102, 126, 234, 0.3);
        }

        .experience-item {
            border-left: 4px solid #667eea;
            padding-left: 2rem;
            margin-bottom: 2rem;
            position: relative;
        }

        .experience-item::before {
            content: '';
            position: absolute;
            left: -8px;
            top: 0;
            width: 12px;
            height: 12px;
            background: #667eea;
            border-radius: 50%;
        }

        .experience-header {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            margin-bottom: 1rem;
            flex-wrap: wrap;
            gap: 1rem;
        }

        .experience-title {
            color: #333;
            font-size: 1.3rem;
            font-weight: 600;
        }

        .experience-company {
            color: #667eea;
            font-weight: 500;
        }

        .experience-date {
            background: rgba(102, 126, 234, 0.1);
            padding: 0.3rem 1rem;
            border-radius: 20px;
            font-size: 0.9rem;
            color: #667eea;
        }

        .experience-details {
            margin-bottom: 1rem;
        }

        .project-info {
            background: rgba(102, 126, 234, 0.05);
            padding: 1rem;
            border-radius: 10px;
            margin-bottom: 1rem;
        }

        .tech-stack {
            display: flex;
            flex-wrap: wrap;
            gap: 0.3rem;
            margin-top: 0.5rem;
        }

        .tech-item {
            background: rgba(102, 126, 234, 0.1);
            color: #667eea;
            padding: 0.2rem 0.6rem;
            border-radius: 15px;
            font-size: 0.8rem;
        }

        .achievements {
            margin-top: 1rem;
        }

        .achievement-item {
            padding: 0.5rem 0;
            border-bottom: 1px solid rgba(102, 126, 234, 0.1);
        }

        .achievement-item:last-child {
            border-bottom: none;
        }

        .education-item {
            background: rgba(102, 126, 234, 0.05);
            padding: 1.5rem;
            border-radius: 15px;
            margin-bottom: 1rem;
            border-left: 4px solid #667eea;
        }

        .certifications {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1rem;
        }

        .cert-item {
            background: linear-gradient(135deg, #667eea, #764ba2);
            color: white;
            padding: 1.5rem;
            border-radius: 15px;
            text-align: center;
            transition: all 0.3s ease;
        }

        .cert-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(102, 126, 234, 0.3);
        }

        .languages {
            display: flex;
            gap: 2rem;
            justify-content: center;
        }

        .language-item {
            text-align: center;
            padding: 1rem;
            background: rgba(102, 126, 234, 0.05);
            border-radius: 15px;
            min-width: 150px;
        }

        .language-name {
            font-weight: 600;
            color: #667eea;
            margin-bottom: 0.5rem;
        }

        @media (max-width: 768px) {
            .container {
                padding: 10px;
            }
            
            .profile-name {
                font-size: 2rem;
            }
            
            .contact-info {
                flex-direction: column;
                align-items: center;
            }
            
            .experience-header {
                flex-direction: column;
                align-items: flex-start;
            }
            
            .languages {
                flex-direction: column;
                align-items: center;
            }
        }

        .fade-in {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.6s ease;
        }

        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header Section -->
        <header class="header fade-in">
            <h1 class="profile-name">Khaled AMIRI</h1>
            <p class="profile-title">Senior FullStack Java Developer</p>
            <p class="profile-summary">
                Experienced Java developer with 8+ years of expertise in Spring, databases (RDBMS & NoSQL), 
                and modern web technologies. Passionate about software development with strong analytical, 
                design, and problem-solving capabilities in Java environments.
            </p>
            <div class="contact-info">
                <div class="contact-item">
                    <span>📧</span>
                    <span>kkhaledamiri@gmail.com</span>
                </div>
                <div class="contact-item">
                    <span>📱</span>
                    <span>+32 496 24 04 41</span>
                </div>
                <div class="contact-item">
                    <span>📍</span>
                    <span>Belgium</span>
                </div>
                <div class="contact-item">
                    <span>💼</span>
                    <span>8+ Years Experience</span>
                </div>
            </div>
        </header>

        <!-- Technical Skills Section -->
        <section class="section fade-in">
            <h2 class="section-title">Technical Skills</h2>
            <div class="skills-grid">
                <div class="skill-category">
                    <h3>Programming Languages</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">Java 21</span>
                        <span class="skill-tag">Java EE</span>
                        <span class="skill-tag">JavaScript</span>
                        <span class="skill-tag">TypeScript</span>
                        <span class="skill-tag">SQL</span>
                        <span class="skill-tag">JSP</span>
                    </div>
                </div>
                <div class="skill-category">
                    <h3>Frameworks</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">Spring MVC</span>
                        <span class="skill-tag">Spring Security</span>
                        <span class="skill-tag">Spring Cloud</span>
                        <span class="skill-tag">Angular</span>
                        <span class="skill-tag">AxonFramework</span>
                        <span class="skill-tag">Vert.x</span>
                    </div>
                </div>
                <div class="skill-category">
                    <h3>Databases</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">PostgreSQL</span>
                        <span class="skill-tag">MySQL</span>
                        <span class="skill-tag">MongoDB</span>
                        <span class="skill-tag">OrientDB</span>
                        <span class="skill-tag">MariaDB</span>
                        <span class="skill-tag">MinIO</span>
                    </div>
                </div>
                <div class="skill-category">
                    <h3>DevOps & Tools</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">Docker</span>
                        <span class="skill-tag">Kubernetes</span>
                        <span class="skill-tag">Jenkins</span>
                        <span class="skill-tag">GitLab CI</span>
                        <span class="skill-tag">Maven</span>
                        <span class="skill-tag">SonarQube</span>
                    </div>
                </div>
                <div class="skill-category">
                    <h3>Message Queue & Security</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">Apache Kafka</span>
                        <span class="skill-tag">ActiveMQ</span>
                        <span class="skill-tag">TPM</span>
                        <span class="skill-tag">PKI</span>
                        <span class="skill-tag">HSM</span>
                        <span class="skill-tag">Keycloak</span>
                    </div>
                </div>
                <div class="skill-category">
                    <h3>Testing & Methodologies</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">JUnit</span>
                        <span class="skill-tag">Mockito</span>
                        <span class="skill-tag">Scrum</span>
                        <span class="skill-tag">Kanban</span>
                        <span class="skill-tag">TDD</span>
                    </div>
                </div>
            </div>
        </section>

        <!-- Experience Section -->
        <section class="section fade-in">
            <h2 class="section-title">Professional Experience</h2>
            
            <div class="experience-item">
                <div class="experience-header">
                    <div>
                        <h3 class="experience-title">Senior Java EE Developer</h3>
                        <p class="experience-company">Cryptolog Consulting/ETNIC</p>
                    </div>
                    <span class="experience-date">Aug 2024 - Present</span>
                </div>
                <div class="project-info">
                    <strong>Project:</strong> SIPAR 2 - Justice Houses Management System<br>
                    <strong>Client:</strong> Maisons de justice en Fédération Wallonie-Bruxelles<br>
                    <strong>Team Size:</strong> 10 members
                    <div class="tech-stack">
                        <span class="tech-item">Java 8</span>
                        <span class="tech-item">JSF</span>
                        <span class="tech-item">PrimeFaces</span>
                        <span class="tech-item">Hibernate</span>
                        <span class="tech-item">DB2</span>
                        <span class="tech-item">JBoss</span>
                        <span class="tech-item">GitLab CI</span>
                    </div>
                </div>
                <div class="achievements">
                    <div class="achievement-item">✓ Developed new features for case and service management using JSF and PrimeFaces</div>
                    <div class="achievement-item">✓ Implemented automated batch processing for recurring tasks</div>
                    <div class="achievement-item">✓ Created automated SMS notification system for case updates</div>
                    <div class="achievement-item">✓ Optimized application performance with caching mechanisms and SQL query optimization</div>
                    <div class="achievement-item">✓ Maintained high code quality using SonarQube and clean code practices</div>
                </div>
            </div>

            <div class="experience-item">
                <div class="experience-header">
                    <div>
                        <h3 class="experience-title">Senior Java Spring Angular Developer</h3>
                        <p class="experience-company">SoftParadigm / Thales GROUP</p>
                    </div>
                    <span class="experience-date">May 2023 - Apr 2024</span>
                </div>
                <div class="project-info">
                    <strong>Project:</strong> MOSIP (Modular Open-Source Identity Platform)<br>
                    <strong>Client:</strong> Government Projects<br>
                    <strong>Team Size:</strong> 6 members
                    <div class="tech-stack">
                        <span class="tech-item">Java 17</span>
                        <span class="tech-item">Spring Boot</span>
                        <span class="tech-item">Spring Security</span>
                        <span class="tech-item">Angular</span>
                        <span class="tech-item">Keycloak</span>
                        <span class="tech-item">PostgreSQL</span>
                        <span class="tech-item">ELK Stack</span>
                        <span class="tech-item">Docker</span>
                        <span class="tech-item">Kubernetes</span>
                    </div>
                </div>
                <div class="achievements">
                    <div class="achievement-item">✓ Developed REST endpoints for advanced identity management features</div>
                    <div class="achievement-item">✓ Implemented data encryption at rest for enhanced security</div>
                    <div class="achievement-item">✓ Customized registration flow with new fields and user experience improvements</div>
                    <div class="achievement-item">✓ Mentored team members and conducted code reviews</div>
                    <div class="achievement-item">✓ Applied TDD methodology with comprehensive unit and integration testing</div>
                </div>
            </div>

            <div class="experience-item">
                <div class="experience-header">
                    <div>
                        <h3 class="experience-title">Senior Java Spring Angular Developer</h3>
                        <p class="experience-company">SoftParadigm</p>
                    </div>
                    <span class="experience-date">Mar 2022 - Apr 2023</span>
                </div>
                <div class="project-info">
                    <strong>Project:</strong> Heero - E-commerce Management Solution<br>
                    <strong>Client:</strong> E-commerce sites<br>
                    <strong>Team Size:</strong> 6 members
                    <div class="tech-stack">
                        <span class="tech-item">Java 8</span>
                        <span class="tech-item">Spring Boot</span>
                        <span class="tech-item">Spring Cloud Gateway</span>
                        <span class="tech-item">Angular</span>
                        <span class="tech-item">PostgreSQL</span>
                        <span class="tech-item">Apache Kafka</span>
                        <span class="tech-item">Docker</span>
                    </div>
                </div>
                <div class="achievements">
                    <div class="achievement-item">✓ Developed REST APIs to enhance application functionality</div>
                    <div class="achievement-item">✓ Improved code quality applying SOLID principles and Design Patterns</div>
                    <div class="achievement-item">✓ Created proof of concepts for new technologies and features</div>
                    <div class="achievement-item">✓ Mentored junior developers and participated in Agile Scrum planning</div>
                </div>
            </div>
        </section>

        <!-- Education Section -->
        <section class="section fade-in">
            <h2 class="section-title">Education</h2>
            <div class="education-item">
                <h3>Engineering Degree in Information Systems and Software</h3>
                <p><strong>TIME</strong> - June 2015</p>
            </div>
            <div class="education-item">
                <h3>University Degree in Information Systems and Software</h3>
                <p><strong>ISI Tunisia</strong> - June 2011</p>
            </div>
        </section>

        <!-- Certifications Section -->
        <section class="section fade-in">
            <h2 class="section-title">Certifications</h2>
            <div class="certifications">
                <div class="cert-item">
                    <h3>Oracle Certified Professional (OCP)</h3>
                    <p>Java SE 6 Programmer</p>
                </div>
                <div class="cert-item">
                    <h3>Kubernetes Application Development</h3>
                    <p>In Progress</p>
                </div>
            </div>
        </section>

        <!-- Languages Section -->
        <section class="section fade-in">
            <h2 class="section-title">Languages</h2>
            <div class="languages">
                <div class="language-item">
                    <div class="language-name">English</div>
                    <div>Fluent</div>
                </div>
                <div class="language-item">
                    <div class="language-name">French</div>
                    <div>Fluent</div>
                </div>
            </div>
        </section>
    </div>

    <script>
        // Smooth scrolling animation
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, observerOptions);

        // Observe all fade-in elements
        document.querySelectorAll('.fade-in').forEach(el => {
            observer.observe(el);
        });

        // Add some interactive effects
        document.querySelectorAll('.skill-tag').forEach(tag => {
            tag.addEventListener('click', () => {
                tag.style.animation = 'none';
                tag.offsetHeight; // Trigger reflow
                tag.style.animation = 'pulse 0.6s ease';
            });
        });

        // Add CSS for pulse animation
        const style = document.createElement('style');
        style.textContent = `
            @keyframes pulse {
                0% { transform: scale(1); }
                50% { transform: scale(1.1); }
                100% { transform: scale(1); }
            }
        `;
        document.head.appendChild(style);
    </script>
</body>
</html>
