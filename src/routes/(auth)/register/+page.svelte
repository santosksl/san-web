<script lang="ts">
    import { Lock, Mail, User } from "@lucide/svelte";
</script>

<section class="flex items-center justify-center h-screen w-screen">
    <div>
        <div class="text-center">
            <h1 class="text-5xl font-extrabold text-orange-400">Registro</h1>
            <p>Seja muito bem vindo(a) a nossa plataforma, para continuar realize o seu registro.</p>
        </div>
        
        <div>
            <form action="" method="post" class="flex flex-col items-center justify-center">
                <div class="ml-8 flex flex-col">
                    <User size="20" class="text-orange-400 relative top-[50px] right-8"/>
                    <label for="username-input" class="text-sm font-semibold text-orange-400">Nome de usuario</label>
                    <input type="text" id="username-input" class="outline-none border border-neutral-300 w-[400px] h-[40px] text-sm pl-3">
                </div>

                <div class="ml-8 flex flex-col">
                    <Mail size="20" class="text-orange-400 relative top-[50px] right-8"/>
                    <label for="email-input" class="text-sm font-semibold text-orange-400">E-mail</label>
                    <input type="text" id="email-input" class="outline-none border border-neutral-300 w-[400px] h-[40px] text-sm pl-3">
                </div>

                <div class="ml-8 flex flex-col">
                    <Lock size="20" class="text-orange-400 relative top-[50px] right-8"/>
                    <label for="password-input" class="text-sm font-semibold text-orange-400">Senha</label>
                    <input type="text" id="password-input" class="outline-none border border-neutral-300 w-[400px] h-[40px] text-sm pl-3">
                </div>

                <div class="mt-5 ">
                    <button class="bg-orange-400 p-2 w-[435px] text-white hover:bg-orange-500 duration-300 cursor-pointer">
                        Registrar
                    </button>
                </div>
            </form>
        </div>
    </div>
</section>