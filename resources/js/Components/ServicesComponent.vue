<template>
  <section class="services-block">
    <div class="wrapper">
      <div class="heading">
        <h1 class="large-heading">What's Included in Pay Platform</h1>
        <span class="label">
          Get <span class="feature-count">100+</span> features out of the box with Pay integrated per-transaction pricing.
        </span>
      </div>

      <div class="services">
        <ServiceItem v-for="(service, index) in services" :key="index" :icon="service.icon" :title="service.title">
          <ul class="service-item-features">
            <ServiceFeature v-for="(item, index) in service.features" :key="index" icon="checkmark-outline">
                {{ item }}
            </ServiceFeature>
          </ul>
        </ServiceItem>
      </div>
    </div>
  </section>
</template>

<script setup>
import ServiceItem from './ServiceItem.vue';
import ServiceFeature from './ServiceFeature.vue';

const services = [
    {
        title: 'Global payments with a single integration',
        icon: 'card-outline',
        features: [
            '120+ global currencies',
            'Global payment methods'
        ]
    },
    {
        title: '24x7 phone, chat and email support',
        icon: 'call-outline',
        features: [
            'Responsive customer support',
            'Multilingual assistance'
        ]
    },
    {
        title: 'Tools to build optimized checkout flows',
        icon: 'phone-portrait-outline',
        features: [
            'Embeddable checkout',
            'Custom UI toolkit'
        ]
    },
    {
        title: 'Fast, predictable payouts to your bank accounts',
        icon: 'cash-outline',
        features: [
            'control payout timing',
            'transparent payouts'
        ]
    },
    {
        title: 'Financial reconciliation and reporting',
        icon: 'bar-chart-outline',
        features: [
            'real-time reporting',
            'unified reporting'
        ]
    },
    {
        title: 'Developer platform and third-party integrations',
        icon: 'pie-chart-outline',
        features: [
            '100+ extentions',
            'developer dashboard'
        ]
    }
];


</script>

<style lang="scss" scoped></style>



