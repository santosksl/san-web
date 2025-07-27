<script lang="ts">
    import MessagesList from "$lib/components/messages/messages-list.component.svelte";
    import { MessageCircle, PhoneCall, Video, Users } from "@lucide/svelte";
</script>

<section class="flex h-screen w-screen">
    <div class="w-[55vw] bg-neutral-200 h-full">
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
    
    <div class="w-full h-full flex flex-col">
        <div class="flex items-center justify-between px-5 pt-3">
            <div>
                <img src="https://github.com/El-Spacex.png" class="rounded-full" width="80" alt="">
            </div>

            <div class="pl-5">
                <p>Você esta conversando com <strong>spacex</strong></p>
            </div>
            
            <div>
                <ul class="flex items-center gap-x-5">
                    <li class="hover:text-orange-400 cursor-pointer duration-300">
                        <PhoneCall />
                    </li>

                    <li class="hover:text-orange-400 cursor-pointer duration-300">
                        <Video />
                    </li>
                </ul>
            </div>
        </div>

        <div class="flex-1 overflow-y-auto">
            <div class="flex mt-8 pl-5">
                <div>
                    <img src="https://github.com/El-Spacex.png" class="rounded-full" width="50" alt="">
                </div>
    
                <div>
                    <p class="pl-3">spacex</p>
                    <p class="text-sm pl-3">Eu sou uma pessoa homossexual e adoro queimar o caneco.</p>
                </div>
            </div>
        </div>

        <div>
            <input type="text" placeholder="Insira sua mensagem" class="outline-none border border-neutral-300 w-full h-[40px] text-sm pl-3">
        </div>
    </div>
</section>