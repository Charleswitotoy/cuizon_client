<template>
    <Header></Header>
</template>

<script setup>
import { ref } from 'vue'
import {
    Dialog,
    DialogPanel,
    Disclosure,
    DisclosureButton,
    DisclosurePanel,
    Menu,
    MenuButton,
    MenuItem,
    MenuItems,
    TransitionChild,
    TransitionRoot,
} from '@headlessui/vue'
import {
    Bars3Icon,
    Bars4Icon,
    BellIcon,
    CalendarIcon,
    ChartPieIcon,
    Cog6ToothIcon,
    DocumentDuplicateIcon,
    FolderIcon,
    UsersIcon,
    XMarkIcon,
} from '@heroicons/vue/24/outline'
import { ChevronRightIcon } from '@heroicons/vue/20/solid'
import { ChevronDownIcon, MagnifyingGlassIcon } from '@heroicons/vue/20/solid'

const navigation = [
    { name: 'Home', href: '/', icon: Bars4Icon, current: true },
    { name: 'About', href: '/about', icon: Bars4Icon, current: false },
    { name: 'Services', href: '/services', icon: Bars4Icon, current: false },
    { name: 'Contact', href: '/contact', icon: Bars4Icon, current: false },
    // {
    //     name: 'Teams',
    //     icon: UsersIcon,
    //     current: false,
    //     children: [
    //         { name: 'Engineering', href: '#' },
    //         { name: 'Human Resources', href: '#' },
    //         { name: 'Customer Success', href: '#' },
    //     ],
    // },
    // {
    //     name: 'Projects',
    //     icon: FolderIcon,
    //     current: false,
    //     children: [
    //         { name: 'GraphQL API', href: '#' },
    //         { name: 'iOS App', href: '#' },
    //         { name: 'Android App', href: '#' },
    //         { name: 'New Customer Portal', href: '#' },
    //     ],
    // },
    // { name: 'Calendar', href: '#', icon: CalendarIcon, current: false },
    // { name: 'Documents', href: '#', icon: DocumentDuplicateIcon, current: false },
    // { name: 'Reports', href: '#', icon: ChartPieIcon, current: false },
]
const teams = [
    { id: 1, name: 'Heroicons', href: '#', initial: 'H', current: true },
    { id: 2, name: 'Tailwind Labs', href: '#', initial: 'T', current: false },
    { id: 3, name: 'Workcation', href: '#', initial: 'W', current: false },
]
const userNavigation = [
    { name: 'Your profile', href: '#' },
    { name: 'Sign out', href: '#' },
]

const sidebarOpen = ref(false)
</script>