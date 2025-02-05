<script setup>
import { Button } from '@/components/ui/button'
import { Card } from '@/components/ui/card'
import {
  Select,
  SelectContent,
  SelectGroup,
  SelectItem,
  SelectLabel,
  SelectTrigger,
  SelectValue,
} from '@/components/ui/select'
import { Avatar } from '@/components/ui/avatar'
import { Badge } from '@/components/ui/badge'
</script>

<template>
  <div class="min-h-screen bg-gradient-to-br from-gray-900 to-black text-white">
    <!-- Logo Section -->
    <div class="flex justify-center pt-8">
      <svg class="h-16 w-auto text-red-500" viewBox="0 0 62 65" fill="none" xmlns="http://www.w3.org/2000/svg">
        <!-- SVG path... -->
      </svg>
    </div>

    <!-- Main Content -->
    <div class="container mx-auto px-4 py-12">
      <div class="grid grid-cols-1 md:grid-cols-2 gap-8 max-w-6xl mx-auto">
        <!-- Left Section -->
        <div class="bg-gray-800/50 rounded-lg p-8">
          <h2 class="text-2xl md:text-3xl font-semibold mb-4 text-red-500">x</h2>
          <p class="text-lg md:text-xl text-gray-300 mb-6">
            -
          </p>
          <div class="flex justify-center">
            <Button class="bg-red-500 hover:bg-red-600 text-lg">Get Started</Button>
          </div>
        </div>

        <!-- Right Section -->
        <div class="space-y-6">
          <!-- Card 1 -->
         <Card class="bg-gray-800/50 rounded-lg p-6 border-blue-600">
            <Avatar />
         </Card>

         

          <!-- Card 2 -->
          <Card class="bg-gray-800/50 rounded-lg p-6 border-blue-600">
            <Badge variant="destructive">
                Test
            </Badge>
         </Card>

          <!-- Card 3 -->
          <Card class="bg-gray-800/50 rounded-lg p-6 border-blue-600">
            <Select>
                <SelectTrigger>
                <SelectValue placeholder="Select a fruit" />
                </SelectTrigger>
                <SelectContent>
                <SelectGroup>
                    <SelectLabel>Fruits</SelectLabel>
                    <SelectItem value="apple">
                    Apple
                    </SelectItem>
                </SelectGroup>
                </SelectContent>
            </Select>
         </Card>
        </div>
      </div>
    </div>
  </div>
</template>