<script>
    let faq1 = false;
    let faq2 = false;
    let faq3 = false;
    let faq4 = false;
    let faq5 = false;
    let faq6 = false;
</script>

<div id="accordion" class="bg-[#F1F6F0] md:px-0 px-4">
    <div class="container mx-auto md:pt-28 pt-24 md:pb-[13.44rem] pb-[11rem]">
        <div class="rounded-3xl bg-white shadow-[4px_4px_2px_2px_#000]">

            <div class="md:py-8 py-6 md:px-10 px-8 border-2 rounded-t-3xl border-solid border-black">
                <input type="checkbox" id="faq1" bind:checked={faq1} class="hidden" />
                <label for="faq1" class="cursor-pointer flex justify-between items-center md:text-lg text-sm gap-8 font-WorkSansSemiBold">
                    <span>Who is it meant for?</span>
                    <span>{faq1 ? '-' : '+'}</span>
                </label>
                {#if faq1}
                    <div class="max-h-0 overflow-hidden font-WorkSansRegular md:text-base text-xs text-gray-500 mt-4 transition-[max-height] duration-[3s] ease-[ease-out]" style="max-height: {faq1 ? '1000px' : '0'};">
                        <p>Django is a high-level web framework for Python that promotes rapid development and clean, pragmatic design. It follows the Model-View-Controller (MVC) architectural pattern, allowing developers to build robust web applications by emphasizing reusable code and a "don't repeat yourself" (DRY) philosophy. With its batteries-included approach, Django comes bundled with a variety of built-in features for tasks like authentication, URL routing, and database access.</p>
                    </div>
                {/if}
            </div>
            <div class="md:py-8 py-6 md:px-10 px-8 border-2 border-solid border-black">
                <input type="checkbox" id="faq2" bind:checked={faq2} class="hidden" />
                <label for="faq2" class="cursor-pointer flex justify-between items-center md:text-lg text-sm gap-8 font-WorkSansSemiBold">
                    <span>What is Hybrid State Of Mind? (HSoM)</span>
                    <span>{faq2 ? '-' : '+'}</span>
                </label>
                {#if faq2}
                    <div class="max-h-0 overflow-hidden font-WorkSansRegular md:text-base text-xs text-gray-500 mt-4 transition-[max-height] duration-[3s] ease-[ease-out]" style="max-height: {faq2 ? '1000px' : '0'};">
                        <p>One of Django's standout features is its Object-Relational Mapping (ORM) system, enabling developers to interact with databases using Python code instead of SQL queries. This abstraction simplifies database operations and supports multiple database backends. Django's built-in administrative interface, the Django Admin, also facilitates effortless management of database records during development.</p>
                    </div>
                {/if}
            </div>
            <div class="md:py-8 py-6 md:px-10 px-8 border-2 border-solid border-black">
                <input type="checkbox" id="faq3" bind:checked={faq3} class="hidden" />
                <label for="faq3" class="cursor-pointer flex justify-between items-center md:text-lg text-sm gap-8 font-WorkSansSemiBold">
                    <span>Is this community moderated? If yes, why?</span>
                    <span>{faq3 ? '-' : '+'}</span>
                </label>
                {#if faq3}
                    <div class="max-h-0 overflow-hidden font-WorkSansRegular md:text-base text-xs text-gray-500 mt-4 transition-[max-height] duration-[3s] ease-[ease-out]" style="max-height: {faq3 ? '1000px' : '0'};">
                        <p>Django incorporates a powerful templating engine that allows developers to create dynamic and data-driven HTML content. Views in Django handle user requests, processing data and interacting with models before rendering templates. This separation of concerns makes it easier to manage and maintain code, promoting a clean and scalable structure for web applications.</p>
                    </div>
                {/if}
            </div>
            <div class="md:py-8 py-6 md:px-10 px-8 border-2 border-solid border-black">
                <input type="checkbox" id="faq4" bind:checked={faq4} class="hidden" />
                <label for="faq4" class="cursor-pointer flex justify-between items-center md:text-lg text-sm gap-8 font-WorkSansSemiBold">
                    <span>I have already applied to HSoM. How long before I hear back?</span>
                    <span>{faq4 ? '-' : '+'}</span>
                </label>
                {#if faq4}
                    <div class="max-h-0 overflow-hidden font-WorkSansRegular md:text-base text-xs text-gray-500 mt-4 transition-[max-height] duration-[3s] ease-[ease-out]" style="max-height: {faq4 ? '1000px' : '0'};">
                        <p>Django places a strong emphasis on security, providing built-in tools to protect against common web vulnerabilities. It includes features like protection against Cross-Site Scripting (XSS) and Cross-Site Request Forgery (CSRF). Additionally, Django supports secure password hashing, making it a reliable choice for developing applications with stringent security requirements.</p>
                    </div>
                {/if}
            </div>
            <div class="md:py-8 py-6 md:px-10 px-8 border-2 border-solid border-black">
                <input type="checkbox" id="faq5" bind:checked={faq5} class="hidden" />
                <label for="faq5" class="cursor-pointer flex justify-between items-center md:text-lg text-sm gap-8 font-WorkSansSemiBold">
                    <span>Can I promote my services or products in any of the channels here?</span>
                    <span>{faq5 ? '-' : '+'}</span>
                </label>
                {#if faq5}
                    <div class="max-h-0 overflow-hidden font-WorkSansRegular md:text-base text-xs text-gray-500 mt-4 transition-[max-height] duration-[3s] ease-[ease-out]" style="max-height: {faq5 ? '1000px' : '0'};">
                        <p>Django benefits from a vibrant and active community of developers and contributors. This community-driven approach ensures continuous improvement, and the extensive documentation makes it easy for both beginners and experienced developers to grasp the framework's concepts and efficiently utilize its features.</p>
                    </div>
                {/if}
            </div>
            <div class="md:py-8 py-6 md:px-10 px-8 rounded-b-3xl border-2 border-solid border-black">
                <input type="checkbox" id="faq6" bind:checked={faq6} class="hidden" />
                <label for="faq6" class="cursor-pointer flex justify-between items-center md:text-lg text-sm gap-8 font-WorkSansSemiBold">
                    <span>If I want to add my friends or colleagues to this community?</span>
                    <span>{faq6 ? '-' : '+'}</span>
                </label>
                {#if faq6}
                    <div class="max-h-0 overflow-hidden font-WorkSansRegular md:text-base text-xs text-gray-500 mt-4 transition-[max-height] duration-[3s] ease-[ease-out]" style="max-height: {faq6 ? '1000px' : '0'};">
                        <p>Django is designed to scale with the growth of applications. It supports the development of modular and reusable components, facilitating extensibility. As project requirements evolve, Django's flexibility allows developers to integrate third-party packages and extend functionality while maintaining a coherent and maintainable codebase. This adaptability makes Django well-suited for projects of varying sizes and complexities.</p>
                    </div>
                {/if}
            </div>

        </div>
    </div>
  
</div>