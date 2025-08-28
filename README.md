<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Joel Castillo y Ashly Aguilar y Kimel Hernandez</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;700&display=swap');
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f7fafc;
        }
        .header-bg {
            background-image: url('https://placehold.co/1200x400/805ad5/ffffff?text=Bienvenidos+a+nuestras+recetas');
            background-size: cover;
            background-position: center;
            position: relative;
        }
        .header-bg::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.5);
        }
        .recipe-card {
            background-color: #ffffff;
            border-radius: 1.5rem;
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s ease-in-out, box-shadow 0.3s ease-in-out;
            border-left: 8px solid #667eea;
        }
        .recipe-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
        }
        .recipe-title {
            color: #4a5568;
        }
        .ingredient-list li, .instruction-list li {
            position: relative;
            padding-left: 1.5rem;
        }
        .ingredient-list li::before {
            content: '🥕';
            position: absolute;
            left: 0;
            top: 0;
        }
        .instruction-list li::before {
            content: '➡️';
            position: absolute;
            left: 0;
            top: 0;
        }
        .animated-emoji {
            animation: bounce-in 1s ease-out forwards;
        }
        @keyframes bounce-in {
            0% { transform: scale(0); opacity: 0; }
            50% { transform: scale(1.2); opacity: 1; }
            100% { transform: scale(1); }
        }
        .cartoon-image {
            animation: pulse 2s infinite ease-in-out;
        }
        @keyframes pulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.05); }
        }
    </style>
