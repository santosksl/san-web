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
                    <li class="hover:text-orange-400 cursor-pointer duration-300 flex flex-col text-[12px] font-semibold items-center justify-center">
                        <MessageCircle />
                        <span>MENSAGENS</span>
                    </li>
                    <li class="hover:text-orange-400 cursor-pointer duration-300  flex flex-col text-[12px] font-semibold items-center justify-center">
                        <Users />
                        <span>GRUPOS</span>
                    </li>
                    <li class="hover:text-orange-400 cursor-pointer duration-300 flex flex-col text-[12px] font-semibold items-center justify-center">
                        <PhoneCall />
                        <span>LIGAÇÕES</span>
                    </li>
                </ul>
            </div>
        </div>
        
        <div>
            <MessagesList />
        </div>
    </div>
</section>