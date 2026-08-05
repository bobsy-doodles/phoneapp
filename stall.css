  <style>
    /* Base page styling */
    body {
        display: flex;
        justify-content: center;
        align-items: center;
        min-height: 100vh;
        background-color: #f0f2f5;
        margin: 0;
        font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
        user-select: none;
    }

    /* The Phone Container */
    .smartphone {
        position: relative;
        width: 360px;
        height: 740px;
        background: #000;
        border-radius: 45px;
        box-shadow: 0px 25px 50px -12px rgba(0, 0, 0, 0.4);
        border: 12px solid #222;
        overflow: hidden;
        box-sizing: border-box;
    }

    /* Screen Notch */
    .notch {
        position: absolute;
        top: 15px;
        left: 50%;
        transform: translateX(-50%);
        width: 110px;
        height: 28px;
        background: #000;
        border-radius: 20px;
        z-index: 100;
    }

    .speaker {
        position: absolute;
        top: 4px;
        left: 50%;
        transform: translateX(-50%);
        width: 40px;
        height: 4px;
        background: #333;
        border-radius: 2px;
    }

    .camera {
        position: absolute;
        top: 9px;
        right: 15px;
        width: 10px;
        height: 10px;
        background: #111;
        border-radius: 50%;
    }

    /* Phone Screen Content Area */
    .screen {
        width: 100%;
        height: 100%;
        background: linear-gradient(135deg, #1e3c72 0%, #2a5298 100%);
        color: white;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        padding: 20px;
        box-sizing: border-box;
        position: relative;
    }

    /* Status Bar */
    .status-bar {
        display: flex;
        justify-content: space-between;
        align-items: center;
        font-size: 14px;
        font-weight: 600;
        margin-top: 12px;
        z-index: 90;
        color: #fff;
    }

    /* App Windows / Screens */
    .app-window {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: #fff;
        color: #000;
        z-index: 50;
        display: none;
        flex-direction: column;
        padding: 60px 20px 30px 20px;
        box-sizing: border-box;
        overflow: auto;
    }

    .app-window.active {
        display: flex;
    }

    /* Home Screen App Grid Layout */
    .app-grid {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        gap: 20px;
        padding: 40px 10px;
        flex-grow: 1;
        z-index: 10;
    }

    .app-icon {
        display: flex;
        flex-direction: column;
        align-items: center;
        cursor: pointer;
        transition: transform 0.2s;
    }

    .app-icon:hover {
        transform: scale(1.05);
    }

    .icon-shape {
        width: 55px;
        height: 55px;
        border-radius: 14px;
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 26px;
        box-shadow: 0 4px 6px rgba(0,0,0,0.1);
    }

    .app-label {
        font-size: 11px;
        margin-top: 6px;
        text-align: center;
        font-weight: 500;
        color: #fff;
        text-shadow: 0 1px 2px rgba(0,0,0,0.6);
    }

    /* App System Colors */
    .phone-bg { background: #4cd964; }
    .store-bg { background: #007aff; color: white; font-weight: bold; font-size: 22px; }
    .dynamic-bg { background: #ff9500; }

    /* DIALER INTERFACE */
    #dialer-app { background: #fff; color: #000; }
    .dial-display {
        font-size: 32px;
        text-align: center;
        margin: 20px 0;
        height: 40px;
        font-weight: 400;
        letter-spacing: 1px;
        overflow: hidden;
    }
    .keypad {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        gap: 15px;
        justify-items: center;
        margin-top: 10px;
    }
    .key {
        width: 65px;
        height: 65px;
        background: #e5e5ea;
        border-radius: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 24px;
        font-weight: 500;
        cursor: pointer;
    }
    .key:active { background: #d1d1d6; }
    .dial-actions {
        display: flex;
        justify-content: center;
        gap: 30px;
        margin-top: 25px;
        align-items: center;
    }
    .call-btn { background: #4cd964; color: white; width: 65px; height: 65px; border-radius: 50%; display: flex; justify-content: center; align-items: center; font-size: 24px; cursor: pointer; }
    .backspace-btn { font-size: 22px; cursor: pointer; color: #8e8e93; width: 40px; text-align: center; }

    /* APP STORE INTERFACE */
    #store-app { background: #f2f2f7; }
    .store-header { font-size: 28px; font-weight: 800; margin-bottom: 15px; }
    .store-item {
        background: #fff;
        padding: 12px;
        border-radius: 12px;
        display: flex;
        align-items: center;
        justify-content: space-between;
        margin-bottom: 12px;
        box-shadow: 0 1px 3px rgba(0,0,0,0.05);
    }
    .store-item-info { display: flex; align-items: center; gap: 12px; }
    .store-icon { width: 45px; height: 45px; border-radius: 10px; display: flex; justify-content: center; align-items: center; font-size: 22px; }
    .store-name { font-weight: 600; font-size: 15px; }
    .get-btn {
        background: #007aff;
        color: white;
        border: none;
        padding: 6px 14px;
        border-radius: 15px;
        font-weight: 600;
        font-size: 13px;
        cursor: pointer;
    }
    .get-btn.installed { background: #e5e5ea; color: #007aff; }

    /* Bottom Home Bar Indicator */
    .home-bar-container {
        position: absolute;
        bottom: 0;
        left: 0;
        width: 100%;
        height: 25px;
        z-index: 200;
        display: flex;
        justify-content: center;
        align-items: center;
        cursor: pointer;
    }
    .home-bar {
        width: 120px;
        height: 5px;
        background: rgba(255, 255, 255, 0.8);
        border-radius: 10px;
        transition: background 0.2s;
    }
    .dark-home-bar .home-bar {
        background: rgba(0, 0, 0, 0.5);
    }

    /* Additional small app styles */
    .app-content {
      flex: 1;
      display: flex;
      flex-direction: column;
      gap: 12px;
    }
    .center {
      display:flex;
      align-items:center;
      justify-content:center;
    }
    canvas { border-radius: 8px; background: white; touch-action: none; }
    .snake-canvas { background: #111; }
    .controls { display:flex; gap:8px; }
    .small-btn { padding:6px 10px; border-radius:8px; border:none; cursor:pointer; background:#007aff; color:white; font-weight:600; }
  </style>
