<template>
    <Content>
        <Container>
            <H1>Contact</H1>
            <div class="prose">
                <p>Looking to get your piano tuned or repaired? Have an old guitar lying around you want fixed?</p>
            </div>
            <form class="mt-10" netlify data-netlify-recaptcha="true">
                <div class="mb-6">
                    <label class="font-bold text-sm block mb-1" for="name">Name<span class="text-red-600">*</span></label>
                    <input placeholder="Full name" id="name" name="name" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" required />
                </div>
                <div class="mb-6">
                    <label class="font-bold text-sm block mb-1" for="email">Email Address<span class="text-red-600">*</span></label>
                    <input placeholder="Email address" id="email" name="email" type="email" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" required />
                </div>
                <div class="mb-6">
                    <label class="font-bold text-sm block mb-1" for="message">Message<span class="text-red-600">*</span></label>
                    <textarea placeholder="Enter message" id="message" name="message" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" required></textarea>
                </div>
                <div class="mb-6">
                    <div data-netlify-recaptcha="true"></div>
                </div>
                <div class="mb-6">
                    <button type="submit" class="mr-5 bg-black hover:bg-gray-700 text-white font-bold py-2 px-4 rounded font-serif">Submit</button>
                </div>
            </form>
        </Container>
    </Content>
</template>

<script>
    export default {
       
    }
</script>