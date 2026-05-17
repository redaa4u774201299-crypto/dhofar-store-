# dhofar-store-
ظَفَار لِلْفِضِّيَّاتِ وَالتُّحَفِ والمرجان
<!DOCTYPE html>
<html lang="en" dir="ltr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dhofar Silver, Antiques & Coral Store</title>
    <style>
        :root {
            --gold: #c9a050;
            --gold-dark: #a07828;
            --gold-light: #f0d78c;
            --bg-dark: #1a1008;
            --bg-card: #241e15;
            --bg-panel: #2a2218;
            --text: #e8dcc8;
            --text-muted: #b8a88a;
            --border: #4a3820;
            --accent: #d4a843;
            --danger: #c0392b;
            --success: #27ae60;
            --shadow-gold: 0 0 20px rgba(201, 160, 80, 0.3);
            --radius: 12px;
            --transition: 0.3s ease;
        }
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body {
            font-family: 'Segoe UI', 'Tahoma', 'Arial', sans-serif;
            background: var(--bg-dark);
            background-image:
                radial-gradient(ellipse at top center, rgba(201, 160, 80, 0.08) 0%, transparent 60%),
                radial-gradient(ellipse at bottom center, rgba(160, 120, 40, 0.05) 0%, transparent 60%);
            color: var(--text);
            min-height: 100vh;
            line-height: 1.7;
            overflow-x: hidden;
        }
        .particles {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 0;
            overflow: hidden;
        }
        .particle {
            position: absolute;
            width: 3px;
            height: 3px;
            background: var(--gold-light);
            border-radius: 50%;
            animation: floatUp 8s infinite ease-in;
            opacity: 0;
        }
        @keyframes floatUp {
            0% { transform: translateY(100vh) scale(0); opacity: 0; }
            10% { opacity: 0.8; }
            30% { opacity: 0.5; }
            70% { opacity: 0.3; }
            100% { transform: translateY(-10vh) scale(1.5); opacity: 0; }
        }
        .main-container {
            position: relative;
            z-index: 1;
            max-width: 1200px;
            margin: 0 auto;
            padding: 10px 16px 100px;
        }
        .header {
            text-align: center;
            padding: 20px 16px 14px;
            position: relative;
        }
        .header-top-row {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 14px;
            flex-wrap: wrap;
        }
        .logo-container {
            position: relative;
            width: 90px;
            height: 90px;
            border-radius: 50%;
            border: 3px solid var(--gold);
            overflow: hidden;
            flex-shrink: 0;
            box-shadow: var(--shadow-gold), 0 0 40px rgba(201, 160, 80, 0.15);
            cursor: pointer;
            transition: var(--transition);
            background: var(--bg-panel);
            display: flex;
            align-items: center;
            justify-content: center;
        }
        .logo-container:hover {
            transform: scale(1.05);
            box-shadow: 0 0 30px rgba(201, 160, 80, 0.5);
        }
        .logo-container img { width: 100%; height: 100%; object-fit: cover; }
        .logo-placeholder { font-size: 40px; color
