<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>David Vicente Calzada | Operations Portfolio</title>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <style>
        :root {
            --primary: #0d1b2a;
            --secondary: #1b263b;
            --accent: #415a77;
            --highlight: #00b4d8;
            --text: #e0e1dd;
            --white: #ffffff;
            --success: #2ecc71;
            --warning: #f1c40f;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }
        html { scroll-behavior: smooth; }
        
        body {
            font-family: 'Segoe UI', sans-serif;
            background-color: var(--primary);
            color: var(--text);
            line-height: 1.4;
        }

        /* ─── NAV (COMPACTO CON ICONO) ─── */
        nav {
            position: fixed; top: 0; width: 100%; z-index: 1000;
            background: rgba(13, 27, 42, 0.98); padding: 10px 8%;
            display: flex; justify-content: space-between; align-items: center;
            border-bottom: 2px solid var(--highlight);
        }
        .brand { display: flex; align-items: center; gap: 10px; }
        .brand-icon {
            width: 32px; height: 32px; background: var(--highlight);
            color: var(--primary); display: flex; align-items: center;
            justify-content: center; border-radius: 6px; font-weight: 900;
        }
        .nav-btns { display: flex; gap: 15px; }
        .nav-link {
            color: var(--text); text-decoration: none; font-size: 0.75rem;
            font-weight: bold; text-transform: uppercase;
        }

        /* ─── SECCIONES ─── */
        .section { padding: 40px 10% 20px; }
        #home { padding-top: 80px; text-align: center; }
        
        .badge { 
            background: var(--highlight); color: var(--primary); 
            padding: 4px 12px; border-radius: 20px; font-weight: bold; 
            font-size: 0.8rem; display: inline-block; margin-bottom: 10px;
        }
        h1 { font-size: 2.8rem; color: var(--white); margin-bottom: 5px; }
        .hero-p { max-width: 600px; margin: 0 auto 15px; font-size: 1rem; color: var(--text); }

        /* ─── CONTACTO ─── */
        .contact-row { display: flex; justify-content: center; gap: 10px; margin-bottom: 20px; }
        .btn-c {
            padding: 8px 16px; background: var(--white); color: var(--primary);
            text-decoration: none; border-radius: 5px; font-weight: bold; font-size: 0.85rem;
        }

        /* ─── GRID DE IMPACTO ─── */
        .grid-3 { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; }
        .achieve-card {
            background: var(--secondary); padding: 20px; border-radius: 10px;
            border: 1px solid var(--accent); position: relative;
        }
        .achieve-card h3 { color: var(--highlight); font-size: 1.8rem; }
        .achieve-card p { font-weight: bold; font-size: 0.85rem; text-transform: uppercase; }

        /* ─── EXPERIENCIA CON ICONOS ─── */
        .exp-box {
            background: rgba(255,255,255,0.03); padding: 20px; 
            border-radius: 15px; margin-bottom: 15px; border-left: 4px solid var(--highlight);
        }
        .exp-header { display: flex; justify-content: space-between; margin-bottom: 10px; }
        .bullet-item { display: flex; gap: 12px; margin-bottom: 8px; align-items: flex-start; }
        .icon-circle { 
            min-width: 32px; height: 32px; background: var(--secondary); 
            border-radius: 50%; display: flex; align-items: center; justify-content: center;
            border: 1px solid var(--highlight); font-size: 1rem;
        }
        .tag { font-size: 0.65rem; padding: 2px 6px; border-radius: 3px; font-weight: bold; margin-left: 8px; }
        .tag-ok { border: 1px solid var(--success); color: var(--success); }
        .tag-warn { border: 1px solid var(--warning); color: var(--warning); }

        /* ─── SKILLS & EDUCATION ─── */
        .pill-container { display: flex; flex-wrap: wrap; gap: 8px; margin-top: 10px; }
        .pill { background: var(--accent); color: var(--white); padding: 4px 10px; border-radius: 5px; font-size: 0.75rem; }

        .chart-wrap { background: var(--secondary); padding: 15px; border-radius: 10px; margin-top: 15px; }

        @media (max-width: 768px) { .nav-btns { display: none; } h1 { font-size: 2rem; } }
    </style>
</head>
<body>

    <nav>
        <div class="brand">
            <div class="brand-icon">V</div>
            <div style="color: var(--white); font-weight: bold;">D. Vicente Calzada</div>
        </div>
        <div class="nav-btns">
            <a href="#home" class="nav-link">Home</a>
            <a href="#experience" class="nav-link">Experience</a>
            <a href="#skills" class="nav-link">Skills</a>
        </div>
    </nav>

    <section id="home" class="section">
        <div class="badge">Supply Chain & Operations Manager</div>
        <h1>David Vicente Calzada</h1>
        <p class="hero-p">Operations leader with 3+ years of experience in high-stakes logistics, mission-critical delivery, and crisis response.</p>
        <div class="contact-row">
            <a href="mailto:davidvicente010297@gmail.com" class="btn-c">✉️ Email</a>
            <a href="https://linkedin.com/in/david-v-c32215097" target="_blank" class="btn-c">🔗 LinkedIn</a>
            <a href="tel:+525634026833" class="btn-c">📞 Call</a>
        </div>
    </section>

    <section id="highlights" class="section">
        <h2 style="font-size: 1.5rem; margin-bottom: 15px;">Impact Milestones</h2>
        <div class="grid-3">
            <div class="achieve-card">
                <h3>37.5%</h3>
                <p>Efficiency Gain</p>
                <small>Reduction in site closure time through workflow redesign.</small>
            </div>
            <div class="achieve-card">
                <h3>+20%</h3>
                <p>Stock Accuracy</p>
                <small>Optimization of nationwide inventory precision.</small>
            </div>
            <div class="achieve-card">
                <h3>100%</h3>
                <p>SLA Compliance</p>
                <small>Zero delays in 31+ critical infrastructure projects.</small>
            </div>
        </div>
        <div class="chart-wrap">
            <canvas id="mainChart" height="70"></canvas>
        </div>
    </section>

    <section id="experience" class="section">
        <h2 style="font-size: 1.5rem; margin-bottom: 15px;">Professional Trajectory</h2>
        
        <div class="exp-box">
            <div class="exp-header">
                <div>
                    <h3 style="color: var(--white); font-size: 1.2rem;">Inventory & Logistics Analyst</h3>
                    <span style="color: var(--highlight); font-weight: bold;">HUAWEI MÉXICO</span>
                </div>
                <div style="color: var(--highlight); font-size: 0.8rem;">2023 — Present</div>
            </div>
            <div class="bullet-item">
                <div class="icon-circle">🌪️</div>
                <div>
                    <strong>Disaster Relief:</strong> Orchestrated emergency deliveries during the Acapulco Hurricane crisis. <span class="tag tag-warn">CRISIS MGMT</span>
                </div>
            </div>
            <div class="bullet-item">
                <div class="icon-circle">🏟️</div>
                <div>
                    <strong>World Cup 2026:</strong> Managed delivery of critical radio base equipment for stadiums. <span class="tag tag-ok">GOAL ACHIEVED</span>
                </div>
            </div>
            <div class="bullet-item">
                <div class="icon-circle">📊</div>
                <div>
                    <strong>Analytics:</strong> Developed Power BI dashboards for 4 national warehouses.
                </div>
            </div>
        </div>

        <div class="exp-box">
            <div class="exp-header">
                <div>
                    <h3 style="color: var(--white); font-size: 1.2rem;">Procurement Specialist</h3>
                    <span style="color: var(--highlight); font-weight: bold;">HUAWEI MÉXICO</span>
                </div>
                <div style="color: var(--highlight); font-size: 0.8rem;">2022 — 2023</div>
            </div>
            <div class="bullet-item">
                <div class="icon-circle">📦</div>
                <div>
                    <strong>FOB Specialist:</strong> Management of mission-critical equipment (UPS, HVAC). <span class="tag tag-ok">FOB EXPERT</span>
                </div>
            </div>
            <div class="bullet-item">
                <div class="icon-circle">🤝</div>
                <div>
                    <strong>Vendor Orchestration:</strong> Coordinated 31 strategic partners nationwide.
                </div>
            </div>
        </div>
    </section>

    <section id="skills" class="section">
        <h2 style="font-size: 1.5rem; margin-bottom: 10px;">Education & Capabilities</h2>
        <div style="background: rgba(255,255,255,0.03); padding: 20px; border-radius: 15px;">
            <p style="color: var(--white); font-weight: bold;">Education: <span style="font-weight: normal; color: var(--text);">B.S. in Industrial Engineering / Logistics</span></p>
            <p style="color: var(--white); font-weight: bold; margin-top: 10px;">Languages: <span style="font-weight: normal; color: var(--text);">Spanish (Native) | English (Professional Proficiency)</span></p>
            
            <div class="pill-container">
                <span class="pill">Power BI</span>
                <span class="pill">Advanced Excel</span>
                <span class="pill">Incoterms 2020</span>
                <span class="pill">ERP Systems</span>
                <span class="pill">SLA Management</span>
                <span class="pill">Reverse Logistics</span>
            </div>
        </div>
    </section>

    <footer style="padding: 30px; text-align: center; border-top: 1px solid var(--accent); font-size: 0.8rem;">
        <p>&copy; 2026 David Vicente Calzada | Supply Chain Excellence</p>
    </footer>

    <script>
        const ctx = document.getElementById('mainChart').getContext('2d');
        new Chart(ctx, {
            type: 'line',
            data: {
                labels: ['Q1', 'Q2', 'Q3', 'Q4', 'Current'],
                datasets: [{
                    label: 'Efficiency %',
                    data: [50, 55, 62, 68, 70],
                    borderColor: '#00b4d8',
                    backgroundColor: 'rgba(0, 180, 216, 0.1)',
                    fill: true,
                    tension: 0.4
                }]
            },
            options: {
                responsive: true,
                plugins: { legend: { display: false } },
                scales: {
                    y: { ticks: { color: '#e0e1dd' }, grid: { color: '#415a77' } },
                    x: { ticks: { color: '#e0e1dd' }, grid: { display: false } }
                }
            }
        });
    </script>
</body>
</html>
