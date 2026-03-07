<template>

<section id="contact" class="py-20 bg-gray-100 dark:bg-gray-900 transition-colors duration-300">
    <div class="container mx-auto max-w-7xl px-6">
        <div class="bg-white dark:bg-gray-800 p-8 md:p-16 rounded-3xl shadow-2xl border border-gray-300 dark:border-gray-700 transition duration-300">
            <h2 class="text-3xl md:text-4xl font-bold text-center text-teal-600 dark:text-teal-400 mb-12">Get in Touch</h2>
            
            <div class="grid md:grid-cols-2 gap-12">
                <!-- Contact Info -->
                <div class="flex flex-col space-y-8">
                    <div class="flex items-start space-x-4">
                        <i class="fas fa-map-marker-alt text-2xl text-teal-600 dark:text-teal-400 flex-shrink-0"></i>
                        <div>
                            <p class="text-gray-800 dark:text-white font-semibold">Address</p>
                            <p class="text-gray-600 dark:text-gray-400">Khulna, Bangladesh</p>
                        </div>
                    </div>
                    <div class="flex items-start space-x-4">
                        <i class="fas fa-envelope text-2xl text-teal-600 dark:text-teal-400 flex-shrink-0"></i>
                        <div>
                            <p class="text-gray-800 dark:text-white font-semibold">Email</p>
                            <p class="text-gray-600 dark:text-gray-400">julfikariucs15@gmail.com</p>
                        </div>
                    </div>
                    <div class="flex items-start space-x-4">
                        <i class="fas fa-phone-alt text-2xl text-teal-600 dark:text-teal-400 flex-shrink-0"></i>
                        <div>
                            <p class="text-gray-800 dark:text-white font-semibold">Phone</p>
                            <p class="text-gray-600 dark:text-gray-400">+8801521459316</p>
                        </div>
                    </div>
                    <!-- Optional: Social Links -->
                    <div class="flex space-x-4 mt-4">
                        <a href="#" class="text-gray-600 dark:text-gray-400 hover:text-teal-600 dark:hover:text-teal-400 transition duration-300 text-2xl">
                            <i class="fab fa-linkedin"></i>
                        </a>
                        <a href="#" class="text-gray-600 dark:text-gray-400 hover:text-teal-600 dark:hover:text-teal-400 transition duration-300 text-2xl">
                            <i class="fab fa-github"></i>
                        </a>
                        <a href="#" class="text-gray-600 dark:text-gray-400 hover:text-teal-600 dark:hover:text-teal-400 transition duration-300 text-2xl">
                            <i class="fab fa-twitter"></i>
                        </a>
                    </div>
                </div>

                <!-- Contact Form -->
                <div>
                    <form action="#" method="POST" class="space-y-6">
                        <input type="text" name="name" placeholder="Your Name" class="w-full p-4 rounded-xl bg-gray-50 dark:bg-gray-700 text-gray-800 dark:text-white border border-gray-300 dark:border-gray-600 focus:outline-none focus:ring-2 focus:ring-teal-500 dark:focus:ring-teal-400 focus:border-teal-500 dark:focus:border-teal-400 transition duration-300 placeholder-gray-500 dark:placeholder-gray-400">
                        <input type="email" name="email" placeholder="Your Email" class="w-full p-4 rounded-xl bg-gray-50 dark:bg-gray-700 text-gray-800 dark:text-white border border-gray-300 dark:border-gray-600 focus:outline-none focus:ring-2 focus:ring-teal-500 dark:focus:ring-teal-400 focus:border-teal-500 dark:focus:border-teal-400 transition duration-300 placeholder-gray-500 dark:placeholder-gray-400">
                        <textarea name="message" rows="5" placeholder="Your Message" class="w-full p-4 rounded-xl bg-gray-50 dark:bg-gray-700 text-gray-800 dark:text-white border border-gray-300 dark:border-gray-600 focus:outline-none focus:ring-2 focus:ring-teal-500 dark:focus:ring-teal-400 focus:border-teal-500 dark:focus:border-teal-400 transition duration-300 placeholder-gray-500 dark:placeholder-gray-400"></textarea>
                        <button type="submit" class="bg-teal-600 hover:bg-teal-700 dark:bg-teal-500 dark:hover:bg-teal-600 text-white font-semibold py-3 px-8 rounded-full shadow-lg transition-colors duration-300 w-full md:w-auto cursor-pointer">Send Message</button>
                    </form>
                </div>
            </div>
        </div>
    </div>
</section>


</template>