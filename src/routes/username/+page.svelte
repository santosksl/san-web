<script lang="ts">
    import MessagesList from "$lib/components/messages/messages-list.component.svelte";
import { MessageCircle, PhoneCall, Users } from "@lucide/svelte";
</script>

<section class="h-screen w-screen">
    <div class="w-[40vw] bg-neutral-200 h-full">
        <div class="flex mb-10">
            <div class="pl-5 pt-5">
                <img width="100" src="https://github.com/santosksl.png" alt="Avatar" class="rounded-full">
            </div>
    
            <div class="w-full">
                <ul class="text-sm flex items-center justify-between mt-10 px-10">
                    <li>
                        <MessageCircle />
                    </li>
                    <li>
                        <Users />
                    </li>
                    <li>
                        <PhoneCall />
                    </li>
                </ul>
            </div>
        </div>
        
        <div>
            <MessagesList />
        </div>
    </div>
</section>