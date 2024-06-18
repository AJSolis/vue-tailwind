<template>
    <nav class="bg-zinc shadow">
        <div class="container mx-auto px-6 py-3">
            <div class="flex justify-center items-center">
                <div class="flex space-x-6">
                    <RouterLink to="/" class="text-gray-700 hover:text-blue-500">Home</RouterLink>
                    <RouterLink to="/about" class="text-gray-700 hover:text-blue-500">About</RouterLink>
                    <RouterLink to="/contact" class="text-gray-700 hover:text-blue-500">Contact Me</RouterLink>
                    <RouterLink to="/tailwind" class="text-gray-700 hover:text-blue-500">Vue Tailwind Projects</RouterLink>
                    <RouterLink to="/resume" class="text-gray-700 hover:text-blue-500">Resume</RouterLink>
                </div>
            </div>
        </div>
    </nav>
</template>