<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>🎄 Christmas Command Center</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600;700&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        * { box-sizing: border-box; margin: 0; padding: 0; }
        
        :root {
            --bg: #0a1628;
            --bg-lighter: #0f1f35;
            --sidebar-bg: rgba(15, 23, 42, 0.95);
            --card: rgba(255,255,255,0.03);
            --card-border: rgba(255,255,255,0.08);
            --card-hover: rgba(255,255,255,0.06);
            --text: #ffffff;
            --text-secondary: rgba(255,255,255,0.6);
            --text-muted: rgba(255,255,255,0.4);
            --accent: #10b981;
            --accent-glow: rgba(16,185,129,0.3);
            --red: #ef4444;
            --red-glow: rgba(239,68,68,0.3);
            --gold: #fbbf24;
            --gold-glow: rgba(251,191,36,0.3);
            --blue: #3b82f6;
            --purple: #8b5cf6;
            --sidebar-width: 280px;
            --sidebar-collapsed: 80px;
        }

        body {
            font-family: 'Inter', system-ui, sans-serif;
            background: var(--bg);
            color: var(--text);
            min-height: 100vh;
            overflow-x: hidden;
        }

        /* Snowfall */
        .snowfall {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 1000;
            overflow: hidden;
        }

        .snowflake {
            position: absolute;
            top: -20px;
            color: white;
            font-size: 1rem;
            animation: fall linear infinite;
            opacity: 0.8;
            text-shadow: 0 0 5px rgba(255,255,255,0.5);
        }

        @keyframes fall {
            0% { transform: translateY(-20px) rotate(0deg); }
            100% { transform: translateY(100vh) rotate(360deg); }
        }

        /* Ambient glow */
        .ambient-glow {
            position: fixed;
            width: 600px;
            height: 600px;
            border-radius: 50%;
            filter: blur(150px);
            opacity: 0.15;
            pointer-events: none;
            z-index: 0;
        }
        .glow-1 { background: #10b981; top: -200px; left: -200px; }
        .glow-2 { background: #ef4444; bottom: -200px; right: -200px; }
        .glow-3 { background: #fbbf24; top: 50%; left: 50%; transform: translate(-50%, -50%); opacity: 0.08; }

        /* Sidebar */
        .sidebar {
            position: fixed;
            top: 0;
            left: 0;
            width: var(--sidebar-width);
            height: 100vh;
            background: var(--sidebar-bg);
            backdrop-filter: blur(20px);
            border-right: 1px solid var(--card-border);
            z-index: 100;
            display: flex;
            flex-direction: column;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            overflow: hidden;
        }

        .sidebar.collapsed {
            width: var(--sidebar-collapsed);
        }

        .sidebar-header {
            padding: 24px 20px;
            border-bottom: 1px solid var(--card-border);
            display: flex;
            align-items: center;
            gap: 14px;
        }

        .sidebar-logo {
            width: 44px;
            height: 44px;
            background: linear-gradient(135deg, var(--accent) 0%, var(--gold) 100%);
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 24px;
            flex-shrink: 0;
        }

        .sidebar-brand {
            overflow: hidden;
            transition: opacity 0.2s;
        }

        .sidebar.collapsed .sidebar-brand {
            opacity: 0;
            width: 0;
        }

        .sidebar-brand h1 {
            font-family: 'Playfair Display', serif;
            font-size: 18px;
            font-weight: 700;
            white-space: nowrap;
        }

        .sidebar-brand p {
            font-size: 11px;
            color: var(--text-muted);
            white-space: nowrap;
        }

        .sidebar-toggle {
            position: absolute;
            top: 28px;
            right: -14px;
            width: 28px;
            height: 28px;
            background: var(--bg-lighter);
            border: 1px solid var(--card-border);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            color: var(--text-secondary);
            font-size: 12px;
            transition: all 0.2s;
            z-index: 101;
        }

        .sidebar-toggle:hover {
            background: var(--accent);
            color: white;
            border-color: var(--accent);
        }

        .sidebar.collapsed .sidebar-toggle {
            transform: rotate(180deg);
        }

        /* Sidebar Navigation */
        .sidebar-nav {
            flex: 1;
            padding: 20px 12px;
            overflow-y: auto;
        }

        .nav-section {
            margin-bottom: 24px;
        }

        .nav-section-title {
            font-size: 10px;
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 1.5px;
            color: var(--text-muted);
            padding: 0 12px;
            margin-bottom: 8px;
            white-space: nowrap;
            overflow: hidden;
        }

        .sidebar.collapsed .nav-section-title {
            opacity: 0;
        }

        .nav-item {
            display: flex;
            align-items: center;
            gap: 12px;
            padding: 12px 14px;
            border-radius: 10px;
            cursor: pointer;
            transition: all 0.2s;
            color: var(--text-secondary);
            text-decoration: none;
            margin-bottom: 4px;
            position: relative;
        }

        .nav-item:hover {
            background: var(--card-hover);
            color: var(--text);
        }

        .nav-item.active {
            background: rgba(16, 185, 129, 0.15);
            color: var(--accent);
        }

        .nav-item.active::before {
            content: '';
            position: absolute;
            left: 0;
            top: 50%;
            transform: translateY(-50%);
            width: 3px;
            height: 20px;
            background: var(--accent);
            border-radius: 0 3px 3px 0;
        }

        .nav-icon {
            width: 22px;
            height: 22px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 16px;
            flex-shrink: 0;
        }

        .nav-text {
            font-size: 14px;
            font-weight: 500;
            white-space: nowrap;
            overflow: hidden;
            transition: opacity 0.2s;
        }

        .sidebar.collapsed .nav-text {
            opacity: 0;
            width: 0;
        }

        .nav-badge {
            margin-left: auto;
            background: var(--accent);
            color: white;
            font-size: 11px;
            font-weight: 600;
            padding: 2px 8px;
            border-radius: 10px;
            transition: opacity 0.2s;
        }

        .sidebar.collapsed .nav-badge {
            opacity: 0;
        }

        /* Sidebar Stats */
        .sidebar-stats {
            padding: 16px;
            border-top: 1px solid var(--card-border);
        }

        .sidebar-stats-title {
            font-size: 10px;
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 1.5px;
            color: var(--text-muted);
            margin-bottom: 12px;
            white-space: nowrap;
            overflow: hidden;
        }

        .sidebar.collapsed .sidebar-stats-title {
            opacity: 0;
        }

        .stats-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 8px;
        }

        .sidebar.collapsed .stats-grid {
            grid-template-columns: 1fr;
        }

        .stat-mini {
            background: var(--card);
            border: 1px solid var(--card-border);
            border-radius: 10px;
            padding: 12px;
            text-align: center;
            transition: all 0.2s;
        }

        .stat-mini:hover {
            background: var(--card-hover);
        }

        .stat-mini-icon {
            font-size: 18px;
            margin-bottom: 4px;
        }

        .stat-mini-value {
            font-size: 18px;
            font-weight: 700;
        }

        .stat-mini-label {
            font-size: 10px;
            color: var(--text-muted);
            white-space: nowrap;
            overflow: hidden;
            text-overflow: ellipsis;
        }

        .sidebar.collapsed .stat-mini-label {
            display: none;
        }

        /* Sidebar Footer */
        .sidebar-footer {
            padding: 16px;
            border-top: 1px solid var(--card-border);
        }

        .user-card {
            display: flex;
            align-items: center;
            gap: 12px;
            padding: 10px;
            background: var(--card);
            border-radius: 12px;
            cursor: pointer;
            transition: all 0.2s;
        }

        .user-card:hover {
            background: var(--card-hover);
        }

        .user-avatar {
            width: 36px;
            height: 36px;
            border-radius: 10px;
            background: linear-gradient(135deg, var(--purple) 0%, var(--blue) 100%);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 16px;
            flex-shrink: 0;
        }

        .user-info {
            overflow: hidden;
            transition: opacity 0.2s;
        }

        .sidebar.collapsed .user-info {
            opacity: 0;
            width: 0;
        }

        .user-name {
            font-size: 13px;
            font-weight: 600;
            white-space: nowrap;
        }

        .user-role {
            font-size: 11px;
            color: var(--text-muted);
            white-space: nowrap;
        }

        /* Main Content */
        .main-content {
            margin-left: var(--sidebar-width);
            transition: margin-left 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            min-height: 100vh;
            padding-bottom: 80px;
        }

        .sidebar.collapsed ~ .main-content {
            margin-left: var(--sidebar-collapsed);
        }

        .container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 40px 32px;
            position: relative;
            z-index: 1;
        }

        /* Header */
        .header {
            margin-bottom: 40px;
        }

        .header-top {
            display: flex;
            align-items: center;
            justify-content: space-between;
            margin-bottom: 24px;
        }

        .header-left h1 {
            font-family: 'Playfair Display', serif;
            font-size: 36px;
            font-weight: 700;
            background: linear-gradient(135deg, #ffffff 0%, #10b981 50%, #ef4444 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin-bottom: 6px;
        }

        .header-left p {
            color: var(--text-secondary);
            font-size: 14px;
        }

        .header-actions {
            display: flex;
            gap: 10px;
        }

        /* Countdown */
        .countdown-section {
            background: linear-gradient(135deg, rgba(16,185,129,0.1) 0%, rgba(239,68,68,0.1) 100%);
            border: 1px solid var(--card-border);
            border-radius: 20px;
            padding: 32px;
            margin-bottom: 32px;
            text-align: center;
            backdrop-filter: blur(20px);
        }

        .countdown-label {
            font-size: 13px;
            text-transform: uppercase;
            letter-spacing: 3px;
            color: var(--text-muted);
            margin-bottom: 20px;
        }

        .countdown-grid {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }

        .countdown-item {
            background: rgba(0,0,0,0.3);
            border-radius: 14px;
            padding: 20px 28px;
            min-width: 100px;
            border: 1px solid var(--card-border);
        }

        .countdown-value {
            font-family: 'Playfair Display', serif;
            font-size: 44px;
            font-weight: 700;
            background: linear-gradient(180deg, #ffffff 0%, var(--accent) 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            line-height: 1;
        }

        .countdown-unit {
            font-size: 11px;
            text-transform: uppercase;
            letter-spacing: 2px;
            color: var(--text-muted);
            margin-top: 6px;
        }

        /* Dashboard Grid */
        .dashboard-grid {
            display: grid;
            grid-template-columns: 2fr 1fr;
            gap: 24px;
        }

        @media (max-width: 1200px) {
            .dashboard-grid { grid-template-columns: 1fr; }
        }

        /* Card */
        .card {
            background: var(--card);
            border: 1px solid var(--card-border);
            border-radius: 16px;
            padding: 24px;
            margin-bottom: 24px;
            transition: all 0.3s;
        }

        .card:hover {
            background: var(--card-hover);
        }

        .card-header {
            display: flex;
            align-items: center;
            justify-content: space-between;
            margin-bottom: 20px;
        }

        .card-title {
            display: flex;
            align-items: center;
            gap: 10px;
            font-size: 16px;
            font-weight: 600;
        }

        .card-title span { font-size: 20px; }

        /* Buttons */
        .btn {
            display: inline-flex;
            align-items: center;
            gap: 6px;
            padding: 8px 14px;
            font-size: 13px;
            font-weight: 500;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            transition: all 0.2s;
        }

        .btn-primary {
            background: var(--accent);
            color: white;
        }

        .btn-primary:hover { background: #0d9668; transform: scale(1.02); }

        .btn-ghost {
            background: transparent;
            color: var(--text-secondary);
            border: 1px solid var(--card-border);
        }

        .btn-ghost:hover { background: var(--card-hover); color: white; }

        .btn-icon {
            width: 36px;
            height: 36px;
            padding: 0;
            justify-content: center;
            border-radius: 10px;
        }

        /* Table */
        .table-wrapper {
            overflow-x: auto;
            margin: 0 -24px;
            padding: 0 24px;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            font-size: 13px;
        }

        th {
            text-align: left;
            padding: 10px 14px;
            font-size: 10px;
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 1px;
            color: var(--text-muted);
            border-bottom: 1px solid var(--card-border);
        }

        td {
            padding: 12px 14px;
            border-bottom: 1px solid var(--card-border);
            vertical-align: middle;
        }

        tr:hover td { background: rgba(255,255,255,0.02); }
        tr:last-child td { border-bottom: none; }

        input, select {
            background: transparent;
            border: none;
            color: var(--text);
            font: inherit;
            outline: none;
            width: 100%;
        }

        input::placeholder { color: var(--text-muted); }
        select { cursor: pointer; }
        select option { background: var(--bg); color: var(--text); }

        /* Tags */
        .tag {
            display: inline-flex;
            align-items: center;
            padding: 4px 10px;
            border-radius: 6px;
            font-size: 11px;
            font-weight: 500;
        }

        .tag-green { background: rgba(16,185,129,0.2); color: #34d399; }
        .tag-yellow { background: rgba(251,191,36,0.2); color: #fcd34d; }
        .tag-blue { background: rgba(59,130,246,0.2); color: #60a5fa; }
        .tag-red { background: rgba(239,68,68,0.2); color: #f87171; }
        .tag-purple { background: rgba(139,92,246,0.2); color: #a78bfa; }

        /* Delete button */
        .delete-btn {
            opacity: 0;
            color: var(--text-muted);
            cursor: pointer;
            font-size: 16px;
            transition: all 0.2s;
        }

        tr:hover .delete-btn, .task-item:hover .delete-btn { opacity: 1; }
        .delete-btn:hover { color: var(--red); }

        /* Budget */
        .budget-display {
            display: flex;
            justify-content: space-between;
            align-items: flex-end;
            margin-bottom: 16px;
        }

        .budget-amount {
            font-size: 36px;
            font-weight: 700;
        }

        .budget-total {
            font-size: 13px;
            color: var(--text-muted);
        }

        .budget-total input {
            width: 70px;
            text-align: right;
            font-weight: 600;
            color: var(--text);
        }

        .progress-bar {
            height: 10px;
            background: rgba(255,255,255,0.1);
            border-radius: 5px;
            overflow: hidden;
            margin-bottom: 10px;
        }

        .progress-fill {
            height: 100%;
            border-radius: 5px;
            transition: all 0.5s ease;
            background: linear-gradient(90deg, var(--accent) 0%, #34d399 100%);
        }

        .progress-fill.over { background: linear-gradient(90deg, var(--red) 0%, #f87171 100%); }

        .budget-stats {
            display: flex;
            justify-content: space-between;
            font-size: 12px;
            color: var(--text-secondary);
        }

        /* Tasks */
        .task-item {
            display: flex;
            align-items: center;
            gap: 12px;
            padding: 12px 0;
            border-bottom: 1px solid var(--card-border);
        }

        .task-item:last-child { border-bottom: none; }

        .checkbox {
            width: 20px;
            height: 20px;
            border: 2px solid var(--card-border);
            border-radius: 5px;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            transition: all 0.2s;
            flex-shrink: 0;
            font-size: 11px;
        }

        .checkbox:hover { border-color: var(--accent); }

        .checkbox.checked {
            background: var(--accent);
            border-color: var(--accent);
        }

        .task-text { flex: 1; font-size: 13px; }
        .task-text.done { text-decoration: line-through; color: var(--text-muted); }

        /* Calendar */
        .calendar-grid {
            display: grid;
            grid-template-columns: repeat(7, 1fr);
            gap: 4px;
            text-align: center;
            font-size: 12px;
        }

        .cal-header {
            color: var(--text-muted);
            font-size: 10px;
            font-weight: 600;
            padding: 6px 0;
        }

        .cal-day {
            padding: 8px 4px;
            border-radius: 6px;
            cursor: pointer;
            transition: all 0.2s;
        }

        .cal-day:hover { background: var(--card-hover); }
        .cal-day.today { background: var(--accent); color: white; font-weight: 600; }
        .cal-day.christmas { background: var(--red); color: white; font-weight: 600; }
        .cal-day.empty { opacity: 0; pointer-events: none; }

        /* Weather */
        .weather-card {
            background: linear-gradient(135deg, rgba(59,130,246,0.15) 0%, rgba(139,92,246,0.15) 100%);
            text-align: center;
            padding: 28px;
        }

        .weather-icon { font-size: 48px; margin-bottom: 8px; }
        .weather-temp { font-size: 36px; font-weight: 700; }
        .weather-desc { color: var(--text-secondary); font-size: 13px; }
        .weather-location { font-size: 11px; color: var(--text-muted); margin-top: 6px; }

        /* Santa Status */
        .santa-card {
            background: linear-gradient(135deg, rgba(239,68,68,0.15) 0%, rgba(251,191,36,0.15) 100%);
        }

        .santa-status {
            display: flex;
            align-items: center;
            gap: 12px;
            margin-top: 14px;
        }

        .santa-dot {
            width: 10px;
            height: 10px;
            background: var(--accent);
            border-radius: 50%;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0%, 100% { box-shadow: 0 0 0 0 var(--accent-glow); }
            50% { box-shadow: 0 0 0 8px transparent; }
        }

        /* Database Status Bar */
        .db-status-bar {
            position: fixed;
            bottom: 0;
            left: var(--sidebar-width);
            right: 0;
            background: rgba(10, 22, 40, 0.95);
            backdrop-filter: blur(10px);
            border-top: 1px solid var(--card-border);
            padding: 10px 24px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            z-index: 99;
            font-size: 11px;
            transition: left 0.3s cubic-bezier(0.4, 0, 0.2, 1);
        }

        .sidebar.collapsed ~ .main-content ~ .db-status-bar,
        .sidebar.collapsed ~ .db-status-bar {
            left: var(--sidebar-collapsed);
        }

        .db-status-left {
            display: flex;
            align-items: center;
            gap: 16px;
        }

        .db-indicator {
            display: flex;
            align-items: center;
            gap: 5px;
            color: var(--text-secondary);
        }

        .db-dot {
            width: 7px;
            height: 7px;
            border-radius: 50%;
            background: var(--accent);
            animation: pulse 2s infinite;
        }

        .db-dot.saving { background: var(--gold); }
        .db-dot.error { background: var(--red); }

        .db-count {
            background: rgba(16,185,129,0.2);
            color: #34d399;
            padding: 2px 6px;
            border-radius: 8px;
            font-size: 10px;
            margin-left: 3px;
        }

        .db-actions {
            display: flex;
            gap: 6px;
        }

        .db-btn {
            padding: 5px 10px;
            font-size: 10px;
            background: var(--card);
            border: 1px solid var(--card-border);
            color: var(--text-secondary);
            border-radius: 5px;
            cursor: pointer;
            transition: all 0.2s;
        }

        .db-btn:hover {
            background: var(--card-hover);
            color: var(--text);
        }

        /* Toast */
        .toast-container {
            position: fixed;
            top: 20px;
            right: 20px;
            z-index: 2000;
            display: flex;
            flex-direction: column;
            gap: 10px;
        }

        .toast {
            background: rgba(10, 22, 40, 0.95);
            backdrop-filter: blur(10px);
            border: 1px solid var(--card-border);
            padding: 12px 18px;
            border-radius: 10px;
            display: flex;
            align-items: center;
            gap: 10px;
            animation: slideIn 0.3s ease;
            box-shadow: 0 10px 40px rgba(0,0,0,0.3);
            font-size: 13px;
        }

        .toast.success { border-left: 3px solid var(--accent); }
        .toast.error { border-left: 3px solid var(--red); }
        .toast.info { border-left: 3px solid var(--blue); }

        @keyframes slideIn {
            from { transform: translateX(100%); opacity: 0; }
            to { transform: translateX(0); opacity: 1; }
        }

        /* Modal */
        .modal-overlay {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: rgba(0,0,0,0.7);
            backdrop-filter: blur(5px);
            display: flex;
            align-items: center;
            justify-content: center;
            z-index: 3000;
            opacity: 0;
            visibility: hidden;
            transition: all 0.3s;
        }

        .modal-overlay.active {
            opacity: 1;
            visibility: visible;
        }

        .modal {
            background: var(--bg);
            border: 1px solid var(--card-border);
            border-radius: 16px;
            padding: 24px;
            width: 90%;
            max-width: 480px;
            transform: scale(0.9);
            transition: transform 0.3s;
        }

        .modal-overlay.active .modal {
            transform: scale(1);
        }

        .modal-header {
            display: flex;
            align-items: center;
            justify-content: space-between;
            margin-bottom: 20px;
        }

        .modal-title {
            font-size: 16px;
            font-weight: 600;
        }

        .modal-close {
            width: 28px;
            height: 28px;
            border-radius: 6px;
            border: none;
            background: var(--card);
            color: var(--text-secondary);
            cursor: pointer;
            font-size: 16px;
        }

        .modal-close:hover { background: var(--card-hover); color: var(--text); }

        .form-group { margin-bottom: 14px; }

        .form-label {
            display: block;
            font-size: 11px;
            font-weight: 500;
            color: var(--text-secondary);
            margin-bottom: 5px;
        }

        .form-input {
            width: 100%;
            padding: 10px 12px;
            background: var(--card);
            border: 1px solid var(--card-border);
            border-radius: 8px;
            color: var(--text);
            font-size: 13px;
            outline: none;
        }

        .form-input:focus {
            border-color: var(--accent);
        }

        .modal-footer {
            display: flex;
            justify-content: flex-end;
            gap: 10px;
            margin-top: 20px;
        }

        /* Responsive */
        @media (max-width: 900px) {
            .sidebar {
                transform: translateX(-100%);
            }
            .sidebar.open {
                transform: translateX(0);
            }
            .main-content {
                margin-left: 0 !important;
            }
            .db-status-bar {
                left: 0 !important;
            }
            .mobile-toggle {
                display: flex !important;
            }
        }

        .mobile-toggle {
            display: none;
            position: fixed;
            top: 20px;
            left: 20px;
            z-index: 150;
            width: 44px;
            height: 44px;
            background: var(--sidebar-bg);
            backdrop-filter: blur(20px);
            border: 1px solid var(--card-border);
            border-radius: 12px;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            font-size: 20px;
        }

        .mobile-toggle:hover {
            background: var(--card-hover);
        }

        /* Scrollbar */
        ::-webkit-scrollbar { width: 5px; height: 5px; }
        ::-webkit-scrollbar-track { background: transparent; }
        ::-webkit-scrollbar-thumb { background: var(--card-border); border-radius: 3px; }

        /* Notion-style Cover Image */
        .cover-container {
            position: relative;
            width: 100%;
            height: 280px;
            overflow: hidden;
        }

        .cover-image {
            width: 100%;
            height: 100%;
            background-image: url('https://images.unsplash.com/photo-1512389142860-9c449e58a814?w=1600&q=80');
            background-size: cover;
            background-position: center 40%;
            transition: transform 0.3s ease;
        }

        .cover-overlay {
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(180deg, 
                transparent 0%, 
                transparent 50%, 
                rgba(10, 22, 40, 0.3) 80%, 
                rgba(10, 22, 40, 0.95) 100%
            );
            pointer-events: none;
        }

        .cover-controls {
            position: absolute;
            bottom: 16px;
            right: 16px;
            display: flex;
            gap: 8px;
            opacity: 0;
            transition: opacity 0.2s ease;
        }

        .cover-container:hover .cover-controls {
            opacity: 1;
        }

        .cover-btn {
            padding: 6px 12px;
            font-size: 12px;
            font-weight: 500;
            background: rgba(0, 0, 0, 0.6);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
            border-radius: 6px;
            color: white;
            cursor: pointer;
            transition: all 0.2s ease;
        }

        .cover-btn:hover {
            background: rgba(0, 0, 0, 0.8);
            border-color: rgba(255, 255, 255, 0.4);
        }

        /* Page Icon */
        .page-icon {
            position: absolute;
            bottom: -40px;
            left: 80px;
            width: 100px;
            height: 100px;
            background: var(--bg);
            border: 4px solid var(--bg);
            border-radius: 16px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 60px;
            cursor: pointer;
            transition: all 0.2s ease;
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.3);
            z-index: 10;
        }

        .page-icon:hover {
            transform: scale(1.05);
            box-shadow: 0 12px 40px rgba(0, 0, 0, 0.4);
        }

        @media (max-width: 900px) {
            .cover-container {
                height: 200px;
            }
            .page-icon {
                left: 32px;
                width: 80px;
                height: 80px;
                font-size: 48px;
                bottom: -30px;
            }
            .header {
                margin-top: 40px !important;
            }
        }
    </style>
</head>
<body>
    <!-- Ambient Glow -->
    <div class="ambient-glow glow-1"></div>
    <div class="ambient-glow glow-2"></div>
    <div class="ambient-glow glow-3"></div>

    <!-- Snowfall -->
    <div class="snowfall" id="snowfall"></div>

    <!-- Mobile Toggle -->
    <div class="mobile-toggle" onclick="toggleMobileSidebar()">☰</div>

    <!-- Sidebar -->
    <aside class="sidebar" id="sidebar">
        <div class="sidebar-toggle" onclick="toggleSidebar()">◀</div>
        
        <div class="sidebar-header">
            <div class="sidebar-logo">🎄</div>
            <div class="sidebar-brand">
                <h1>Christmas HQ</h1>
                <p>Command Center 2024</p>
            </div>
        </div>

        <nav class="sidebar-nav">
            <div class="nav-section">
                <div class="nav-section-title">Main</div>
                <a href="#dashboard" class="nav-item active" data-section="dashboard">
                    <div class="nav-icon">📊</div>
                    <span class="nav-text">Dashboard</span>
                </a>
                <a href="#gifts" class="nav-item" data-section="gifts">
                    <div class="nav-icon">🎁</div>
                    <span class="nav-text">Gift Tracker</span>
                    <span class="nav-badge" id="nav-gifts-count">0</span>
                </a>
                <a href="#guests" class="nav-item" data-section="guests">
                    <div class="nav-icon">👥</div>
                    <span class="nav-text">Guest List</span>
                    <span class="nav-badge" id="nav-guests-count">0</span>
                </a>
                <a href="#menu" class="nav-item" data-section="menu">
                    <div class="nav-icon">🍽️</div>
                    <span class="nav-text">Menu Planner</span>
                </a>
            </div>

            <div class="nav-section">
                <div class="nav-section-title">Planning</div>
                <a href="#shopping" class="nav-item" data-section="shopping">
                    <div class="nav-icon">🛒</div>
                    <span class="nav-text">Shopping List</span>
                </a>
                <a href="#events" class="nav-item" data-section="events">
                    <div class="nav-icon">📅</div>
                    <span class="nav-text">Events</span>
                </a>
                <a href="#tasks" class="nav-item" data-section="tasks">
                    <div class="nav-icon">✅</div>
                    <span class="nav-text">Tasks</span>
                    <span class="nav-badge" id="nav-tasks-count">0</span>
                </a>
            </div>

            <div class="nav-section">
                <div class="nav-section-title">Settings</div>
                <a href="#" class="nav-item" onclick="exportData(); return false;">
                    <div class="nav-icon">📤</div>
                    <span class="nav-text">Export Data</span>
                </a>
                <a href="#" class="nav-item" onclick="importData(); return false;">
                    <div class="nav-icon">📥</div>
                    <span class="nav-text">Import Data</span>
                </a>
                <a href="#" class="nav-item" onclick="resetData(); return false;">
                    <div class="nav-icon">🔄</div>
                    <span class="nav-text">Reset All</span>
                </a>
            </div>
        </nav>

        <div class="sidebar-stats">
            <div class="sidebar-stats-title">Quick Stats</div>
            <div class="stats-grid">
                <div class="stat-mini">
                    <div class="stat-mini-icon">🎁</div>
                    <div class="stat-mini-value" id="side-stat-gifts">0</div>
                    <div class="stat-mini-label">Gifts</div>
                </div>
                <div class="stat-mini">
                    <div class="stat-mini-icon">✅</div>
                    <div class="stat-mini-value" id="side-stat-tasks">0%</div>
                    <div class="stat-mini-label">Done</div>
                </div>
            </div>
        </div>

        <div class="sidebar-footer">
            <div class="user-card">
                <div class="user-avatar">🎅</div>
                <div class="user-info">
                    <div class="user-name">Santa Claus</div>
                    <div class="user-role">Chief Happiness Officer</div>
                </div>
            </div>
        </div>
    </aside>

    <!-- Main Content -->
    <main class="main-content">
        <!-- Notion-style Cover Image -->
        <div class="cover-container" id="cover-container">
            <div class="cover-image" id="cover-image"></div>
            <div class="cover-overlay"></div>
            <div class="cover-controls">
                <button class="cover-btn" onclick="changeCover()">🖼️ Change cover</button>
                <button class="cover-btn" onclick="repositionCover()">↕️ Reposition</button>
            </div>
            <!-- Page Icon -->
            <div class="page-icon" id="page-icon" onclick="changeIcon()">🎄</div>
        </div>

        <div class="container">
            <!-- Header -->
            <header class="header" style="margin-top: 60px;">
                <div class="header-top">
                    <div class="header-left">
                        <h1>🎄 Christmas Command Center</h1>
                        <p>Your complete holiday mission control • All systems operational</p>
                    </div>
                    <div class="header-actions">
                        <button class="btn btn-ghost" onclick="exportData()">📤 Export</button>
                        <button class="btn btn-primary" onclick="addGift()">+ Add Gift</button>
                    </div>
                </div>
            </header>

            <!-- Countdown -->
            <section class="countdown-section">
                <div class="countdown-label">🎅 Santa Arrives In</div>
                <div class="countdown-grid">
                    <div class="countdown-item">
                        <div class="countdown-value" id="days">00</div>
                        <div class="countdown-unit">Days</div>
                    </div>
                    <div class="countdown-item">
                        <div class="countdown-value" id="hours">00</div>
                        <div class="countdown-unit">Hours</div>
                    </div>
                    <div class="countdown-item">
                        <div class="countdown-value" id="minutes">00</div>
                        <div class="countdown-unit">Minutes</div>
                    </div>
                    <div class="countdown-item">
                        <div class="countdown-value" id="seconds">00</div>
                        <div class="countdown-unit">Seconds</div>
                    </div>
                </div>
            </section>

            <!-- Dashboard Grid -->
            <div class="dashboard-grid">
                <!-- Left Column -->
                <div class="left-column">
                    <!-- Gift Tracker -->
                    <div class="card" id="gifts">
                        <div class="card-header">
                            <div class="card-title"><span>🎁</span> Gift Tracker</div>
                            <button class="btn btn-primary" onclick="addGift()">+ Add Gift</button>
                        </div>
                        <div class="table-wrapper">
                            <table>
                                <thead>
                                    <tr>
                                        <th>Recipient</th>
                                        <th>Gift</th>
                                        <th>Price</th>
                                        <th>Status</th>
                                        <th>Priority</th>
                                        <th></th>
                                    </tr>
                                </thead>
                                <tbody id="gifts-body"></tbody>
                            </table>
                        </div>
                    </div>

                    <!-- Guest List -->
                    <div class="card" id="guests">
                        <div class="card-header">
                            <div class="card-title"><span>👥</span> Guest List</div>
                            <button class="btn btn-primary" onclick="addGuest()">+ Add Guest</button>
                        </div>
                        <div class="table-wrapper">
                            <table>
                                <thead>
                                    <tr>
                                        <th>Name</th>
                                        <th>Relationship</th>
                                        <th>Dietary</th>
                                        <th>RSVP</th>
                                        <th></th>
                                    </tr>
                                </thead>
                                <tbody id="guests-body"></tbody>
                            </table>
                        </div>
                    </div>

                    <!-- Menu Planner -->
                    <div class="card" id="menu">
                        <div class="card-header">
                            <div class="card-title"><span>🍽️</span> Menu Planner</div>
                            <button class="btn btn-primary" onclick="addMenuItem()">+ Add Dish</button>
                        </div>
                        <div class="table-wrapper">
                            <table>
                                <thead>
                                    <tr>
                                        <th>Dish</th>
                                        <th>Category</th>
                                        <th>Assigned To</th>
                                        <th>Status</th>
                                        <th></th>
                                    </tr>
                                </thead>
                                <tbody id="menu-body"></tbody>
                            </table>
                        </div>
                    </div>

                    <!-- Shopping List -->
                    <div class="card" id="shopping">
                        <div class="card-header">
                            <div class="card-title"><span>🛒</span> Shopping List</div>
                            <button class="btn btn-primary" onclick="addShoppingItem()">+ Add Item</button>
                        </div>
                        <div class="table-wrapper">
                            <table>
                                <thead>
                                    <tr>
                                        <th style="width:30px"></th>
                                        <th>Item</th>
                                        <th>Category</th>
                                        <th>Qty</th>
                                        <th>Price</th>
                                        <th></th>
                                    </tr>
                                </thead>
                                <tbody id="shopping-body"></tbody>
                            </table>
                        </div>
                    </div>

                    <!-- Events -->
                    <div class="card" id="events">
                        <div class="card-header">
                            <div class="card-title"><span>📅</span> Event Schedule</div>
                            <button class="btn btn-primary" onclick="addEvent()">+ Add Event</button>
                        </div>
                        <div class="table-wrapper">
                            <table>
                                <thead>
                                    <tr>
                                        <th>Date</th>
                                        <th>Time</th>
                                        <th>Event</th>
                                        <th>Location</th>
                                        <th></th>
                                    </tr>
                                </thead>
                                <tbody id="events-body"></tbody>
                            </table>
                        </div>
                    </div>
                </div>

                <!-- Right Column -->
                <div class="right-column">
                    <!-- Budget -->
                    <div class="card">
                        <div class="card-header">
                            <div class="card-title"><span>💰</span> Budget</div>
                        </div>
                        <div class="budget-display">
                            <div>
                                <div class="budget-amount" id="budget-spent">$0</div>
                                <div style="font-size:11px;color:var(--text-muted)">spent</div>
                            </div>
                            <div class="budget-total">
                                of $<input type="number" id="budget-total" value="1000" onchange="updateBudget()">
                            </div>
                        </div>
                        <div class="progress-bar">
                            <div class="progress-fill" id="budget-bar" style="width:0%"></div>
                        </div>
                        <div class="budget-stats">
                            <span id="budget-percent">0% used</span>
                            <span id="budget-remaining">$1000 left</span>
                        </div>
                    </div>

                    <!-- Weather -->
                    <div class="card weather-card">
                        <div class="weather-icon">❄️</div>
                        <div class="weather-temp">-24°</div>
                        <div class="weather-desc">Heavy Snow</div>
                        <div class="weather-location">📍 North Pole, Arctic</div>
                    </div>

                    <!-- Calendar -->
                    <div class="card">
                        <div class="card-header">
                            <div class="card-title"><span>📆</span> December 2024</div>
                        </div>
                        <div class="calendar-grid" id="calendar"></div>
                    </div>

                    <!-- Tasks -->
                    <div class="card" id="tasks">
                        <div class="card-header">
                            <div class="card-title"><span>✅</span> Tasks</div>
                            <button class="btn btn-ghost" onclick="addTask()">+ Add</button>
                        </div>
                        <div id="tasks-container"></div>
                    </div>

                    <!-- Santa Status -->
                    <div class="card santa-card">
                        <div class="card-title"><span>🎅</span> Santa Status</div>
                        <div class="santa-status">
                            <div class="santa-dot"></div>
                            <div>
                                <div style="font-weight:500;">Preparing at Workshop</div>
                                <div style="font-size:11px;color:var(--text-muted);">All elves on schedule</div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </main>

    <!-- Database Status Bar -->
    <div class="db-status-bar">
        <div class="db-status-left">
            <div class="db-indicator">
                <div class="db-dot" id="db-dot"></div>
                <span id="db-status-text">All changes saved</span>
            </div>
            <div class="db-indicator">🎁<span class="db-count" id="db-gifts-count">0</span></div>
            <div class="db-indicator">👥<span class="db-count" id="db-guests-count">0</span></div>
            <div class="db-indicator">🍽️<span class="db-count" id="db-menu-count">0</span></div>
            <div class="db-indicator">🛒<span class="db-count" id="db-shopping-count">0</span></div>
            <div class="db-indicator">📅<span class="db-count" id="db-events-count">0</span></div>
            <div class="db-indicator">✅<span class="db-count" id="db-tasks-count">0</span></div>
        </div>
        <div class="db-actions">
            <button class="db-btn" onclick="exportData()">📤 Export</button>
            <button class="db-btn" onclick="importData()">📥 Import</button>
        </div>
    </div>

    <!-- Toast Container -->
    <div class="toast-container" id="toast-container"></div>

    <!-- Import Modal -->
    <div class="modal-overlay" id="import-modal">
        <div class="modal">
            <div class="modal-header">
                <div class="modal-title">📥 Import Data</div>
                <button class="modal-close" onclick="closeImportModal()">×</button>
            </div>
            <div class="form-group">
                <label class="form-label">Paste your exported JSON data below:</label>
                <textarea class="form-input" id="import-textarea" rows="8" placeholder='{"gifts":[],"guests":[],...}'></textarea>
            </div>
            <div class="modal-footer">
                <button class="btn btn-ghost" onclick="closeImportModal()">Cancel</button>
                <button class="btn btn-primary" onclick="confirmImport()">Import Data</button>
            </div>
        </div>
    </div>

    <script>
        // State
        let state = {
            gifts: [
                { id: 1, recipient: 'Mom', gift: 'Cashmere Scarf', price: 85, status: 'wrapped', priority: 'high' },
                { id: 2, recipient: 'Dad', gift: 'Smart Watch', price: 250, status: 'bought', priority: 'high' },
                { id: 3, recipient: 'Sister', gift: 'Book Collection', price: 45, status: 'idea', priority: 'medium' },
            ],
            guests: [
                { id: 1, name: 'Grandma Rose', relationship: 'Family', dietary: 'None', rsvp: 'yes' },
                { id: 2, name: 'Uncle Bob', relationship: 'Family', dietary: 'Vegetarian', rsvp: 'yes' },
                { id: 3, name: 'Aunt Mary', relationship: 'Family', dietary: 'Gluten-free', rsvp: 'pending' },
            ],
            menu: [
                { id: 1, dish: 'Roast Turkey', category: 'main', assignedTo: 'You', status: 'planned' },
                { id: 2, dish: 'Mashed Potatoes', category: 'side', assignedTo: 'Mom', status: 'confirmed' },
                { id: 3, dish: 'Pumpkin Pie', category: 'dessert', assignedTo: 'Sister', status: 'confirmed' },
            ],
            shopping: [
                { id: 1, item: 'Turkey (12 lbs)', category: 'food', qty: 1, price: 45, bought: false },
                { id: 2, item: 'Wrapping Paper', category: 'supplies', qty: 5, price: 15, bought: true },
                { id: 3, item: 'String Lights', category: 'decor', qty: 2, price: 30, bought: true },
            ],
            events: [
                { id: 1, date: '2024-12-24', time: '18:00', event: 'Christmas Eve Dinner', location: 'Home' },
                { id: 2, date: '2024-12-25', time: '10:00', event: 'Gift Opening', location: 'Living Room' },
                { id: 3, date: '2024-12-25', time: '15:00', event: 'Christmas Dinner', location: 'Dining Room' },
            ],
            tasks: [
                { id: 1, text: 'Decorate Christmas tree', done: true },
                { id: 2, text: 'Wrap all presents', done: false },
                { id: 3, text: 'Send holiday cards', done: true },
                { id: 4, text: 'Buy groceries', done: false },
                { id: 5, text: 'Clean the house', done: false },
            ],
            budget: 1000
        };

        const STORAGE_KEY = 'christmas-hq-v3';

        // Load/Save
        function loadState() {
            try {
                const saved = localStorage.getItem(STORAGE_KEY);
                if (saved) state = { ...state, ...JSON.parse(saved) };
            } catch(e) {}
        }

        let saveTimeout;
        function saveState() {
            const dot = document.getElementById('db-dot');
            const statusText = document.getElementById('db-status-text');
            
            dot.classList.add('saving');
            statusText.textContent = 'Saving...';
            
            clearTimeout(saveTimeout);
            saveTimeout = setTimeout(() => {
                try {
                    localStorage.setItem(STORAGE_KEY, JSON.stringify(state));
                    dot.classList.remove('saving', 'error');
                    statusText.textContent = 'All changes saved';
                    updateDbStatus();
                } catch(e) {
                    dot.classList.remove('saving');
                    dot.classList.add('error');
                    statusText.textContent = 'Save failed!';
                    showToast('❌ Failed to save data', 'error');
                }
            }, 300);
        }

        // Sidebar
        function toggleSidebar() {
            document.getElementById('sidebar').classList.toggle('collapsed');
        }

        function toggleMobileSidebar() {
            document.getElementById('sidebar').classList.toggle('open');
        }

        // Snowfall
        function createSnowfall() {
            const container = document.getElementById('snowfall');
            const flakes = ['❄', '❅', '❆', '✧', '•'];
            
            for (let i = 0; i < 40; i++) {
                const flake = document.createElement('div');
                flake.className = 'snowflake';
                flake.textContent = flakes[Math.floor(Math.random() * flakes.length)];
                flake.style.left = Math.random() * 100 + '%';
                flake.style.fontSize = (Math.random() * 10 + 6) + 'px';
                flake.style.opacity = Math.random() * 0.5 + 0.2;
                flake.style.animationDuration = (Math.random() * 10 + 10) + 's';
                flake.style.animationDelay = (Math.random() * 10) + 's';
                container.appendChild(flake);
            }
        }

        // Countdown
        function updateCountdown() {
            const now = new Date();
            let xmas = new Date(now.getFullYear(), 11, 25);
            if (now > xmas) xmas = new Date(now.getFullYear() + 1, 11, 25);
            
            const diff = xmas - now;
            const d = Math.floor(diff / (1000*60*60*24));
            const h = Math.floor((diff / (1000*60*60)) % 24);
            const m = Math.floor((diff / (1000*60)) % 60);
            const s = Math.floor((diff / 1000) % 60);

            document.getElementById('days').textContent = String(d).padStart(2, '0');
            document.getElementById('hours').textContent = String(h).padStart(2, '0');
            document.getElementById('minutes').textContent = String(m).padStart(2, '0');
            document.getElementById('seconds').textContent = String(s).padStart(2, '0');
        }

        // Calendar
        function renderCalendar() {
            const cal = document.getElementById('calendar');
            const now = new Date();
            const today = now.getDate();
            const month = now.getMonth();
            const firstDay = new Date(2024, 11, 1).getDay();
            const days = ['S','M','T','W','T','F','S'];
            
            let html = days.map(d => `<div class="cal-header">${d}</div>`).join('');
            for (let i = 0; i < firstDay; i++) html += '<div class="cal-day empty"></div>';
            for (let i = 1; i <= 31; i++) {
                let cls = 'cal-day';
                if (month === 11 && i === today) cls += ' today';
                if (i === 25) cls += ' christmas';
                html += `<div class="${cls}">${i}</div>`;
            }
            cal.innerHTML = html;
        }

        // Stats
        function updateStats() {
            const giftCount = state.gifts.length;
            const wrappedCount = state.gifts.filter(g => g.status === 'wrapped').length;
            const guestCount = state.guests.filter(g => g.rsvp === 'yes').length;
            const done = state.tasks.filter(t => t.done).length;
            const pct = state.tasks.length ? Math.round((done / state.tasks.length) * 100) : 0;
            
            document.getElementById('side-stat-gifts').textContent = giftCount;
            document.getElementById('side-stat-tasks').textContent = pct + '%';
            
            document.getElementById('nav-gifts-count').textContent = giftCount;
            document.getElementById('nav-guests-count').textContent = guestCount;
            document.getElementById('nav-tasks-count').textContent = done + '/' + state.tasks.length;
        }

        function updateDbStatus() {
            document.getElementById('db-gifts-count').textContent = state.gifts.length;
            document.getElementById('db-guests-count').textContent = state.guests.length;
            document.getElementById('db-menu-count').textContent = state.menu.length;
            document.getElementById('db-shopping-count').textContent = state.shopping.length;
            document.getElementById('db-events-count').textContent = state.events.length;
            document.getElementById('db-tasks-count').textContent = state.tasks.length;
        }

        // Budget
        function updateBudget() {
            const total = parseFloat(document.getElementById('budget-total').value) || 0;
            state.budget = total;
            const spent = state.gifts.reduce((s, g) => s + (parseFloat(g.price) || 0), 0);
            const pct = total > 0 ? Math.min((spent / total) * 100, 100) : 0;
            const remaining = total - spent;
            const over = remaining < 0;

            document.getElementById('budget-spent').textContent = '$' + spent;
            document.getElementById('budget-percent').textContent = pct.toFixed(0) + '% used';
            document.getElementById('budget-remaining').textContent = '$' + Math.abs(remaining) + (over ? ' over' : ' left');
            document.getElementById('budget-remaining').style.color = over ? 'var(--red)' : 'var(--text-secondary)';
            
            const bar = document.getElementById('budget-bar');
            bar.style.width = pct + '%';
            bar.className = 'progress-fill' + (over ? ' over' : '');
            saveState();
        }

        // Gifts
        function renderGifts() {
            const tbody = document.getElementById('gifts-body');
            tbody.innerHTML = state.gifts.map(g => `
                <tr>
                    <td><input value="${g.recipient}" onchange="updateGift(${g.id},'recipient',this.value)" placeholder="Name"></td>
                    <td><input value="${g.gift}" onchange="updateGift(${g.id},'gift',this.value)" placeholder="Gift idea"></td>
                    <td><input type="number" value="${g.price}" onchange="updateGift(${g.id},'price',this.value)" placeholder="0"></td>
                    <td>
                        <select onchange="updateGift(${g.id},'status',this.value)">
                            <option value="idea" ${g.status==='idea'?'selected':''}>💡 Idea</option>
                            <option value="bought" ${g.status==='bought'?'selected':''}>🛍️ Bought</option>
                            <option value="wrapped" ${g.status==='wrapped'?'selected':''}>🎁 Wrapped</option>
                        </select>
                    </td>
                    <td>
                        <select onchange="updateGift(${g.id},'priority',this.value)">
                            <option value="high" ${g.priority==='high'?'selected':''}>🔴 High</option>
                            <option value="medium" ${g.priority==='medium'?'selected':''}>🟡 Medium</option>
                            <option value="low" ${g.priority==='low'?'selected':''}>🟢 Low</option>
                        </select>
                    </td>
                    <td><span class="delete-btn" onclick="deleteGift(${g.id})">×</span></td>
                </tr>
            `).join('');
            updateStats(); updateBudget();
        }
        function addGift() { state.gifts.push({id:Date.now(),recipient:'',gift:'',price:0,status:'idea',priority:'medium'}); renderGifts(); saveState(); }
        function updateGift(id,f,v) { const g=state.gifts.find(x=>x.id===id); if(g){g[f]=f==='price'?parseFloat(v)||0:v; renderGifts(); saveState();} }
        function deleteGift(id) { state.gifts=state.gifts.filter(g=>g.id!==id); renderGifts(); saveState(); }

        // Guests
        function renderGuests() {
            const tbody = document.getElementById('guests-body');
            tbody.innerHTML = state.guests.map(g => `
                <tr>
                    <td><input value="${g.name}" onchange="updateGuest(${g.id},'name',this.value)" placeholder="Name"></td>
                    <td><input value="${g.relationship}" onchange="updateGuest(${g.id},'relationship',this.value)" placeholder="Family/Friend"></td>
                    <td><input value="${g.dietary}" onchange="updateGuest(${g.id},'dietary',this.value)" placeholder="None"></td>
                    <td>
                        <select onchange="updateGuest(${g.id},'rsvp',this.value)">
                            <option value="pending" ${g.rsvp==='pending'?'selected':''}>⏳ Pending</option>
                            <option value="yes" ${g.rsvp==='yes'?'selected':''}>✅ Yes</option>
                            <option value="no" ${g.rsvp==='no'?'selected':''}>❌ No</option>
                        </select>
                    </td>
                    <td><span class="delete-btn" onclick="deleteGuest(${g.id})">×</span></td>
                </tr>
            `).join('');
            updateStats();
        }
        function addGuest() { state.guests.push({id:Date.now(),name:'',relationship:'',dietary:'None',rsvp:'pending'}); renderGuests(); saveState(); }
        function updateGuest(id,f,v) { const g=state.guests.find(x=>x.id===id); if(g){g[f]=v; renderGuests(); saveState();} }
        function deleteGuest(id) { state.guests=state.guests.filter(g=>g.id!==id); renderGuests(); saveState(); }

        // Menu
        function renderMenu() {
            const tbody = document.getElementById('menu-body');
            tbody.innerHTML = state.menu.map(m => `
                <tr>
                    <td><input value="${m.dish}" onchange="updateMenu(${m.id},'dish',this.value)" placeholder="Dish name"></td>
                    <td>
                        <select onchange="updateMenu(${m.id},'category',this.value)">
                            <option value="appetizer" ${m.category==='appetizer'?'selected':''}>🥗 Appetizer</option>
                            <option value="main" ${m.category==='main'?'selected':''}>🍖 Main</option>
                            <option value="side" ${m.category==='side'?'selected':''}>🥔 Side</option>
                            <option value="dessert" ${m.category==='dessert'?'selected':''}>🍰 Dessert</option>
                            <option value="drink" ${m.category==='drink'?'selected':''}>🥤 Drink</option>
                        </select>
                    </td>
                    <td><input value="${m.assignedTo}" onchange="updateMenu(${m.id},'assignedTo',this.value)" placeholder="Who"></td>
                    <td>
                        <select onchange="updateMenu(${m.id},'status',this.value)">
                            <option value="planned" ${m.status==='planned'?'selected':''}>📝 Planned</option>
                            <option value="confirmed" ${m.status==='confirmed'?'selected':''}>✅ Confirmed</option>
                        </select>
                    </td>
                    <td><span class="delete-btn" onclick="deleteMenu(${m.id})">×</span></td>
                </tr>
            `).join('');
        }
        function addMenuItem() { state.menu.push({id:Date.now(),dish:'',category:'main',assignedTo:'',status:'planned'}); renderMenu(); saveState(); }
        function updateMenu(id,f,v) { const m=state.menu.find(x=>x.id===id); if(m){m[f]=v; renderMenu(); saveState();} }
        function deleteMenu(id) { state.menu=state.menu.filter(m=>m.id!==id); renderMenu(); saveState(); }

        // Shopping
        function renderShopping() {
            const tbody = document.getElementById('shopping-body');
            tbody.innerHTML = state.shopping.map(s => `
                <tr>
                    <td><div class="checkbox ${s.bought?'checked':''}" onclick="toggleShopping(${s.id})">${s.bought?'✓':''}</div></td>
                    <td><input value="${s.item}" onchange="updateShopping(${s.id},'item',this.value)" placeholder="Item" style="${s.bought?'text-decoration:line-through;opacity:0.5':''}"></td>
                    <td>
                        <select onchange="updateShopping(${s.id},'category',this.value)">
                            <option value="food" ${s.category==='food'?'selected':''}>🍎 Food</option>
                            <option value="decor" ${s.category==='decor'?'selected':''}>🎄 Decor</option>
                            <option value="supplies" ${s.category==='supplies'?'selected':''}>📦 Supplies</option>
                            <option value="gifts" ${s.category==='gifts'?'selected':''}>🎁 Gifts</option>
                        </select>
                    </td>
                    <td><input type="number" value="${s.qty}" onchange="updateShopping(${s.id},'qty',this.value)" min="1" style="width:50px"></td>
                    <td><input type="number" value="${s.price}" onchange="updateShopping(${s.id},'price',this.value)" min="0"></td>
                    <td><span class="delete-btn" onclick="deleteShopping(${s.id})">×</span></td>
                </tr>
            `).join('');
        }
        function addShoppingItem() { state.shopping.push({id:Date.now(),item:'',category:'food',qty:1,price:0,bought:false}); renderShopping(); saveState(); }
        function toggleShopping(id) { const s=state.shopping.find(x=>x.id===id); if(s){s.bought=!s.bought; renderShopping(); saveState();} }
        function updateShopping(id,f,v) { const s=state.shopping.find(x=>x.id===id); if(s){s[f]=['qty','price'].includes(f)?parseFloat(v)||0:v; renderShopping(); saveState();} }
        function deleteShopping(id) { state.shopping=state.shopping.filter(s=>s.id!==id); renderShopping(); saveState(); }

        // Events
        function renderEvents() {
            const tbody = document.getElementById('events-body');
            tbody.innerHTML = state.events.sort((a,b)=>new Date(a.date+' '+a.time)-new Date(b.date+' '+b.time)).map(e => `
                <tr>
                    <td><input type="date" value="${e.date}" onchange="updateEvent(${e.id},'date',this.value)"></td>
                    <td><input type="time" value="${e.time}" onchange="updateEvent(${e.id},'time',this.value)"></td>
                    <td><input value="${e.event}" onchange="updateEvent(${e.id},'event',this.value)" placeholder="Event"></td>
                    <td><input value="${e.location}" onchange="updateEvent(${e.id},'location',this.value)" placeholder="Location"></td>
                    <td><span class="delete-btn" onclick="deleteEvent(${e.id})">×</span></td>
                </tr>
            `).join('');
        }
        function addEvent() { state.events.push({id:Date.now(),date:'2024-12-25',time:'12:00',event:'',location:''}); renderEvents(); saveState(); }
        function updateEvent(id,f,v) { const e=state.events.find(x=>x.id===id); if(e){e[f]=v; renderEvents(); saveState();} }
        function deleteEvent(id) { state.events=state.events.filter(e=>e.id!==id); renderEvents(); saveState(); }

        // Tasks
        function renderTasks() {
            const container = document.getElementById('tasks-container');
            container.innerHTML = state.tasks.map(t => `
                <div class="task-item">
                    <div class="checkbox ${t.done?'checked':''}" onclick="toggleTask(${t.id})">${t.done?'✓':''}</div>
                    <span class="task-text ${t.done?'done':''}">${t.text}</span>
                    <span class="delete-btn" onclick="deleteTask(${t.id})">×</span>
                </div>
            `).join('');
            updateStats();
        }
        function addTask() { const txt=prompt('New task:'); if(txt?.trim()){state.tasks.push({id:Date.now(),text:txt.trim(),done:false}); renderTasks(); saveState();} }
        function toggleTask(id) { const t=state.tasks.find(x=>x.id===id); if(t){t.done=!t.done; renderTasks(); saveState();} }
        function deleteTask(id) { state.tasks=state.tasks.filter(t=>t.id!==id); renderTasks(); saveState(); }

        // Toast
        function showToast(message, type = 'success') {
            const container = document.getElementById('toast-container');
            const toast = document.createElement('div');
            toast.className = `toast ${type}`;
            toast.innerHTML = `<span>${message}</span>`;
            container.appendChild(toast);
            setTimeout(() => { toast.style.opacity = '0'; setTimeout(() => toast.remove(), 300); }, 3000);
        }

        // Export/Import
        function exportData() {
            try {
                const dataStr = JSON.stringify(state, null, 2);
                const blob = new Blob([dataStr], { type: 'application/json' });
                const url = URL.createObjectURL(blob);
                const a = document.createElement('a');
                a.href = url;
                a.download = `christmas-hq-${new Date().toISOString().split('T')[0]}.json`;
                document.body.appendChild(a);
                a.click();
                document.body.removeChild(a);
                URL.revokeObjectURL(url);
                showToast('📤 Data exported successfully!', 'success');
            } catch(e) {
                showToast('❌ Export failed', 'error');
            }
        }

        function importData() { document.getElementById('import-modal').classList.add('active'); }
        function closeImportModal() { document.getElementById('import-modal').classList.remove('active'); document.getElementById('import-textarea').value = ''; }
        
        function confirmImport() {
            try {
                const imported = JSON.parse(document.getElementById('import-textarea').value);
                if (!imported.gifts || !imported.guests || !imported.tasks) throw new Error('Invalid data');
                state = { ...state, ...imported };
                saveState();
                document.getElementById('budget-total').value = state.budget;
                renderGifts(); renderGuests(); renderMenu(); renderShopping(); renderEvents(); renderTasks();
                updateDbStatus();
                closeImportModal();
                showToast('📥 Data imported successfully!', 'success');
            } catch(e) {
                showToast('❌ Invalid JSON data', 'error');
            }
        }

        function resetData() {
            if(confirm('Reset all data? This cannot be undone.')) {
                localStorage.removeItem(STORAGE_KEY);
                showToast('🔄 All data reset!', 'info');
                setTimeout(() => location.reload(), 1000);
            }
        }

        // Navigation
        document.querySelectorAll('.nav-item[data-section]').forEach(item => {
            item.addEventListener('click', function(e) {
                document.querySelectorAll('.nav-item').forEach(i => i.classList.remove('active'));
                this.classList.add('active');
                const section = this.dataset.section;
                const el = document.getElementById(section);
                if (el) {
                    el.scrollIntoView({ behavior: 'smooth', block: 'start' });
                }
                // Close mobile sidebar
                document.getElementById('sidebar').classList.remove('open');
            });
        });

        document.getElementById('import-modal').addEventListener('click', (e) => {
            if (e.target.id === 'import-modal') closeImportModal();
        });

        // Cover Images - Christmas themed from Unsplash
        const coverImages = [
            'https://images.unsplash.com/photo-1512389142860-9c449e58a814?w=1600&q=80', // Christmas lights
            'https://images.unsplash.com/photo-1482517967863-00e15c9b44be?w=1600&q=80', // Snowy forest
            'https://images.unsplash.com/photo-1576919228236-a097c32a5cd4?w=1600&q=80', // Christmas decorations
            'https://images.unsplash.com/photo-1543589077-47d81606c1bf?w=1600&q=80', // Christmas tree
            'https://images.unsplash.com/photo-1513297887119-d46091b24bfa?w=1600&q=80', // Winter scene
            'https://images.unsplash.com/photo-1545622783-b3e021430fee?w=1600&q=80', // Cozy Christmas
            'https://images.unsplash.com/photo-1544982503-9f984c14501a?w=1600&q=80', // Gifts
            'https://images.unsplash.com/photo-1511895426328-dc8714191300?w=1600&q=80', // Holiday lights
        ];

        let currentCoverIndex = 0;
        let coverPosition = 40;

        function changeCover() {
            currentCoverIndex = (currentCoverIndex + 1) % coverImages.length;
            const coverEl = document.getElementById('cover-image');
            coverEl.style.opacity = '0';
            setTimeout(() => {
                coverEl.style.backgroundImage = `url('${coverImages[currentCoverIndex]}')`;
                coverEl.style.opacity = '1';
            }, 200);
            showToast('🖼️ Cover image changed!', 'success');
        }

        function repositionCover() {
            coverPosition = coverPosition === 40 ? 20 : coverPosition === 20 ? 60 : 40;
            document.getElementById('cover-image').style.backgroundPosition = `center ${coverPosition}%`;
            showToast('↕️ Cover repositioned!', 'info');
        }

        // Page Icons
        const pageIcons = ['🎄', '🎅', '🎁', '⛄', '❄️', '🦌', '🔔', '⭐', '🕯️', '🎿', '🧣', '☃️'];
        let currentIconIndex = 0;

        function changeIcon() {
            currentIconIndex = (currentIconIndex + 1) % pageIcons.length;
            const iconEl = document.getElementById('page-icon');
            iconEl.style.transform = 'scale(0.8)';
            setTimeout(() => {
                iconEl.textContent = pageIcons[currentIconIndex];
                iconEl.style.transform = 'scale(1)';
            }, 150);
            showToast('✨ Icon changed!', 'success');
        }

        // Init
        loadState();
        document.addEventListener('DOMContentLoaded', () => {
            document.getElementById('budget-total').value = state.budget;
            // Add transition for cover image opacity
            document.getElementById('cover-image').style.transition = 'opacity 0.3s ease, background-position 0.3s ease';
            createSnowfall();
            renderCalendar();
            renderGifts();
            renderGuests();
            renderMenu();
            renderShopping();
            renderEvents();
            renderTasks();
            updateCountdown();
            updateDbStatus();
            setInterval(updateCountdown, 1000);
            setTimeout(() => showToast('🎄 Welcome to Christmas HQ!', 'success'), 500);
        });
    </script>
</body>
</html>
