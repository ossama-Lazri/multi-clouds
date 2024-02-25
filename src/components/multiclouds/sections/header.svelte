<script>
    import logo from '../../../assets/logo.svg'
    import vector1 from '../../../assets/vector1.svg'
    import vector2 from '../../../assets/vector2.svg'
    import vector3 from '../../../assets/vector3.svg'

    let isModalOpen = false
    const toggleModal = () => isModalOpen = !isModalOpen
    const submitMessage = () => alert('it works!')
</script>

<header id="header" class="md:min-h-screen bg-header w-full relative overflow-hidden">
    <!--Modal-->
        <div class="fixed h-screen inset-0 w-full bg-black bg-opacity-40 md:p-0 p-4 place-content-center z-[9999] {isModalOpen ? 'grid' : 'hidden'}">
            <div class="border shadow-[4px_4px_0px_0px_#000] rounded-2xl border-solid border-black bg-white md:px-[5.7rem] sm:px-8 px-4 md:pt-10 pt-7 md:pb-[4.75rem] pb-14 flex flex-col justify-center items-center relative">
                <button on:click={toggleModal} class="p-2 border shadow-[2px_2px_0px_0px_#000] rounded-[1.25rem] border-solid border-black absolute top-6 right-6 bg-white">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none"><path fill-rule="evenodd" clip-rule="evenodd" d="M13.414 12L17.707 7.70701C18.098 7.31601 18.098 6.68401 17.707 6.29301C17.316 5.90201 16.684 5.90201 16.293 6.29301L12 10.586L7.70701 6.29301C7.31601 5.90201 6.68401 5.90201 6.29301 6.29301C5.90201 6.68401 5.90201 7.31601 6.29301 7.70701L10.586 12L6.29301 16.293C5.90201 16.684 5.90201 17.316 6.29301 17.707C6.48801 17.902 6.74401 18 7.00001 18C7.25601 18 7.51201 17.902 7.70701 17.707L12 13.414L16.293 17.707C16.488 17.902 16.744 18 17 18C17.256 18 17.512 17.902 17.707 17.707C18.098 17.316 18.098 16.684 17.707 16.293L13.414 12Z" fill="black"/></svg>
                </button>
                <span class="text-black text-center text-2xl font-WorkSansSemiBold leading-9">Sign up</span>
                <p class="mt-4 text-black text-center md:text-base font-WorkSansRegular text-xs leading-6 md:mb-10 pb-7">Lorem ipsum dolor sit amet consectetur. </p>
                <form on:submit|preventDefault={submitMessage} class="w-full flex flex-col">
                    <div class="flex flex-col md:gap-6 gap-3 md:mb-12 mb-6">
                        <div>
                            <label for="name" class="text-black font-WorkSansSemiBold text-sm leading-5">Full name</label>
                            <input id="name" type="text" class="block w-full focus:shadow-[4px_4px_0px_0px_#000] border font-WorkSansSemiBold md:mt-2 border-solid border-black md:min-w-[36rem] md:py-4 py-2 md:px-6 px-3 md:text-base text-sm placeholder:text-[#8F9BB3] leading-6 outline-none" placeholder="Enter">
                        </div>
                        <div>
                            <label for="email" class="text-black font-WorkSansSemiBold text-sm leading-5">Email</label>
                            <input id="email" type="text" class="block w-full focus:shadow-[4px_4px_0px_0px_#000] border font-WorkSansSemiBold md:mt-2 border-solid border-black md:min-w-[36rem] md:py-4 py-2 md:px-6 px-3 md:text-base text-sm placeholder:text-[#8F9BB3] leading-6 outline-none" placeholder="example@mail.com">
                        </div>
                        <div>
                            <label for="password" class="text-black font-WorkSansSemiBold text-sm leading-5">Password</label>
                            <input id="password" type="text" class="block w-full focus:shadow-[4px_4px_0px_0px_#000] border font-WorkSansSemiBold md:mt-2 border-solid border-black md:min-w-[36rem] md:py-4 py-2 md:px-6 px-3 md:text-base text-sm placeholder:text-[#8F9BB3] leading-6 outline-none" placeholder="Enter">
                        </div>
                    </div>
                    <button type="submit" class="md:py-[0.88rem] py-2 md:px-8 px-4 text-black font-WorkSansMedium leading-5 border shadow-[4px_4px_0px_0px_#000] rounded-lg border-solid border-black bg-[#ceff1a] hover:shadow-[3px_3px_0px_0px_#000]">Sign up</button>
                </form>
            </div>
        </div>
    <!---->
    <div class="container mx-auto md:px-0 px-4">
        <nav class="flex justify-between items-center pt-[0.87rem]">
            <a href="#!"><img src="{logo}" alt="logo" class="md:w-full sm:w-3/4 w-4/5"></a>
            <div class="flex items-center md:gap-4 gap-2 whitespace-nowrap">
                <button on:click class="md:px-8 px-6 md:py-[0.875rem] py-[0.675rem] text-black md:text-base text-sm font-WorkSansMedium leading-5">Log in</button>
                <button on:click={toggleModal} class="md:px-8 px-6 md:py-[0.875rem] py-[0.675rem] text-black md:text-base text-sm font-WorkSansMedium leading-5 border shadow-[4px_4px_0px_0px_#000] hover:shadow-[3px_3px_0px_0px_#000] rounded-lg border-solid border-black bg-[#ceff1a]">Sign up</button>
            </div>
        </nav>
        <div class="my-44 text-center z-10 relative">
            <h1 class="text-[#49DBC8] md:mb-11 mb-6 font-TerminaBold [text-shadow:0px_8px_0px_#000] text-center md:text-8xl text-6xl font-bold leading-[normal]">MULTI CLOUDS</h1>
            <p class="text-black text-sm font-WorkSansRegular md:text-xl leading-7">Automate on-premises and multi cloud infrastructure from one point</p>
        </div>
    </div>
    <div class="">
        <img src="{vector1}" alt="vector" class="absolute sm:top-[13rem] top-72 md:right-[35rem] sm:right-[13rem] right-44 -z-0" >
        <img src="{vector2}" alt="vector" class="absolute top-[9.6rem] -z-0" >
        <img src="{vector3}" alt="vector" class="absolute md:top-[15rem] top-40 right-12 md:right-[10rem] -z-0" >
    </div>
</header>