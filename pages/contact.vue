<template>
    <Content>
        <Container>
            <H1>Contact</H1>
            <div class="prose">
                <p>
                    Looking to get your piano tuned or repaired? Have an old
                    guitar lying around you want fixed?
                </p>
                <h4>Pricing</h4>
                <p>
                    At Brink's Piano Works our prices are non negotiable, and
                    subject to change, based on many factors including the
                    condition of one's piano.
                </p>
                <p>
                    We also charge per km, outside of my area. The price is
                    firm, to drop the cost, line up more pianos so the travel
                    bill can be split between more people.
                </p>
            </div>
            <form class="mt-10" netlify netlify-honeypot="bot-field">
                <div class="hidden">
                    <label
                        >Don’t fill this out if you're human:
                        <input name="bot-field"
                    /></label>
                </div>
                <div class="mb-6">
                    <label class="font-bold text-sm block mb-1" for="name"
                        >Name<span class="text-red-600">*</span></label
                    >
                    <input
                        placeholder="Full name"
                        id="name"
                        name="name"
                        class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
                        required
                    />
                </div>
                <div class="mb-6">
                    <label class="font-bold text-sm block mb-1" for="email"
                        >Email Address<span class="text-red-600">*</span></label
                    >
                    <input
                        placeholder="Email address"
                        id="email"
                        name="email"
                        type="email"
                        class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
                        required
                    />
                </div>
                <div class="mb-6">
                    <label class="font-bold text-sm block mb-1" for="address"
                        >Physical Address</label
                    >
                    <input
                        placeholder="12345 123 Street, Grande Prairie, AB"
                        id="address"
                        name="address"
                        type="text"
                        class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
                    />
                </div>
                <div class="mb-6">
                    <label class="font-bold text-sm block mb-1" for="message"
                        >Message<span class="text-red-600">*</span></label
                    >
                    <textarea
                        placeholder="Enter message"
                        id="message"
                        name="message"
                        class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
                        required
                    ></textarea>
                </div>
                <div class="mb-6">
                    <label class="inline-flex items-center">
                        <input
                            type="checkbox"
                            class="form-checkbox h-4 w-4"
                            name="piano_tuned_regularly"
                            value="yes"
                        /><span class="font-bold text-sm block ml-2"
                            >Has your piano been tuned regularly?</span
                        >
                    </label>
                </div>
                <div class="mb-6">
                    <label class="inline-flex items-center">
                        <input
                            type="checkbox"
                            class="form-checkbox h-4 w-4"
                            name="piano_keys_need_repair"
                            value="yes"
                        /><span class="font-bold text-sm block ml-2"
                            >Do any of your piano keys require repair?</span
                        >
                    </label>
                </div>
                <div class="mb-6">
                    <label class="inline-flex items-center">
                        <input
                            type="checkbox"
                            class="form-checkbox h-4 w-4"
                            name="piano_requires_repair"
                            value="yes"
                        /><span class="font-bold text-sm block ml-2"
                            >Does your piano require any repair?</span
                        >
                    </label>
                </div>
                <div class="mb-6">
                    <label class="inline-flex items-center">
                        <input
                            type="checkbox"
                            class="form-checkbox h-4 w-4"
                            name="piano_keys_feel_weird"
                            value="yes"
                        /><span class="font-bold text-sm block ml-2"
                            >Do any of your piano's keys feel weird?</span
                        >
                    </label>
                </div>
                <div class="mb-6">
                    <label class="font-bold text-sm block mb-1" for="brand"
                        >What is your piano's brand?</label
                    >
                    <input
                        placeholder="Piano brand"
                        id="brand"
                        name="brand"
                        type="text"
                        class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
                    />
                </div>
                <div class="mb-6">
                    <label class="font-bold text-sm block mb-1" for="tunedLast"
                        >When was your piano tuned last?</label
                    >
                    <input
                        placeholder=""
                        id="tunedLast"
                        name="brand"
                        type="date"
                        class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
                    />
                </div>
                <div class="mb-6">
                    <label class="font-bold text-sm block mb-1"
                        >Upright or Grand Piano?</label
                    >
                    <label class="font-bold text-sm mr-4">
                        <input
                            type="radio"
                            class="form-radio h-4 w-4"
                            name="piano_type"
                            value="upright"
                        />
                        Upright
                    </label>
                    <label class="font-bold text-sm mr-4">
                        <input
                            type="radio"
                            class="form-radio h-4 w-4"
                            name="piano_type"
                            value="upright"
                        />
                        Grand
                    </label>
                </div>

                <div class="mb-6">
                    <button
                        type="submit"
                        class="mr-5 bg-black hover:bg-gray-700 text-white font-bold py-2 px-4 rounded font-serif"
                    >
                        Submit
                    </button>
                </div>
            </form>
        </Container>
    </Content>
</template>

<script>
export default {};
</script>
