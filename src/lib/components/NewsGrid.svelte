<script>
  const articles = [
    {
      title: "The Future of Web3: Why European Founders Are Leading the Charge",
      author: "Heartcore Team",
      image: "/generated/image-close-up-of-hands-working-on-laptop-with-1766584733922-0.webp"
    },
    {
      title: "Founder NPS: The Metric That Matters Most in Venture Capital",
      author: "Investment Team",
      image: "/generated/image-european-startup-founder-in-deep-convers-1766584736573-1.webp"
    },
    {
      title: "Building for the Long Term: Our Concentrated Investment Approach",
      author: "Heartcore Capital",
      image: "/generated/image-diverse-tech-team-collaborating-around-w-1766584739346-2.webp"
    }
  ];
</script>

<section class="py-12 md:py-16 overflow-hidden">
  <div class="container mx-auto px-6 md:px-12 relative">
    <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
      {#each articles as article}
        <div class="group cursor-pointer">
          <div class="aspect-[16/10] overflow-hidden mb-6 bg-gray-100">
            <img 
              src={article.image} 
              alt={article.title}
              class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105"
            />
          </div>
          <h3 class="text-xl font-light text-gray-900 mb-3 leading-snug group-hover:text-gray-600 transition-colors">
            {article.title}
          </h3>
          <p class="text-xs text-gray-500 uppercase tracking-wide">by {article.author}</p>
        </div>
      {/each}
    </div>

    <!-- Navigation Arrow -->
    <div class="absolute top-1/2 -right-4 md:right-4 transform -translate-y-1/2 hidden md:block">
      <button class="w-12 h-12 flex items-center justify-center text-gray-400 hover:text-black transition-colors" aria-label="Next">
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M9 18L15 12L9 6" stroke="currentColor" stroke-width="1" stroke-linecap="round" stroke-linejoin="round"/>
        </svg>
      </button>
    </div>
  </div>
</section>
