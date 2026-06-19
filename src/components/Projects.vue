<template>

     <!-- Projects Section (Updated Layout) -->
       <section id="projects" class="bg-gradient-to-br py-20 bg-gray-100 dark:from-gray-800 dark:to-gray-900 transition-colors duration-300">
    <div class="container mx-auto max-w-7xl px-6">
        <h2 class="text-3xl md:text-4xl font-bold text-center text-teal-500 dark:text-teal-400 mb-12">
            Personal Projects
        </h2>

          <!-- Project Card 4 - HRM SaaS -->
        <div class="bg-white dark:bg-gray-800 rounded-3xl shadow-2xl border border-gray-200 dark:border-gray-700 overflow-hidden mb-8 md:flex transform hover:-translate-y-2 transition-transform duration-300">
            <div class="md:w-1/2 p-8 md:p-12 order-2 md:order-1">
                <h3 class="text-2xl font-bold text-gray-900 dark:text-white mb-2">HRM (SaaS)</h3>
                <p class="text-gray-700 dark:text-gray-300 mb-6">
                    Developed a comprehensive SaaS-based Human Resource Management (HRM) platform that helps organizations manage their workforce, operations, and internal communication from a centralized dashboard. The system includes multiple HR modules such as staff management, attendance tracking, leave applications, training management, performance appraisal, reminders, document management, and calendar-based scheduling.
                </p>
                <p class="text-gray-700 dark:text-gray-300 mb-6">
                    The platform also provides subscription management, working eligibility tracking, enhanced DBS management, and automated notifications to streamline HR workflows. Administrators and managers can monitor employee activities, manage records, and automate communication through email alerts and reminders.
                </p>
                <p class="text-gray-700 dark:text-gray-300 mb-6">
                    The system is designed with a modern dashboard interface, modular sidebar navigation, and role-based access control to support scalable SaaS operations for multiple organizations.
                </p>
                <div class="flex flex-wrap gap-2 mb-6">
                    <span class="bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-300 py-1 px-3 rounded-full text-xs">Laravel</span>
                    <span class="bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-300 py-1 px-3 rounded-full text-xs">Vue.js</span>
                    <span class="bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-300 py-1 px-3 rounded-full text-xs">Inertia.js</span>
                    <span class="bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-300 py-1 px-3 rounded-full text-xs">Tailwind CSS</span>
                    <span class="bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-300 py-1 px-3 rounded-full text-xs">MySQL</span>
                </div>
                <div class="flex flex-col sm:flex-row space-y-3 sm:space-y-0 sm:space-x-4">
                    <a href="#" class="bg-teal-500 text-white font-semibold py-2 px-6 rounded-full text-sm hover:bg-teal-600 transition-colors duration-300 text-center">Live Site</a>
                    <a href="/project-details/hrm-saas" class="bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-300 font-semibold py-2 px-6 rounded-full text-sm hover:bg-gray-300 dark:hover:bg-gray-600 transition-colors duration-300 text-center">View Details</a>
                </div>
            </div>
            <div class="md:w-1/2 flex items-center justify-center p-4 order-1 md:order-2">
                <img src="/img/hrm_dashboard.png" alt="HRM SaaS Platform" class="rounded-2xl w-full h-100 object-fit">
            </div>
        </div>
        
        <!-- Project Card 1 -->
        <div class="bg-white dark:bg-gray-800 rounded-3xl shadow-2xl border border-gray-200 dark:border-gray-700 overflow-hidden mb-8 md:flex transform hover:-translate-y-2 transition-transform duration-300">
            <div class="md:w-1/2 flex items-center justify-center p-4">
                <img src="https://placehold.co/200x100/222222/a3e635?text=LMS" alt="LMS with Payment" class="rounded-2xl w-full h-60 object-cover">
            </div>
            <div class="md:w-1/2 p-8 md:p-12">
                <h3 class="text-2xl font-bold text-gray-900 dark:text-white mb-2">LMS with Payment</h3>
                <p class="text-gray-700 dark:text-gray-300 mb-6">
                    Developed a simple LMS featuring tutor and student logins, course browsing, and integration with PayPal and Stripe for course purchases.
                </p>
                <div class="flex flex-wrap gap-2 mb-6">
                    <span class="bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-300 py-1 px-3 rounded-full text-xs">Laravel</span>
                    <span class="bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-300 py-1 px-3 rounded-full text-xs">PHP</span>
                    <span class="bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-300 py-1 px-3 rounded-full text-xs">HTML</span>
                    <span class="bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-300 py-1 px-3 rounded-full text-xs">CSS</span>
                    <span class="bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-300 py-1 px-3 rounded-full text-xs">JavaScript</span>
                    <span class="bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-300 py-1 px-3 rounded-full text-xs">MySQL DB</span>
                </div>
                <div class="flex flex-col sm:flex-row space-y-3 sm:space-y-0 sm:space-x-4">
                    <a href="#" class="bg-teal-500 text-white font-semibold py-2 px-6 rounded-full text-sm hover:bg-teal-600 transition-colors duration-300 text-center">Live Site</a>
                    <a href="#" class="bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-300 font-semibold py-2 px-6 rounded-full text-sm hover:bg-gray-300 dark:hover:bg-gray-600 transition-colors duration-300 text-center">Source Code</a>
                </div>
            </div>
        </div>

        <!-- Project Card 2 -->
        <div class="bg-white dark:bg-gray-800 rounded-3xl shadow-2xl border border-gray-200 dark:border-gray-700 overflow-hidden mb-8 md:flex transform hover:-translate-y-2 transition-transform duration-300">
            <div class="md:w-1/2 p-8 md:p-12 order-2 md:order-1">
                <h3 class="text-2xl font-bold text-gray-900 dark:text-white mb-2">E-Commerce Web Application</h3>
                <p class="text-gray-700 dark:text-gray-300 mb-6">
                    An online shopping application where users can browse, search, and order products by brand or category after registration. Admin panel allows managing products, categories, brands, and orders.
                </p>
                <div class="flex flex-wrap gap-2 mb-6">
                    <span class="bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-300 py-1 px-3 rounded-full text-xs">HTML</span>
                    <span class="bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-300 py-1 px-3 rounded-full text-xs">CSS</span>
                    <span class="bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-300 py-1 px-3 rounded-full text-xs">Bootstrap</span>
                    <span class="bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-300 py-1 px-3 rounded-full text-xs">JavaScript</span>
                    <span class="bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-300 py-1 px-3 rounded-full text-xs">jQuery</span>
                    <span class="bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-300 py-1 px-3 rounded-full text-xs">Laravel</span>
                    <span class="bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-300 py-1 px-3 rounded-full text-xs">MySQL DB</span>
                </div>
                <div class="flex flex-col sm:flex-row space-y-3 sm:space-y-0 sm:space-x-4">
                    <a href="#" class="bg-teal-500 text-white font-semibold py-2 px-6 rounded-full text-sm hover:bg-teal-600 transition-colors duration-300 text-center">Live Site</a>
                    <a href="#" class="bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-300 font-semibold py-2 px-6 rounded-full text-sm hover:bg-gray-300 dark:hover:bg-gray-600 transition-colors duration-300 text-center">Source Code</a>
                </div>
            </div>
            <div class="md:w-1/2 flex items-center justify-center p-4 order-1 md:order-2">
                <img src="https://placehold.co/300x200/222222/a3e635?text=E-Commerce" alt="E-Commerce Web Application" class="rounded-2xl w-full h-60 object-cover">
            </div>
        </div>

        <!-- Project Card 3 -->
        <div class="bg-white dark:bg-gray-800 rounded-3xl shadow-2xl border border-gray-200 dark:border-gray-700 overflow-hidden mb-8 md:flex transform hover:-translate-y-2 transition-transform duration-300">
            <div class="md:w-1/2 flex items-center justify-center p-4">
                <img src="https://placehold.co/600x400/222222/a3e635?text=Helpdesk" alt="Helpdesk Tracking System" class="rounded-2xl w-full h-60 object-cover">
            </div>
            <div class="md:w-1/2 p-8 md:p-12">
                <h3 class="text-2xl font-bold text-gray-900 dark:text-white mb-2">Helpdesk Tracking System</h3>
                <p class="text-gray-700 dark:text-gray-300 mb-6">
                    Analyzes the performance of users participating in contests across various online judges and evaluates the performance metrics, providing valuable insights into their achievements and progress.
                </p>
                <div class="flex flex-wrap gap-2 mb-6">
                    <span class="bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-300 py-1 px-3 rounded-full text-xs">Laravel</span>
                    <span class="bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-300 py-1 px-3 rounded-full text-xs">PHP</span>
                    <span class="bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-300 py-1 px-3 rounded-full text-xs">Bootstrap</span>
                    <span class="bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-300 py-1 px-3 rounded-full text-xs">REST API</span>
                </div>
                <div class="flex flex-col sm:flex-row space-y-3 sm:space-y-0 sm:space-x-4">
                    <a href="#" class="bg-teal-500 text-white font-semibold py-2 px-6 rounded-full text-sm hover:bg-teal-600 transition-colors duration-300 text-center">Live Site</a>
                    <a href="#" class="bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-300 font-semibold py-2 px-6 rounded-full text-sm hover:bg-gray-300 dark:hover:bg-gray-600 transition-colors duration-300 text-center">Source Code</a>
                </div>
            </div>
        </div>

      
    </div>
</section>

</template>