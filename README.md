# ArduinoUnityLab

не ну я пока хз



Assets/
├── Scripts/
│   ├── Core/
│   │   ├── ArduinoCore.cs          # Главное ядро (пины, таймеры)
│   │   ├── ArduinoPin.cs           # Класс пина (режим, состояние, ШИМ)
│   │   └── SimulationManager.cs    # Управление симуляцией (запуск/пауза)
│   │
│   ├── Components/
│   │   ├── BaseComponent.cs        # Базовый класс для всех компонентов
│   │   ├── LED.cs                  # Светодиод
│   │   ├── Resistor.cs             # Резистор
│   │   ├── Button.cs               # Кнопка
│   │   ├── Potentiometer.cs        # Потенциометр
│   │   └── ArduinoBoard.cs         # Сама плата Arduino (визуальный объект)
│   │
│   ├── Circuit/
│   │   ├── Wire.cs                 # Провод (линия между пинами)
│   │   ├── CircuitGraph.cs         # Граф соединений (узлы-рёбра)
│   │   └── ConnectionValidator.cs  # Проверка корректности соединений
│   │
│   ├── UI/
│   │   ├── InspectorPanel.cs       # Панель свойств (клик по компоненту)
│   │   ├── CodeEditor.cs           # Редактор кода (с подсветкой)
│   │   ├── ToolbarManager.cs       # Кнопки (Старт/Стоп/Пауза)
│   │   └── LabSelector.cs          # Выбор лабораторной работы
│   │
│   ├── LabWorks/
│   │   ├── LabWorkManager.cs       # Управление лабораторными работами
│   │   └── LabWorkData.cs          # Класс для хранения данных лабораторной
│   │
│   └── Data/
│       ├── ProjectSaver.cs         # Сохранение/загрузка проекта (JSON)
│       └── ComponentLibrary.cs     # База данных компонентов
│
├── Prefabs/
│   ├── Components/
│   │   ├── Arduino.prefab
│   │   ├── LED.prefab
│   │   ├── Resistor.prefab
│   │   ├── Button.prefab
│   │   ├── Potentiometer.prefab
│   │   └── Wire.prefab              # (опционально)
│   │
│   └── UI/
│       ├── InspectorPanel.prefab
│       ├── CodeEditorPanel.prefab
│       ├── Toolbar.prefab
│       └── LabSelectorPanel.prefab
│
├── Sprites/
│   └── Components/
│       ├── arduino_board.png
│       ├── led_off.png
│       ├── led_on.png
│       ├── resistor.png
│       ├── button.png
│       └── potentiometer.png
│
├── Scenes/
│   └── MainScene.unity
│
└── Resources/
    └── LabWorks/
        ├── L01_LED.json
        ├── L02_RunningLine.json
        ├── L03_PWM.json
        └── ...
