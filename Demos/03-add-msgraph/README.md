# <a name="how-to-run-the-completed-project"></a><span data-ttu-id="13038-101">Como executar o projeto concluído</span><span class="sxs-lookup"><span data-stu-id="13038-101">How to run the completed project</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13038-102">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="13038-102">Prerequisites</span></span>

<span data-ttu-id="13038-103">Para executar o projeto concluído nessa pasta, você precisará do seguinte:</span><span class="sxs-lookup"><span data-stu-id="13038-103">To run the completed project in this folder, you need the following:</span></span>

- <span data-ttu-id="13038-104">[Node. js](https://nodejs.org) instalado em sua máquina de desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="13038-104">[Node.js](https://nodejs.org) installed on your development machine.</span></span> <span data-ttu-id="13038-105">Se você não tiver o Node. js, visite o link anterior para opções de download.</span><span class="sxs-lookup"><span data-stu-id="13038-105">If you do not have Node.js, visit the previous link for download options.</span></span> <span data-ttu-id="13038-106">(**Observação:** este tutorial foi escrito com o nó versão 10.7.0.</span><span class="sxs-lookup"><span data-stu-id="13038-106">(**Note:** This tutorial was written with Node version 10.7.0.</span></span> <span data-ttu-id="13038-107">As etapas deste guia podem funcionar com outras versões, mas que não foram testadas.</span><span class="sxs-lookup"><span data-stu-id="13038-107">The steps in this guide may work with other versions, but that has not been tested.)</span></span>
- <span data-ttu-id="13038-108">Uma conta pessoal da Microsoft com uma caixa de correio no Outlook.com ou uma conta corporativa ou de estudante da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="13038-108">Either a personal Microsoft account with a mailbox on Outlook.com, or a Microsoft work or school account.</span></span>

<span data-ttu-id="13038-109">Se você não tem uma conta da Microsoft, há algumas opções para obter uma conta gratuita:</span><span class="sxs-lookup"><span data-stu-id="13038-109">If you don't have a Microsoft account, there are a couple of options to get a free account:</span></span>

- <span data-ttu-id="13038-110">Você pode [se inscrever para uma nova conta pessoal da Microsoft](https://signup.live.com/signup?wa=wsignin1.0&rpsnv=12&ct=1454618383&rver=6.4.6456.0&wp=MBI_SSL_SHARED&wreply=https://mail.live.com/default.aspx&id=64855&cbcxt=mai&bk=1454618383&uiflavor=web&uaid=b213a65b4fdc484382b6622b3ecaa547&mkt=E-US&lc=1033&lic=1).</span><span class="sxs-lookup"><span data-stu-id="13038-110">You can [sign up for a new personal Microsoft account](https://signup.live.com/signup?wa=wsignin1.0&rpsnv=12&ct=1454618383&rver=6.4.6456.0&wp=MBI_SSL_SHARED&wreply=https://mail.live.com/default.aspx&id=64855&cbcxt=mai&bk=1454618383&uiflavor=web&uaid=b213a65b4fdc484382b6622b3ecaa547&mkt=E-US&lc=1033&lic=1).</span></span>
- <span data-ttu-id="13038-111">Você pode [se inscrever no programa para desenvolvedores do office 365](https://developer.microsoft.com/office/dev-program) para obter uma assinatura gratuita do Office 365.</span><span class="sxs-lookup"><span data-stu-id="13038-111">You can [sign up for the Office 365 Developer Program](https://developer.microsoft.com/office/dev-program) to get a free Office 365 subscription.</span></span>

## <a name="register-a-web-application-with-the-azure-active-directory-admin-center"></a><span data-ttu-id="13038-112">Registrar um aplicativo Web com o centro de administração do Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="13038-112">Register a web application with the Azure Active Directory admin center</span></span>

1. <span data-ttu-id="13038-113">Abra um navegador e navegue até o [centro de administração do Azure Active Directory](https://aad.portal.azure.com).</span><span class="sxs-lookup"><span data-stu-id="13038-113">Open a browser and navigate to the [Azure Active Directory admin center](https://aad.portal.azure.com).</span></span> <span data-ttu-id="13038-114">Faça logon usando uma **conta pessoal** (aka: conta da Microsoft) ou **conta corporativa ou de estudante**.</span><span class="sxs-lookup"><span data-stu-id="13038-114">Login using a **personal account** (aka: Microsoft Account) or **Work or School Account**.</span></span>

1. <span data-ttu-id="13038-115">Selecione **Azure Active Directory** na navegação à esquerda e, em seguida, selecione **registros de aplicativo (visualização)** em **gerenciar**.</span><span class="sxs-lookup"><span data-stu-id="13038-115">Select **Azure Active Directory** in the left-hand navigation, then select **App registrations (Preview)** under **Manage**.</span></span>

    ![<span data-ttu-id="13038-116">Uma captura de tela dos registros de aplicativo</span><span class="sxs-lookup"><span data-stu-id="13038-116">A screenshot of the App registrations</span></span> ](/tutorial/images/aad-portal-app-registrations.png)

1. <span data-ttu-id="13038-117">Selecione **novo registro**.</span><span class="sxs-lookup"><span data-stu-id="13038-117">Select **New registration**.</span></span> <span data-ttu-id="13038-118">Na página **registrar um aplicativo** , defina os valores da seguinte maneira.</span><span class="sxs-lookup"><span data-stu-id="13038-118">On the **Register an application** page, set the values as follows.</span></span>

    - <span data-ttu-id="13038-119">Defina \*\*\*\* o nome `Node.js Graph Tutorial`como.</span><span class="sxs-lookup"><span data-stu-id="13038-119">Set **Name** to `Node.js Graph Tutorial`.</span></span>
    - <span data-ttu-id="13038-120">Defina os **tipos de conta com suporte** para **contas em qualquer diretório organizacional e contas pessoais da Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="13038-120">Set **Supported account types** to **Accounts in any organizational directory and personal Microsoft accounts**.</span></span>
    - <span data-ttu-id="13038-121">Em **URI**de redirecionamento, defina o primeiro menu `Web` suspenso como e defina o `http://localhost:3000/auth/callback`valor como.</span><span class="sxs-lookup"><span data-stu-id="13038-121">Under **Redirect URI**, set the first drop-down to `Web` and set the value to `http://localhost:3000/auth/callback`.</span></span>

    ![Uma captura de tela da página registrar um aplicativo](/tutorial/images/aad-register-an-app.png)

1. <span data-ttu-id="13038-123">Escolha **registrar**.</span><span class="sxs-lookup"><span data-stu-id="13038-123">Choose **Register**.</span></span> <span data-ttu-id="13038-124">Na página **tutorial do gráfico node. js** , copie o valor da **ID do aplicativo (cliente)** e salve-o, você precisará dele na próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="13038-124">On the **Node.js Graph Tutorial** page, copy the value of the **Application (client) ID** and save it, you will need it in the next step.</span></span>

    ![Uma captura de tela da ID do aplicativo do novo registro de aplicativo](/tutorial/images/aad-application-id.png)

1. <span data-ttu-id="13038-126">Selecione **autenticação** em **gerenciar**.</span><span class="sxs-lookup"><span data-stu-id="13038-126">Select **Authentication** under **Manage**.</span></span> <span data-ttu-id="13038-127">Localize a seção **Grant implícita** e habilite os tokens de **ID**.</span><span class="sxs-lookup"><span data-stu-id="13038-127">Locate the **Implicit grant** section and enable **ID tokens**.</span></span> <span data-ttu-id="13038-128">Selecione **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="13038-128">Choose **Save**.</span></span>

    ![Uma captura de tela da seção Grant implícita](/tutorial/images/aad-implicit-grant.png)

1. <span data-ttu-id="13038-130">Selecione **certificados & segredos** sob **gerenciar**.</span><span class="sxs-lookup"><span data-stu-id="13038-130">Select **Certificates & secrets** under **Manage**.</span></span> <span data-ttu-id="13038-131">Selecione o botão **novo cliente secreto** .</span><span class="sxs-lookup"><span data-stu-id="13038-131">Select the **New client secret** button.</span></span> <span data-ttu-id="13038-132">Insira um valor em **Descrição** e selecione uma das opções para **expirar** e escolha **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="13038-132">Enter a value in **Description** and select one of the options for **Expires** and choose **Add**.</span></span>

    ![Uma captura de tela da caixa de diálogo Adicionar um segredo do cliente](/tutorial/images/aad-new-client-secret.png)

1. <span data-ttu-id="13038-134">Copie o valor de segredo do cliente antes de sair desta página.</span><span class="sxs-lookup"><span data-stu-id="13038-134">Copy the client secret value before you leave this page.</span></span> <span data-ttu-id="13038-135">Você precisará dela na próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="13038-135">You will need it in the next step.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="13038-136">Esse segredo do cliente nunca é mostrado novamente, portanto, certifique-se de copiá-lo agora.</span><span class="sxs-lookup"><span data-stu-id="13038-136">This client secret is never shown again, so make sure you copy it now.</span></span>

    ![Uma captura de tela do novo segredo do cliente recentemente adicionado](/tutorial/images/aad-copy-client-secret.png)

## <a name="configure-the-sample"></a><span data-ttu-id="13038-138">Configurar o exemplo</span><span class="sxs-lookup"><span data-stu-id="13038-138">Configure the sample</span></span>

1. <span data-ttu-id="13038-139">ReNomear `.env.example` o `.env`arquivo para.</span><span class="sxs-lookup"><span data-stu-id="13038-139">Rename the `.env.example` file to `.env`.</span></span>
1. <span data-ttu-id="13038-140">Edite `.env` o arquivo e faça as seguintes alterações.</span><span class="sxs-lookup"><span data-stu-id="13038-140">Edit the `.env` file and make the following changes.</span></span>
    1. <span data-ttu-id="13038-141">Substitua `YOUR_APP_ID_HERE` pela **ID do aplicativo** obtida do portal de registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="13038-141">Replace `YOUR_APP_ID_HERE` with the **Application Id** you got from the App Registration Portal.</span></span>
    1. <span data-ttu-id="13038-142">Substitua `YOUR_APP_PASSWORD_HERE` pela senha obtida do portal de registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="13038-142">Replace `YOUR_APP_PASSWORD_HERE` with the password you got from the App Registration Portal.</span></span>
1. <span data-ttu-id="13038-143">Na sua interface de linha de comando (CLI), navegue até este diretório e execute o seguinte comando para instalar os requisitos.</span><span class="sxs-lookup"><span data-stu-id="13038-143">In your command-line interface (CLI), navigate to this directory and run the following command to install requirements.</span></span>

    ```Shell
    npm install
    ```

## <a name="run-the-sample"></a><span data-ttu-id="13038-144">Executar o exemplo</span><span class="sxs-lookup"><span data-stu-id="13038-144">Run the sample</span></span>

1. <span data-ttu-id="13038-145">Execute o comando a seguir em sua CLI para iniciar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="13038-145">Run the following command in your CLI to start the application.</span></span>

    ```Shell
    npm start
    ```

1. <span data-ttu-id="13038-146">Abra um navegador e navegue até `http://localhost:3000`.</span><span class="sxs-lookup"><span data-stu-id="13038-146">Open a browser and browse to `http://localhost:3000`.</span></span>