</head>
<body class="bg-gray-100 text-gray-800">

    <!-- Header Section -->
    <header class="header-bg relative flex items-center justify-center h-96 rounded-b-3xl overflow-hidden">
        <div class="relative z-10 text-center p-4">
            <h1 class="text-5xl md:text-7xl font-bold text-white mb-4 drop-shadow-lg">
                <span class="animated-emoji">👨‍🍳</span> Joel Castillo  y kimel Hernadez <span class="text-pink-300">&</span> Ashly Aguilar <span class="animated-emoji">👩‍🍳</span>
            </h1>
            <p class="text-xl md:text-2xl text-white drop-shadow-md">
                ¡Nuestras recetas secretas, de nuestra cocina a tu corazón!
            </p>
        </div>
    </header>

    <!-- Main Content -->
    <main class="container mx-auto p-4 md:p-8">

        <!-- Recipe Section: Ensalada Fresca -->
        
        <section class="my-10">
            <div class="recipe-card p-6 md:p-8 flex flex-col lg:flex-row items-center space-y-6 lg:space-y-0 lg:space-x-8">
                <div class="flex-1">
                    <h2 class="text-3xl font-bold recipe-title mb-4">Ensalada Fresca 🥗</h2>
                    
                    <img src="ensalada.jpg" alt="Ensalada Fresca" class="rounded-xl w-full cartoon-image mb-4">
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Ingredientes:</h3>
                    <ul class="list-disc pl-6 space-y-1 text-lg ingredient-list">
                        <li>2 manzanas de gala</li>
                        <li>¼ de cebolla morada</li>
                        <li>½ taza de elotes amarillos</li>
                        <li>1 pepino</li>
                        <li>½ zanahoria</li>
                        <li>1 onza de maní</li>
                        <li>4 hojas de lechuga (palmito o romana)</li>
                        <li>2 limones</li>
                        <li>2 tazas de agua</li>
                        <li>Aderezo italiano</li>
                    </ul>
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Tips o recomendaciones:</h3>
                    <ul class="list-disc pl-6 space-y-1 text-lg">
                        <li>Personalízalo: Si no te gusta un ingrediente, siéntete libre de omitirlo o sustituirlo.</li>
                        <li>Aderezo casero: Para un toque aún más personal, utiliza tu propio aderezo italiano hecho con aceite de oliva, vinagre balsámico, ajo, hierbas y miel para dulzor.</li>
                        <li>Decoración: Coloca la ensalada en un plato bonito y adorna con hojas de menta fresca.</li>
                    </ul>
                </div>
            </div>
        </section>

        <!-- Recipe Section: Ensalada de Frutas -->
        <section class="my-10">
            <div class="recipe-card p-6 md:p-8 flex flex-col lg:flex-row items-center space-y-6 lg:space-y-0 lg:space-x-8">
                <div class="flex-1">
                    <h2 class="text-3xl font-bold recipe-title mb-4">Ensalada de Frutas 🍓🥝</h2>
                    <img src="ensalada de frutas.jpg" alt="Ensalada de Frutas" class="rounded-xl w-full cartoon-image mb-4">
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Ingredientes:</h3>
                    <ul class="list-disc pl-6 space-y-1 text-lg ingredient-list">
                        <li>1 manzana de gala</li>
                        <li>2 kiwis</li>
                        <li>10 fresas</li>
                        <li>1 naranja</li>
                        <li>2 rodajas de piña</li>
                        <li>6 hojas de menta</li>
                        <li>1 limón</li>
                        <li>Vinagreta dulce: El jugo de 2 naranjas, ½ de miel de abeja, 1 cucharada de vino blanco</li>
                    </ul>
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Instrucciones:</h3>
                    <ol class="list-decimal pl-6 space-y-2 text-lg instruction-list">
                        <li>Preparación de la fruta: Lava, pela y corta todas las frutas en cubos o trozos. Lava las hojas de menta.</li>
                        <li>Preparación de la vinagreta: En un recipiente, exprime el jugo de las naranjas, agrega la miel y el vino blanco. Mezcla bien.</li>
                        <li>Ensamblaje de la ensalada: En un bowl grande, coloca las frutas cortadas y las hojas de menta picadas. Vierte la vinagreta y mezcla.</li>
                        <li>Servir: Sirve de inmediato o refrigera por un par de minutos.</li>
                    </ol>
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Consejos adicionales:</h3>
                    <ul class="list-disc pl-6 space-y-1 text-lg">
                        <li>Personaliza tu ensalada: Añade frutas de temporada como uvas, mango o melón.</li>
                        <li>Cambia el nivel de dulzura: Si quieres más dulce, pon más miel. Para más ácido, añade más jugo de naranja o limón.</li>
                        <li>Decoración: Puedes cubrir la ensalada con yogur natural, granola o semillas.</li>
                    </ul>
                </div>
            </div>
        </section>

        <!-- Recipe Section: Emparedado de Baguette -->
        <section class="my-10">
            <div class="recipe-card p-6 md:p-8 flex flex-col lg:flex-row items-center space-y-6 lg:space-y-0 lg:space-x-8">
                <div class="flex-1">
                    <h2 class="text-3xl font-bold recipe-title mb-4">Emparedado de Baguette 🥖</h2>
                    <img src="baguet.jpg" alt="Emparedado de Baguette" class="rounded-xl w-full cartoon-image mb-4">
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Ingredientes:</h3>
                    <ul class="list-disc pl-6 space-y-1 text-lg ingredient-list">
                        <li>3 rebanadas de baguette</li>
                        <li>3 hojas de lechuga romana o palmito</li>
                        <li>½ libra de lomo de res o angelina</li>
                        <li>4 lascas de queso mozzarella</li>
                        <li>Pimienta y sal al gusto</li>
                        <li>4 lascas de jamón</li>
                        <li>1 cebolla morada (corte juliana)</li>
                        <li>1 cucharada de mantequilla</li>
                        <li>½ taza de jugo de naranja</li>
                        <li>2 cucharadas de azúcar</li>
                        <li>Para el aderezo: ½ taza de mayonesa, ¼ de pepino, 1/4 de taza de mostaza, Romero deshidratado</li>
                    </ul>
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Procedimiento:</h3>
                    <ol class="list-decimal pl-6 space-y-2 text-lg instruction-list">
                        <li>Prepara el aderezo: Licúa mayonesa, pepino, mostaza y romero. Reserva.</li>
                        <li>Cocina la carne: Sofríe el lomo de res con mantequilla, sal y pimienta.</li>
                        <li>Prepara la cebolla caramelizada: Sofríe la cebolla morada con mantequilla y azúcar. Añade jugo de naranja y cocina a fuego bajo hasta que caramelice.</li>
                        <li>Arma el emparedado: Tuesta la baguette. Unta aderezo en una rebanada. Agrega lechuga, lomo, queso, jamón, cebolla y más aderezo. Cubre con otra rebanada.</li>
                    </ol>
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Sugerencias adicionales:</h3>
                    <ul class="list-disc pl-6 space-y-1 text-lg">
                        <li>Cambios: Puedes probar con tomate, aguacate o huevo frito.</li>
                        <li>Pan: Usa pan de molde o ciabatta si no tienes baguette.</li>
                        <li>Carne: Reemplaza el lomo con pollo, pavo o tofu.</li>
                        <li>Aderezo: El yogur griego natural es una buena alternativa a la mayonesa.</li>
                    </ul>
                </div>
            </div>
        </section>

        <!-- Recipe Section: Ensalada César -->
        <section class="my-10">
            <div class="recipe-card p-6 md:p-8 flex flex-col lg:flex-row items-center space-y-6 lg:space-y-0 lg:space-x-8">
                <div class="flex-1">
                    <h2 class="text-3xl font-bold recipe-title mb-4">Ensalada César 🐔</h2>
                    <img src="ensalada cesar.jpg" alt="Ensalada César" class="rounded-xl w-full cartoon-image mb-4">
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Ingredientes para la ensalada:</h3>
                    <ul class="list-disc pl-6 space-y-1 text-lg ingredient-list">
                        <li>½ lechuga romana (o palmito)</li>
                        <li>2 tomates</li>
                        <li>3 cucharadas de queso parmesano rallado</li>
                    </ul>
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Para marinar el pollo:</h3>
                    <ul class="list-disc pl-6 space-y-1 text-lg ingredient-list">
                        <li>Pechuga de pollo deshuesada</li>
                        <li>1 ½ cucharada de paprika</li>
                        <li>2 ramitas de romero</li>
                        <li>Sal y pimienta al gusto</li>
                        <li>1 dado de aceite de oliva</li>
                    </ul>
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Procedimiento:</h3>
                    <ol class="list-decimal pl-6 space-y-2 text-lg instruction-list">
                        <li>Marinar y cocinar el pollo: Mezcla el pollo en cubos con paprika, romero, sal, pimienta y aceite. Cocina en una sartén.</li>
                        <li>Armar la ensalada: En un bowl, combina la lechuga, los tomates y el queso parmesano. Añade el pollo desmenuzado.</li>
                    </ol>
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Crotones e Ingredientes para el Aderezo:</h3>
                    <ul class="list-disc pl-6 space-y-1 text-lg ingredient-list">
                        <li>Medio pan baguette, aceite de oliva, mantequilla, ajo, sazón completa.</li>
                        <li>Aderezo: Yema de huevo, anchoas (opcional), mostaza, queso parmesano, ajo, aceite de oliva, pimienta.</li>
                    </ul>
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Procedimiento adicional:</h3>
                    <ol class="list-decimal pl-6 space-y-2 text-lg instruction-list">
                        <li>Prepara los crotones: Corta el pan en cubos, mezcla con aceite, mantequilla, sazón y ajo. Hornea.</li>
                        <li>Prepara el aderezo: En un bowl, mezcla la yema, mostaza, ajo, limón, queso y anchoas. Bate mientras agregas el aceite de oliva.</li>
                        <li>Montaje: Coloca una cama de lechuga, tomates cherrys, pollo, crotones y queso parmesano.</li>
                    </ol>
                </div>
            </div>
        </section>

        <!-- Recipe Section: Fondos -->
        <section class="my-10">
            <div class="recipe-card p-6 md:p-8 flex flex-col lg:flex-row items-center space-y-6 lg:space-y-0 lg:space-x-8">
                <div class="flex-1">
                    <h2 class="text-3xl font-bold recipe-title mb-4">Fondos (Claro y Oscuro) 🥣</h2>
                    <img src="fondo.jpg" alt="Fondo Claro y Oscuro" class="rounded-xl w-full cartoon-image mb-4">
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Fondo Claro:</h3>
                    <p class="text-lg">Ingredientes: 1lb de menudos de pollo, ½ de chile verde, ½ de cebolla, ½ litro de agua, 1 hoja de laurel, hierbas aromáticas.</p>
                    <p class="text-lg mt-2">Procedimiento: Lavar los huesos, hervir, espumar, colar. Para clarificar, mezclar claras de huevo con carne molida y vegetales. Calentar con el caldo base y colar cuidadosamente.</p>
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Fondo Oscuro:</h3>
                    <p class="text-lg">Ingredientes: 1lb de huesos de res, ½ de chile verde, ½ de cebolla, ½ litro de agua, 1 hoja de laurel, hierbas aromáticas.</p>
                    <p class="text-lg mt-2">Procedimiento: Tostar los huesos en el horno. Sofríe los vegetales en una olla. Desglasa la bandeja y agrega el líquido a la olla. Cocina los huesos y vegetales a fuego bajo por 4-6 horas. Cuela el fondo.</p>
                </div>
            </div>
        </section>

        <!-- Recipe Section: Vinagreta Clásica -->
        <section class="my-10">
            <div class="recipe-card p-6 md:p-8 flex flex-col lg:flex-row items-center space-y-6 lg:space-y-0 lg:space-x-8">
                <div class="flex-1">
                    <h2 class="text-3xl font-bold recipe-title mb-4">Vinagreta Clásica 🌿</h2>
                    <img src="vinagreta.jpg" alt="Vinagreta Clásica" class="rounded-xl w-full cartoon-image mb-4">
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Ingredientes:</h3>
                    <ul class="list-disc pl-6 space-y-1 text-lg ingredient-list">
                        <li>¼ de taza de aceite de oliva</li>
                        <li>¼ de taza de vinagre (balsámico, de vino o de manzana)</li>
                        <li>½ cucharadita de sal</li>
                        <li>⅛ cucharadita de pimienta</li>
                        <li>1 cdita de mostaza Dijon</li>
                        <li>1 cdita de miel de abeja</li>
                        <li>1 diente de ajo finamente picado</li>
                        <li>Opcional: orégano, romero, tomillo o albahaca</li>
                    </ul>
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Procedimiento:</h3>
                    <ol class="list-decimal pl-6 space-y-2 text-lg instruction-list">
                        <li>En un tazón, mezcla todos los ingredientes húmedos y secos.</li>
                        <li>Bate enérgicamente hasta emulsionar.</li>
                        <li>Ajusta el sabor a tu gusto.</li>
                    </ol>
                </div>
            </div>
        </section>

        <!-- Recipe Section: Salsa Bechamel y Derivada -->
        <section class="my-10">
            <div class="recipe-card p-6 md:p-8 flex flex-col lg:flex-row items-center space-y-6 lg:space-y-0 lg:space-x-8">
                <div class="flex-1">
                    <h2 class="text-3xl font-bold recipe-title mb-4">Salsa Bechamel y Derivada 🧀</h2>
                    <img src="salsa bechamel.jpg" alt="Salsa Bechamel" class="rounded-xl w-full cartoon-image mb-4">
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Ingredientes Bechamel:</h3>
                    <ul class="list-disc pl-6 space-y-1 text-lg ingredient-list">
                        <li>50 gramos de mantequilla</li>
                        <li>50 gramos de harina</li>
                        <li>600 ml de leche entera</li>
                        <li>Pizca de nuez moscada, sal y pimienta</li>
                    </ul>
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Procedimiento:</h3>
                    <ol class="list-decimal pl-6 space-y-2 text-lg instruction-list">
                        <li>En una olla, derrite la mantequilla y añade la harina para crear un roux.</li>
                        <li>Retira del fuego y agrega la leche poco a poco, batiendo.</li>
                        <li>Vuelve al fuego y cocina sin dejar de remover hasta que espese. Sazona.</li>
                    </ol>
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Salsa Derivada (Puerros o Hongos):</h3>
                    <p class="text-lg mt-2">Ingredientes: 2 tazas de fondo blanco, 2 puerros o ½ lata de hongos, 2 ajos, 2 cucharadas de mantequilla, 2 tazas de bechamel, sal, pimienta, 1 onza de vino blanco.</p>
                    <p class="text-lg mt-2">Procedimiento: Sofríe ajo, puerros/hongos en mantequilla. Añade vino, fondo blanco y bechamel. Cocina a fuego bajo hasta que se integre.</p>
                </div>
            </div>
        </section>

        <!-- Recipe Section: Salsa Tipo Italiana -->
        <section class="my-10">
            <div class="recipe-card p-6 md:p-8 flex flex-col lg:flex-row items-center space-y-6 lg:space-y-0 lg:space-x-8">
                <div class="flex-1">
                    <h2 class="text-3xl font-bold recipe-title mb-4">Salsa Tipo Italiana 🍝</h2>
                    <img src="salsa italiana.jpg" alt="Salsa Tipo Italiana" class="rounded-xl w-full cartoon-image mb-4">
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Ingredientes:</h3>
                    <ul class="list-disc pl-6 space-y-1 text-lg ingredient-list">
                        <li>½ taza de tomate o 15 tomates</li>
                        <li>3 tazas de fondo de res</li>
                        <li>1 cucharada de aceite</li>
                        <li>½ de carne molida</li>
                        <li>3 dientes de ajo</li>
                        <li>¼ de cebolla blanca</li>
                        <li>¼ de chile verde</li>
                        <li>1 cucharada de azúcar</li>
                        <li>Albahaca, orégano, tomillo</li>
                        <li>Sal y pimienta al gusto</li>
                        <li>¼ de taza de queso parmesano</li>
                    </ul>
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Procedimiento:</h3>
                    <ol class="list-decimal pl-6 space-y-2 text-lg instruction-list">
                        <li>Sofríe cebolla, chile verde y ajo en aceite.</li>
                        <li>Incorpora la carne molida y cocina hasta dorar.</li>
                        <li>Añade tomate y fondo de res. Cocina a fuego lento por 20 minutos.</li>
                        <li>Añade azúcar y hierbas. Sazona y mezcla con el queso parmesano.</li>
                    </ol>
                </div>
            </div>
        </section>

        <!-- Recipe Section: Pasta Fresca -->
        <section class="my-10">
            <div class="recipe-card p-6 md:p-8 flex flex-col lg:flex-row items-center space-y-6 lg:space-y-0 lg:space-x-8">
                <div class="flex-1">
                    <h2 class="text-3xl font-bold recipe-title mb-4">Pasta Fresca con Salsa Alfredo 🍝</h2>
                    <img src="pasta alfredo.jpg" alt="Pasta Fresca" class="rounded-xl w-full cartoon-image mb-4">
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Ingredientes Pasta:</h3>
                    <ul class="list-disc pl-6 space-y-1 text-lg ingredient-list">
                        <li>50 gramos de harina</li>
                        <li>5 huevos medianos</li>
                        <li>Pizca de sal</li>
                        <li>½ cdita de aceite vegetal</li>
                    </ul>
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Procedimiento:</h3>
                    <ol class="list-decimal pl-6 space-y-2 text-lg instruction-list">
                        <li>Forma un volcán con la harina. Agrega huevos, sal y aceite en el centro.</li>
                        <li>Amasa por 10-15 minutos hasta que esté suave. Deja reposar por 30 minutos.</li>
                        <li>Estira la masa y córtala en la forma deseada. Cocina en agua hirviendo por 2-3 minutos.</li>
                    </ol>
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Ingredientes Salsa Alfredo:</h3>
                    <ul class="list-disc pl-6 space-y-1 text-lg ingredient-list">
                        <li>4 onzas de tocino</li>
                        <li>1 pechuga de pollo</li>
                        <li>3 onzas de mozzarella</li>
                        <li>150 gramos de queso parmesano</li>
                        <li>Aceite de oliva, vino blanco, perejil, pimiento rojo, ajo, pimentón amarillo.</li>
                    </ul>
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Procedimiento:</h3>
                    <ol class="list-decimal pl-6 space-y-2 text-lg instruction-list">
                        <li>Fríe el tocino y el pollo en una sartén. Retira y reserva.</li>
                        <li>Sofríe pimientos y ajo en la misma sartén.</li>
                        <li>Añade vino blanco y deja que se evapore.</li>
                        <li>Agrega mozzarella y queso parmesano. Remueve hasta que se espese.</li>
                        <li>Incorpora perejil, tocino y mezcla con la pasta.</li>
                    </ol>
                </div>
            </div>
        </section>

        <!-- Recipe Section: Arroz Cantones -->
        <section class="my-10">
            <div class="recipe-card p-6 md:p-8 flex flex-col lg:flex-row items-center space-y-6 lg:space-y-0 lg:space-x-8">
                <div class="flex-1">
                    <h2 class="text-3xl font-bold recipe-title mb-4">Arroz Cantonés 🥡</h2>
                    <img src="arroz cantones.jpg" alt="Arroz Cantonés" class="rounded-xl w-full cartoon-image mb-4">
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Ingredientes:</h3>
                    <ul class="list-disc pl-6 space-y-1 text-lg ingredient-list">
                        <li>Para el arroz: 2 tazas de arroz blanco, aceite vegetal, ajo, sal, agua.</li>
                        <li>Para las proteínas: pechuga de pollo, nuca de cerdo, tocino, huevos.</li>
                        <li>Vegetales: cebollines, ajo, cebolla blanca, salsa de soya, aceite de ajonjolí, mantequilla.</li>
                    </ul>
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Procedimiento:</h3>
                    <ol class="list-decimal pl-6 space-y-2 text-lg instruction-list">
                        <li>Prepara el arroz: Lava el arroz, sofríelo con ajo y cocina según las instrucciones.</li>
                        <li>Prepara las proteínas: Fríe el pollo, el cerdo y el tocino por separado. Haz una tortilla fina con los huevos.</li>
                        <li>Arma el arroz: Sofríe los vegetales en un wok. Añade el arroz cocido, las proteínas y los huevos. Vierte la salsa de soya y el aceite de ajonjolí.</li>
                    </ol>
                </div>
            </div>
        </section>

        <!-- Recipe Section: Paella a la Valenciana -->
        <section class="my-10">
            <div class="recipe-card p-6 md:p-8 flex flex-col lg:flex-row items-center space-y-6 lg:space-y-0 lg:space-x-8">
                <div class="flex-1">
                    <h2 class="text-3xl font-bold recipe-title mb-4">Paella a la Valenciana 🥘</h2>
                    <img src="paella.jpg" alt="Paella a la Valenciana" class="rounded-xl w-full cartoon-image mb-4">
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Ingredientes:</h3>
                    <ul class="list-disc pl-6 space-y-1 text-lg ingredient-list">
                        <li>Proteínas: chorizos, lomo de cerdo, pollo, tocino.</li>
                        <li>Arroz: 2 tazas de arroz precocido.</li>
                        <li>Vegetales: guisantes, tomates, perejil, cebolla, alubias chinas, pimiento rojo, pimiento verde, limón.</li>
                        <li>Especias: romero, tomillo, laurel, sal, pimienta, ajo, azafrán.</li>
                    </ul>
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Procedimiento:</h3>
                    <ol class="list-decimal pl-6 space-y-2 text-lg instruction-list">
                        <li>Dora el tocino, el cerdo, el pollo y los chorizos. Retira y reserva.</li>
                        <li>Sofríe los vegetales en la paellera. Agrega los tomates, hierbas y especias.</li>
                        <li>Regresa las proteínas a la paellera. Añade guisantes, alubias y azafrán.</li>
                        <li>Vierte el arroz y cubre con caldo. Cocina sin revolver hasta que el líquido se absorba.</li>
                        <li>Deja reposar con los chorizos encima. Decora con perejil y limón.</li>
                    </ol>
                </div>
            </div>
        </section>

        <!-- Recipe Section: Chimichurri -->
        <section class="my-10">
            <div class="recipe-card p-6 md:p-8 flex flex-col lg:flex-row items-center space-y-6 lg:space-y-0 lg:space-x-8">
                <div class="flex-1">
                    <h2 class="text-3xl font-bold recipe-title mb-4">Chimichurri 🌶️</h2>
                    <img src="chimichurri.jpg" alt="Chimichurri" class="rounded-xl w-full cartoon-image mb-4">
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Ingredientes:</h3>
                    <ul class="list-disc pl-6 space-y-1 text-lg ingredient-list">
                        <li>6 dientes de ajo</li>
                        <li>1 taza de perejil picado</li>
                        <li>¼ de taza de aceite vegetal</li>
                        <li>1 taza de vinagre blanco o de vino</li>
                        <li>1 cucharada de mantequilla o aceite de oliva</li>
                        <li>½ pimiento rojo, ½ pimiento amarillo</li>
                        <li>Romero, orégano, cebollines, sal, pimienta, cilantro.</li>
                        <li>Papas cambray, pan baguette.</li>
                    </ul>
                    <h3 class="text-2xl font-semibold text-gray-700 mt-6 mb-2">Procedimiento:</h3>
                    <ol class="list-decimal pl-6 space-y-2 text-lg instruction-list">
                        <li>Combina todos los ingredientes picados y las especias en un tazón.</li>
                        <li>Añade el vinagre y los aceites. Sazona y deja reposar 30 minutos.</li>
                        <li>Cocina las papas cambray hasta que estén tiernas. Saltea en mantequilla con ajo y eneldo.</li>
                        <li>Corta y tuesta el pan baguette. Unta con mantequilla y ajo, y espolvorea con queso parmesano.</li>
                    </ol>
                </div>
            </div>
        </section>
        
        <!-- Coffee Section -->
        <section class="my-10">
            <div class="recipe-card p-6 md:p-8 flex flex-col lg:flex-row items-center space-y-6 lg:space-y-0 lg:space-x-8">
                <div class="flex-1">
                    <h2 class="text-3xl font-bold recipe-title mb-4">Recetas de Café ☕</h2>
                    <img src="cafes.png" alt="Recetas de Café" class="rounded-xl w-full cartoon-image mb-4">
                    <div class="grid md:grid-cols-2 gap-8 mt-6">
                        <!-- Cappuccino -->
                        <div>
                            <h3 class="text-2xl font-semibold text-gray-700 mb-2">Cappuccino</h3>
                            <p class="text-lg"><strong>Ingredientes:</strong> 1 taza de expreso, 1 taza de leche, cacao, canela.</p>
                            <p class="text-lg mt-2"><strong>Procedimiento:</strong> Prepara el expreso. Calienta y espuma la leche. Vierte la leche cremada sobre el café. Espolvorea cacao o canela.</p>
                        </div>
                        <!-- Café Bombón -->
                        <div>
                            <h3 class="text-2xl font-semibold text-gray-700 mb-2">Café Bombón</h3>
                            <p class="text-lg"><strong>Ingredientes:</strong> 2 tazas de café expreso, ½ taza de leche condensada.</p>
                            <p class="text-lg mt-2"><strong>Procedimiento:</strong> Vierte la leche condensada en una taza. Con cuidado, vierte el café expreso encima para crear dos capas. Sirve sin mezclar.</p>
                        </div>
                        <!-- Café Expreso -->
                        <div>
                            <h3 class="text-2xl font-semibold text-gray-700 mb-2">Café Expreso</h3>
                            <p class="text-lg"><strong>Ingredientes:</strong> 2 tazas de café molido, 1 taza de agua.</p>
                            <p class="text-lg mt-2"><strong>Procedimiento:</strong> Muele el café finamente. Compacta en el porta filtro y extrae el café con una máquina de expreso. El resultado debe ser un líquido concentrado con crema.</p>
                        </div>
                        <!-- Café Afogato -->
                        <div>
                            <h3 class="text-2xl font-semibold text-gray-700 mb-2">Café Afogato</h3>
                            <p class="text-lg"><strong>Ingredientes:</strong> 1 taza de café expreso o semi-expreso, 1 bola de helado de vainilla.</p>
                            <p class="text-lg mt-2"><strong>Procedimiento:</strong> Coloca el helado en una taza o vaso. Vierte el café caliente sobre el helado y sirve de inmediato.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Drinks Section -->
        <section class="my-10">
            <div class="recipe-card p-6 md:p-8 flex flex-col lg:flex-row items-center space-y-6 lg:space-y-0 lg:space-x-8">
                <div class="flex-1">
                    <h2 class="text-3xl font-bold recipe-title mb-4">Bebidas Refrescantes 🍹</h2>
                    <img src="bebidas.png" alt="Bebidas Refrescantes" class="rounded-xl w-full cartoon-image mb-4">
                    <div class="grid md:grid-cols-2 gap-8 mt-6">
                        <!-- Mimosa -->
                        <div>
                            <h3 class="text-2xl font-semibold text-gray-700 mb-2">Mimosa</h3>
                            <p class="text-lg"><strong>Ingredientes:</strong> ½ taza de jugo de naranja, ¼ de taza de espumante (Sprite o Fiesta), 2 cucharadas de granadina o jarabe de cereza, hielo.</p>
                            <p class="text-lg mt-2"><strong>Procedimiento:</strong> En una copa, vierte el jugo de naranja y la granadina. Vierte el espumante con cuidado para crear capas. Agrega hielo y sirve.</p>
                        </div>
                        <!-- Limonada con Pepino y Hierbabuena -->
                        <div>
                            <h3 class="text-2xl font-semibold text-gray-700 mb-2">Limonada con Pepino y Hierbabuena</h3>
                            <p class="text-lg"><strong>Ingredientes:</strong> 1 taza de limonada, 4 rodajas de pepino, 3 rodajas de hierbabuena, azúcar, hielo.</p>
                            <p class="text-lg mt-2"><strong>Procedimiento:</strong> En un vaso, presiona suavemente el pepino y la hierbabuena. Agrega azúcar y hielo. Vierte la limonada y remueve.</p>
                        </div>
                        <!-- Sangría -->
                        <div>
                            <h3 class="text-2xl font-semibold text-gray-700 mb-2">Sangría</h3>
                            <p class="text-lg"><strong>Ingredientes:</strong> ½ taza de jugo de naranja, ½ manzana, ⅓ taza de Sprite, ⅓ taza de jugo de uva.</p>
                            <p class="text-lg mt-2"><strong>Procedimiento:</strong> Mezcla la manzana, el jugo de naranja y el jugo de uva. Refrigera por 30 minutos. Justo antes de servir, añade el Sprite. Sirve con trozos de fruta.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

    </main>

    <!-- Footer Section -->
    <footer class="bg-gray-800 text-white p-4 text-center rounded-t-3xl">
        <p>&copy; 2025 Joel Castillo & Ashly Aguilar & Kimel Hernandez . Todas las recetas son nuestras. ¡Disfruta!</p>
    </footer>

</body>
</html>
