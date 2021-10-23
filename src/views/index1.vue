<script>
import Navbar from '@/components/navbar';
import Service from '@/components/services';
import Features from '@/components/features';
import Pricing from '@/components/pricing';
import Blog from '@/components/blog';
import Contact from '@/components/contact';
import Footer from '@/components/footer';
import Hero from '@/components/hero';

/**
 * Index-1
 */
export default {
    components: { Navbar, Service, Features, Pricing, Blog, Contact, Footer, Hero },
};
</script>
<template>
    <div>
        <Navbar />
        <div v-scroll-spy>
            <Hero />
            <Service />
            <Features />
            <Pricing />
            <Blog />
            <Contact />
            <Footer />
        </div>
    </div>
</template>
