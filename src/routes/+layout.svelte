<script>
  import Nav from "./common/Nav.svelte";
  import Contact from "./common/Contact.svelte";
  import Follow from "./common/Follow.svelte";
  import "../app.css";

  let { children } = $props();
</script>

<svelte:head>
  <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "Person",
      "name": "Ayo Kozlovskij",
      "jobTitle": "Certified Health Coach",
      "url": "https://www.ayoosteo.com",
      "sameAs": [
        "https://www.instagram.com/ayokozlovskij",
        "https://www.linkedin.com/in/ayo-oluade"
      ],
      "image": "https://www.ayoosteo.com/ayo-profile.png",
      "description": "London-based online health coach and osteopath supporting people with chronic illness, diabetes, migraines, low energy, and new health diagnoses.",
      "hasOfferCatalog": {
        "@type": "OfferCatalog",
        "name": "Health Services",
        "itemListElement": [
          {
            "@type": "Offer",
            "itemOffered": {
              "@type": "Service",
              "name": "Health Coaching",
              "serviceType": "Online Health Coaching",
              "areaServed": [
                {
                  "@type": "Place",
                  "name": "London"
                },
                {
                  "@type": "Country",
                  "name": "United Kingdom"
                }
              ],
              "availableChannel": {
                "@type": "ServiceChannel",
                "serviceLocation": {
                  "@type": "Place",
                  "name": "Online via Zoom or Facetime"
                }
              },
              "description": "Personalised health coaching to help with chronic illness, low energy, migraines, and creating sustainable habits. Delivered online with a focus on clients in London and the UK."
            }
          }
        ]
      }
    }
  </script>
</svelte:head>

<div id="app">
  <Nav />
  <main>{@render children()}</main>
  <Contact />
  <Follow />
</div>
