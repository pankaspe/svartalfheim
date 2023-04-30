<script lang="ts">
      import { Input, Label, Checkbox, Button, A, Heading, Hr } from 'flowbite-svelte';
</script>

<div class="flex justify-center">
    <div class="bg-white dark:bg-gray-700 md:w-4/6 w-full p-6 rounded-lg drop-shadow-md">
        <div>
            <Heading tag="h1" customSize="text-4xl font-extrabold  md:text-5xl lg:text-6xl">
                Edit profile
            </Heading>
        </div>
        <Hr class="my-8" height="h-px" />
        <form>
            <div class="grid gap-6 mb-6 md:grid-cols-2">
              <div>
                <Label for="first_name" class="mb-2">First name</Label>
                <Input type="text" id="first_name" placeholder="John" required  />
              </div>
              <div>
                <Label for="last_name" class="mb-2">Last name</Label>
                <Input type="text" id="last_name" placeholder="Doe" />
              </div>
              <div>
                <Label for="company" class="mb-2">Company</Label>
                <Input type="text" id="company" placeholder="Flowbite" />
              </div>
              <div>
                <Label for="phone" class="mb-2">Phone number</Label>
                <Input type="tel" id="phone" placeholder="123-45-678" pattern="[0-9]{3}-[0-9]{2}-[0-9]{3}" />
              </div>
              <div>
                <Label for="website" class="mb-2">Website URL</Label>
                <Input type="url" id="website" placeholder="flowbite.com" />
              </div>
              <div>
                <Label for="address" class="mb-2">Address</Label>
                <Input type="text" id="address" placeholder="your address" />
              </div>

            </div>
            <div class="mb-6">
              <Label for="email" class="mb-2">Email address</Label>
              <Input type="email" id="email" placeholder="john.doe@company.com" required />
            </div>
            <div class="mb-6">
              <Label for="password" class="mb-2">Password</Label>
              <Input type="password" id="password" placeholder="•••••••••" required />
            </div>
            <div class="mb-6">
              <Label for="confirm_password" class="mb-2">Confirm password</Label>
              <Input type="password" id="confirm_password" placeholder="•••••••••" required />
            </div>
            <Checkbox class="mb-6 space-x-1" required>I agree with the <A href="/">terms and conditions</A>.</Checkbox>
            <Button type="submit" color="yellow">Submit</Button>
          </form>
    </div>
  </div>