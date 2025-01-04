<script>
    const products = [
        { id: 1, name: 'Wireless Headphones', price: 99.99, category: 'Electronics', image: '/products/headset.webp', description: 'Sleek wireless headphones with excellent sound quality and comfort.' },
        { id: 2, name: 'Gaming Mouse', price: 49.99, category: 'Electronics', image: '/products/gaming-mouse.webp', description: 'Ergonomic gaming mouse with RGB lighting and programmable buttons.' },
        { id: 3, name: 'Coffee Maker', price: 79.99, category: 'Appliances', image: '/products/coffee-maker.webp', description: 'Compact coffee maker with a modern design and digital display.' },
        { id: 4, name: 'Yoga Mat', price: 29.99, category: 'Fitness', image: '/products/yoga-mat.webp', description: 'Purple yoga mat with a textured surface for better grip and comfort.' },
        { id: 5, name: 'Running Shoes', price: 119.99, category: 'Fitness', image: '/products/running-shoes.webp', description: 'Breathable running shoes with cushioned soles and stylish design.' },
        { id: 6, name: 'Desk Lamp', price: 39.99, category: 'Home Office', image: '/products/lamp.webp', description: 'Minimalist desk lamp with adjustable neck and modern aesthetic.' },
        { id: 7, name: 'Bluetooth Speaker', price: 89.99, category: 'Electronics', image: '/products/speaker.webp', description: 'Portable Bluetooth speaker with mesh design and high-quality sound.' },
        { id: 8, name: 'Vacuum Cleaner', price: 199.99, category: 'Appliances', image: '/products/odd-vacuum-cleaner.webp', description: 'Futuristic upright vacuum cleaner with a sleek and ergonomic design.' },
        { id: 9, name: 'Smartwatch', price: 149.99, category: 'Electronics', image: '/products/smartwatch.webp', description: 'Modern smartwatch with a sleek design and intuitive interface.' }
    ];
</script>

<div class="max-w-7xl flex flex-wrap justify-between m-auto gap-10 my-10 p-20">
    {#each products as product}
        <!-- Card -->
        <a class="group relative w-80 hover:scale-[102%] transition-all cursor-pointer" href="/">
            <img src={product.image} alt={product.description} class="object-cover rounded-t-md">

            <div class="pt-2">
                <div class="flex justify-between item-center">
                    <p class="font-medium bg-gradient-to-r from-red-500 via-orange-500  to-purple-500 bg-clip-text text-transparent">{product.name}</p>
                    <p class="font-bold">${product.price}</p>
                </div>

                <p class="font-light mt-2">{product.description}</p>
            </div>
        </a>
    {/each}
</div>