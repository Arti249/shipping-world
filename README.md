<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shipping World Tycoon</title>
    <style>
        body { 
            font-family: Arial, sans-serif; 
            background: url('https://upload.wikimedia.org/wikipedia/commons/thumb/5/5a/World_map_blank_without_borders.svg/1280px-World_map_blank_without_borders.svg.png') no-repeat center center fixed;
            background-size: cover;
            color: #0ff; 
            margin: 0; 
            padding: 20px; 
            position: relative;
        }
        .overlay {
            position: fixed;
            top: 0; left: 0; right: 0; bottom: 0;
            background: rgba(10, 20, 45, 0.78);
            z-index: -1;
        }
        .container { 
            max-width: 1200px; 
            margin: auto; 
            background: rgba(17, 34, 51, 0.95); 
            padding: 20px; 
            border-radius: 12px; 
            display: flex;
            gap: 20px;
        }
        .main { flex: 1; }
        .sidebar { width: 300px; background: rgba(34, 51, 68, 0.98); padding: 18px; border-radius: 10px; }
        h1 { color: #0f0; text-align: center; text-shadow: 0 0 12px #000; }
        button { 
            background: #0a5; color: white; padding: 12px 18px; margin: 5px; 
            border: none; border-radius: 6px; cursor: pointer; font-size: 16px; 
        }
        button:hover { background: #0f8; }
        .ship { 
            background: rgba(34, 51, 68, 0.95); 
            padding: 14px; margin: 10px 0; border-radius: 8px; cursor: pointer; 
        }
        .log { 
            height: 240px; overflow-y: scroll; background: rgba(0,0,0,0.9); 
            padding: 12px; border-radius: 6px; font-size: 14px; 
        }
        .port-marker {
            position: absolute;
            color: #ff0;
            font-size: 32px;
            text-shadow: 0 0 10px #f00;
            cursor: pointer;
            z-index: 100;
            transition: transform 0.2s;
        }
        .port-marker:hover { transform: scale
        
