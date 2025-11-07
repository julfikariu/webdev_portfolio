<template>

    <section id="contact" class="py-20 bg-gray-100 dark:bg-gray-900 transition-colors duration-300">
    <div class="container mx-auto max-w-7xl px-6">
        <div class="bg-gray-800 dark:bg-gray-800 p-8 md:p-16 rounded-3xl shadow-2xl border border-gray-700 dark:border-gray-700 transition duration-300">
            <h2 class="text-3xl md:text-4xl font-bold text-center text-teal-400 mb-12">Get in Touch</h2>
            
            <div class="grid md:grid-cols-2 gap-12">
                <!-- Contact Info -->
                <div class="flex flex-col space-y-8">
                    <div class="flex items-start space-x-4">
                        <i class="fas fa-map-marker-alt text-2xl text-teal-400 flex-shrink-0"></i>
                        <div>
                            <p class="text-white font-semibold">Address</p>
                            <p class="text-gray-400">Kushtia, Bangladesh</p>
                        </div>
                    </div>
                    <div class="flex items-start space-x-4">
                        <i class="fas fa-envelope text-2xl text-teal-400 flex-shrink-0"></i>
                        <div>
                            <p class="text-white font-semibold">Email</p>
                            <p class="text-gray-400">julfikariucs15@gmail.com</p>
                        </div>
                    </div>
                    <div class="flex items-start space-x-4">
                        <i class="fas fa-phone-alt text-2xl text-teal-400 flex-shrink-0"></i>
                        <div>
                            <p class="text-white font-semibold">Phone</p>
                            <p class="text-gray-400">+8801521459316</p>
                        </div>
                    </div>
                    <!-- Optional: Social Links -->
                    <div class="flex space-x-4 mt-4">
                        <a href="#" class="text-gray-400 hover:text-teal-400 transition duration-300 text-2xl">
                            <i class="fab fa-linkedin"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-teal-400 transition duration-300 text-2xl">
                            <i class="fab fa-github"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-teal-400 transition duration-300 text-2xl">
                            <i class="fab fa-twitter"></i>
                        </a>
                    </div>
                </div>

                <!-- Contact Form -->
                <div>
                    <form action="#" method="POST" class="space-y-6">
                        <input type="text" name="name" placeholder="Your Name" class="w-full p-4 rounded-xl bg-gray-700 dark:bg-gray-700 text-white border border-gray-600 dark:border-gray-600 focus:outline-none focus:ring-2 focus:ring-teal-400 focus:border-teal-400 transition duration-300">
                        <input type="email" name="email" placeholder="Your Email" class="w-full p-4 rounded-xl bg-gray-700 dark:bg-gray-700 text-white border border-gray-600 dark:border-gray-600 focus:outline-none focus:ring-2 focus:ring-teal-400 focus:border-teal-400 transition duration-300">
                        <textarea name="message" rows="5" placeholder="Your Message" class="w-full p-4 rounded-xl bg-gray-700 dark:bg-gray-700 text-white border border-gray-600 dark:border-gray-600 focus:outline-none focus:ring-2 focus:ring-teal-400 focus:border-teal-400 transition duration-300"></textarea>
                        <button type="submit" class="bg-teal-500 hover:bg-teal-600 text-white font-semibold py-3 px-8 rounded-full shadow-lg transition-colors duration-300 w-full md:w-auto">Send Message</button>
                    </form>
                </div>
            </div>
        </div>
    </div>
</section>


</template>