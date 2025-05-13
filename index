<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Proyecto Final Análisis de decisiones</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
            background-color: #f5f5f5;
        }
        
        .header {
            text-align: center;
            margin-bottom: 30px;
            padding-bottom: 20px;
            border-bottom: 2px solid #3498db;
        }
        
        .authors {
            font-style: italic;
            color: #555;
            margin-bottom: 10px;
        }
        
        .title {
            font-size: 24px;
            font-weight: bold;
            color: #2c3e50;
        }
        
        .activity {
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            padding: 20px;
            margin-bottom: 30px;
        }
        
        .activity-title {
            font-size: 20px;
            color: #3498db;
            margin-bottom: 15px;
            padding-bottom: 10px;
            border-bottom: 1px solid #eee;
        }
        
        .data-table {
            width: 100%;
            border-collapse: collapse;
            margin: 15px 0;
        }
        
        .data-table th, .data-table td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: left;
        }
        
        .data-table th {
            background-color: #f2f2f2;
        }
        
        .data-table tr:nth-child(even) {
            background-color: #f9f9f9;
        }
        
        .chart-container {
            margin: 20px 0;
            height: 300px;
            background-color: #fff;
            border-radius: 8px;
            padding: 15px;
            box-shadow: 0 1px 3px rgba(0,0,0,0.1);
        }
        
        .highlight {
            background-color: #e3f2fd;
            padding: 2px 5px;
            border-radius: 3px;
        }
        
        .data-highlight {
            font-weight: bold;
            color: #e74c3c;
        }
        
        .category {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
            margin: 15px 0;
        }
        
        .category-item {
            background-color: #3498db;
            color: white;
            padding: 8px 15px;
            border-radius: 20px;
            font-size: 14px;
        }
        
        .tabs {
            display: flex;
            margin-bottom: 20px;
            border-bottom: 1px solid #ddd;
        }
        
        .tab {
            padding: 10px 20px;
            cursor: pointer;
            background-color: #f1f1f1;
            border: none;
            transition: 0.3s;
        }
        
        .tab:hover {
            background-color: #ddd;
        }
        
        .tab.active {
            background-color: #3498db;
            color: white;
        }
        
        .tab-content {
            display: none;
            animation: fadeEffect 1s;
        }
        
        @keyframes fadeEffect {
            from {opacity: 0;}
            to {opacity: 1;}
        }
        
        .gender-comparison {
            display: flex;
            justify-content: space-around;
            margin: 20px 0;
        }
        
        .gender-box {
            width: 45%;
            padding: 15px;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        
        .male {
            background-color: #d4e6f7;
            border-left: 5px solid #3498db;
        }
        
        .female {
            background-color: #f7d4e5;
            border-left: 5px solid #e91e63;
        }
        
        .age-bars {
            display: flex;
            flex-direction: column;
            gap: 5px;
            margin: 15px 0;
        }
        
        .age-bar {
            display: flex;
            align-items: center;
        }
        
        .age-label {
            width: 50px;
            font-weight: bold;
        }
        
        .bar {
            height: 20px;
            background-color: #3498db;
            margin-left: 10px;
            transition: width 0.5s;
        }
        
        .bmi-value {
            margin-left: 10px;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <div class="header">
        <div class="authors">
            Claudina Villanueva Rosado<br>
            Danna Pagaza Sandoval<br>
            Ana Sofía Moreno Santos
        </div>
        <div class="title">Proyecto Final Análisis de decisiones</div>
    </div>
    
    <div class="tabs">
        <button class="tab active" onclick="openTab(event, 'act1')">Actividad 1</button>
        <button class="tab" onclick="openTab(event, 'act2')">Actividad 2-3</button>
        <button class="tab" onclick="openTab(event, 'act5')">Actividad 5-6</button>
        <button class="tab" onclick="openTab(event, 'act7')">Actividad 7-8</button>
        <button class="tab" onclick="openTab(event, 'act9')">Actividad 9-10</button>
    </div>
    
    <div id="act1" class="tab-content" style="display: block;">
        <div class="activity">
            <div class="activity-title">Actividad 1A. Análisis IMC</div>
            <p>Análisis inicial del Índice de Masa Corporal en la población estudiada.</p>
        </div>
        
        <div class="activity">
            <div class="activity-title">Actividad 1B. Análisis IMC</div>
            <p>Continuación del análisis del Índice de Masa Corporal con enfoque en antecedentes de diabetes.</p>
            
            <h3>Total de personas con antecedentes de diabetes: <span class="data-highlight">1726</span></h3>
            
            <div class="category">
                <div class="category-item">Bajo peso</div>
                <div class="category-item">Normal</div>
                <div class="category-item">Obesidad I</div>
                <div class="category-item">Obesidad II</div>
                <div class="category-item">Obesidad III</div>
                <div class="category-item">Sobrepeso I</div>
                <div class="category-item">Sobrepeso II</div>
            </div>
            
            <table class="data-table">
                <tr>
                    <th>Clasificación IMC</th>
                    <th>Recuento</th>
                    <th>Porcentaje</th>
                </tr>
                <tr>
                    <td>Obesidad I</td>
                    <td>37Y</td>
                    <td>19.52%</td>
                </tr>
                <tr>
                    <td>Obesidad II</td>
                    <td>38</td>
                    <td>15.53%</td>
                </tr>
                <tr>
                    <td>Obesidad III</td>
                    <td>37Y</td>
                    <td>19.52%</td>
                </tr>
                <tr>
                    <td>Sobrepeso I</td>
                    <td>134</td>
                    <td>7.15%</td>
                </tr>
                <tr>
                    <td>Sobrepeso II</td>
                    <td>145</td>
                    <td>9.44%</td>
                </tr>
            </table>
        </div>
    </div>
    
    <div id="act2" class="tab-content">
        <div class="activity">
            <div class="activity-title">Actividad 2. Análisis columnas en DAX</div>
            <p>Análisis de datos utilizando expresiones de análisis de datos (DAX).</p>
        </div>
        
        <div class="activity">
            <div class="activity-title">Actividad 3. Análisis de medidas en DAX</div>
            
            <h3>Edad Promedio de pacientes con obesidad tipo I, tipo 2 y tipo 3: <span class="data-highlight">25.83</span></h3>
            
            <table class="data-table">
                <tr>
                    <th>Clasificación IMC</th>
                    <th>Edad Promedio</th>
                </tr>
                <tr>
                    <td>Obesidad I</td>
                    <td>25.87</td>
                </tr>
                <tr>
                    <td>Obesidad II</td>
                    <td>28.00</td>
                </tr>
                <tr>
                    <td>Obesidad III</td>
                    <td>23.04</td>
                </tr>
                <tr>
                    <td>Total</td>
                    <td>25.83</td>
                </tr>
            </table>
            
            <h3>Elementos influyentes clave - Segmentos principales</h3>
            <p>¿Qué influye en IMC para aumento?</p>
            <p>Cuando el promedio de IMC aumenta en EDAD es 24 - 32: <span class="data-highlight">6.78</span></p>
            
            <div class="chart-container">
                <p><strong>Promedio de IMC</strong></p>
                <p>De media, es más probable que IMC aumente cuando EDAD es 24 - 32 que de lo contrario.</p>
                <p>Promedio (elementos seleccionados excluidos): 27-99</p>
                
                <div class="age-bars">
                    <div class="age-bar">
                        <div class="age-label">22 o menos</div>
                        <div class="bar" style="width: 10%;"></div>
                        <div class="bmi-value">22</div>
                    </div>
                    <div class="age-bar">
                        <div class="age-label">22 - 24</div>
                        <div class="bar" style="width: 25%;"></div>
                        <div class="bmi-value">24</div>
                    </div>
                    <div class="age-bar">
                        <div class="age-label">24 - 32</div>
                        <div class="bar" style="width: 80%;"></div>
                        <div class="bmi-value">30</div>
                    </div>
                    <div class="age-bar">
                        <div class="age-label">32 - 36</div>
                        <div class="bar" style="width: 40%;"></div>
                        <div class="bmi-value">27</div>
                    </div>
                    <div class="age-bar">
                        <div class="age-label">más de 36</div>
                        <div class="bar" style="width: 15%;"></div>
                        <div class="bmi-value">22</div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    
    <div id="act5" class="tab-content">
        <div class="activity">
            <div class="activity-title">Actividad 5. Análisis con Inteligencia Artificial</div>
            
            <h3>Promedio de COMIDAS AL DIA por EDAD</h3>
            
            <table class="data-table">
                <tr>
                    <th>Edad</th>
                    <th>Comidas/día</th>
                    <th>Edad</th>
                    <th>Comidas/día</th>
                </tr>
                <tr>
                    <td>55</td>
                    <td>3.00</td>
                    <td>14</td>
                    <td>3.00</td>
                </tr>
                <tr>
                    <td>51</td>
                    <td>3.00</td>
                    <td>56</td>
                    <td>3.00</td>
                </tr>
                <tr>
                    <td>18</td>
                    <td>2.88</td>
                    <td>29</td>
                    <td>2.85</td>
                </tr>
                <tr>
                    <td>31</td>
                    <td>2.73</td>
                    <td>41</td>
                    <td>2.65</td>
                </tr>
                <tr>
                    <td>40</td>
                    <td>2.68</td>
                    <td>38</td>
                    <td>2.56</td>
                </tr>
                <tr>
                    <td>44</td>
                    <td>2.67</td>
                    <td>35</td>
                    <td>2.53</td>
                </tr>
                <tr>
                    <td>32</td>
                    <td>2.65</td>
                    <td>39</td>
                    <td>2.52</td>
                </tr>
                <tr>
                    <td>28</td>
                    <td>2.66</td>
                    <td>39</td>
                    <td>2.52</td>
                </tr>
            </table>
        </div>
        
        <div class="activity">
            <div class="activity-title">Actividad 6. Comidas promedio por edad</div>
            <p>Análisis continuo de la relación entre edad y cantidad de comidas diarias.</p>
        </div>
    </div>
    
    <div id="act7" class="tab-content">
        <div class="activity">
            <div class="activity-title">Actividad 7. IMC Promedio por actividad física</div>
            
            <h3>Promedio de IMC por ACTIVIDAD-Física</h3>
            
            <div class="chart-container">
                <p>Gráfico que muestra la relación entre el nivel de actividad física y el IMC promedio.</p>
                <!-- En una implementación real, aquí iría un gráfico generado con Chart.js o similar -->
                <div style="background-color: #eee; height: 200px; display: flex; justify-content: center; align-items: center;">
                    [Gráfico de IMC por nivel de actividad física]
                </div>
            </div>
        </div>
        
        <div class="activity">
            <div class="activity-title">Actividad 8. IMC Promedio dependiendo de si fuman o no</div>
            
            <h3>Promedio de IMC por FUMADOR</h3>
            
            <div class="chart-container">
                <p>Comparación del IMC promedio entre fumadores y no fumadores.</p>
                <!-- En una implementación real, aquí iría un gráfico generado con Chart.js o similar -->
                <div style="background-color: #eee; height: 200px; display: flex; justify-content: center; align-items: center;">
                    [Gráfico de IMC por condición de fumador]
                </div>
            </div>
        </div>
    </div>
    
    <div id="act9" class="tab-content">
        <div class="activity">
            <div class="activity-title">Actividad 9. IMC Promedio por edad en orden</div>
            
            <table class="data-table">
                <tr>
                    <th>EDAD</th>
                    <th>Promedio de IMC</th>
                </tr>
                <tr>
                    <td>17</td>
                    <td>21.44</td>
                </tr>
                <tr>
                    <td>16</td>
                    <td>21.56</td>
                </tr>
                <tr>
                    <td>51</td>
                    <td>23.37</td>
                </tr>
                <tr>
                    <td>61</td>
                    <td>24.24</td>
                </tr>
                <tr>
                    <td>14</td>
                    <td>24.62</td>
                </tr>
                <tr>
                    <td>19</td>
                    <td>25.47</td>
                </tr>
                <tr>
                    <td>18</td>
                    <td>25.64</td>
                </tr>
                <tr>
                    <td>20</td>
                    <td>26.22</td>
                </tr>
                <tr>
                    <td>35</td>
                    <td>27.70</td>
                </tr>
                <tr>
                    <td>48</td>
                    <td>27.86</td>
                </tr>
                <tr>
                    <td>55</td>
                    <td>27.96</td>
                </tr>
                <tr>
                    <td>56</td>
                    <td>28.09</td>
                </tr>
                <tr>
                    <td><strong>Total</strong></td>
                    <td><strong>29.70</strong></td>
                </tr>
            </table>
        </div>
        
        <div class="activity">
            <div class="activity-title">Actividad 10. IMC Promedio por clasificación y género</div>
            
            <h3>Promedio de IMC por ClasificaciónIMC y GENERO</h3>
            
            <div class="gender-comparison">
                <div class="gender-box male">
                    <h4>Hombres</h4>
                    <ul>
                        <li>Bajo peso: 17.31</li>
                        <li>Normal: 22.28</li>
                        <li>Sobrepeso I: 26.29</li>
                        <li>Sobrepeso II: 26.45</li>
                        <li>Obesidad I: 32.70</li>
                        <li>Obesidad II: 49.47</li>
                        <li>Obesidad III: 36.85</li>
                    </ul>
                </div>
                
                <div class="gender-box female">
                    <h4>Mujeres</h4>
                    <ul>
                        <li>Bajo peso: 17.33</li>
                        <li>Normal: 21.93</li>
                        <li>Sobrepeso I: 26.15</li>
                        <li>Sobrepeso II: 28.54</li>
                        <li>Obesidad I: 34.83</li>
                        <li>Obesidad II: 38.60</li>
                        <li>Obesidad III: 31.83</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
    
    <script>
        function openTab(evt, tabName) {
            var i, tabcontent, tablinks;
            
            // Oculta todos los contenidos de pestañas
            tabcontent = document.getElementsByClassName("tab-content");
            for (i = 0; i < tabcontent.length; i++) {
                tabcontent[i].style.display = "none";
            }
            
            // Elimina la clase "active" de todos los botones de pestaña
            tablinks = document.getElementsByClassName("tab");
            for (i = 0; i < tablinks.length; i++) {
                tablinks[i].className = tablinks[i].className.replace(" active", "");
            }
            
            // Muestra la pestaña actual y agrega la clase "active" al botón que abrió la pestaña
            document.getElementById(tabName).style.display = "block";
            evt.currentTarget.className += " active";
        }
        
        // Simular datos para gráficos (en una implementación real usarías una biblioteca como Chart.js)
        document.addEventListener('DOMContentLoaded', function() {
            // Podrías inicializar gráficos reales aquí
            console.log("Página cargada - aquí se inicializarían los gráficos");
        });
    </script>
</body>
</html>
