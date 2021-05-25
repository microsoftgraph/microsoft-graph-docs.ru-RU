<!-- markdownlint-disable MD002 MD041 -->

<span data-ttu-id="1b60c-101">В этом упражнении вы создадим, запустите и утвердите конвейер Azure Data Factory для извлечения данных из Microsoft 365 в служба хранилища Azure Blob для дополнительной обработки.</span><span class="sxs-lookup"><span data-stu-id="1b60c-101">In this exercise you will create, run, and approve an Azure Data Factory pipeline to extract data from Microsoft 365 to an Azure Storage Blob for additional processing.</span></span>

## <a name="create-a-microsoft-azure-active-directory-application-registration"></a><span data-ttu-id="1b60c-102">Создание регистрации Microsoft Azure Active Directory приложений</span><span class="sxs-lookup"><span data-stu-id="1b60c-102">Create a Microsoft Azure Active Directory application registration</span></span>

<span data-ttu-id="1b60c-103">Первым шагом является создание приложения Azure AD, которое будет использоваться в качестве основного обеспечения безопасности для запуска процесса извлечения данных.</span><span class="sxs-lookup"><span data-stu-id="1b60c-103">The first step is to create an Azure AD application that will be used as the security principal to run the data extraction process.</span></span>

1. <span data-ttu-id="1b60c-104">Откройте браузер и перейдите на портал [Azure.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="1b60c-104">Open a browser and go to your [Azure Portal](https://portal.azure.com/).</span></span>

1. <span data-ttu-id="1b60c-105">Впишитесь в использование учетной записи **с правами глобального** администратора для клиентов Azure и Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1b60c-105">Sign in using an account with **Global administrator** rights to your Azure and Microsoft 365 tenants.</span></span>

1. <span data-ttu-id="1b60c-106">На боковой панели навигации **выберите Azure Active Directory** (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="1b60c-106">On the sidebar navigation, select **Azure Active Directory** (Azure AD).</span></span>

1. <span data-ttu-id="1b60c-107">На странице Обзор Azure AD выберите **регистрации приложений** из раздела **Управление** меню.</span><span class="sxs-lookup"><span data-stu-id="1b60c-107">On the Azure AD Overview page, select **App registrations** from the **Manage** section of the menu.</span></span>

1. <span data-ttu-id="1b60c-108">Выберите **кнопку Новая регистрация.**</span><span class="sxs-lookup"><span data-stu-id="1b60c-108">Select the **New registration** button.</span></span>

    ![Снимок экрана, на котором показаны регистрации приложений в Azure Active Directory службе на портале Azure.](images/data-connect-azure-aad-app-reg.png)

1. <span data-ttu-id="1b60c-110">Используйте следующие значения для создания нового приложения Azure AD и выбора **Register.**</span><span class="sxs-lookup"><span data-stu-id="1b60c-110">Use the following values to create a new Azure AD application and select **Register**.</span></span>

   - <span data-ttu-id="1b60c-111">**Имя:** Microsoft Graph Подключение передачи данных</span><span class="sxs-lookup"><span data-stu-id="1b60c-111">**Name**: Microsoft Graph Data Connect Data Transfer</span></span>
   - <span data-ttu-id="1b60c-112">**Поддерживаемые типы** учетных записей. Учетные записи только в этом организационном каталоге.</span><span class="sxs-lookup"><span data-stu-id="1b60c-112">**Supported account types**: Accounts in this organizational directory only.</span></span>
   - <span data-ttu-id="1b60c-113">**Перенаправление URI:** Оставьте значения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1b60c-113">**Redirect URI**: Leave the default values.</span></span>

    ![Снимок экрана, на котором показаны действия по регистрации нового приложения на портале Azure.](images/data-connect-aad-redirect-uri.png)

1. <span data-ttu-id="1b60c-115">Найдите **ID приложения (клиента) и** скопируйте его так, как вам понадобится позже в этом учебнике.</span><span class="sxs-lookup"><span data-stu-id="1b60c-115">Locate the **Application (client) ID** and copy it as you will need it later in this tutorial.</span></span> <span data-ttu-id="1b60c-116">Это будет называться главным ИД службы.</span><span class="sxs-lookup"><span data-stu-id="1b60c-116">This will be referred to as the service principal ID.</span></span>

1. <span data-ttu-id="1b60c-117">Найдите **ID каталога (клиента)** и скопируйте его так, как вам потребуется в этом руководстве.</span><span class="sxs-lookup"><span data-stu-id="1b60c-117">Locate the **Directory (tenant) ID** and copy it as you will need it later in this tutorial.</span></span> <span data-ttu-id="1b60c-118">Это будет называться ИД клиента.</span><span class="sxs-lookup"><span data-stu-id="1b60c-118">This will be referred to as the tenant ID.</span></span>

1. <span data-ttu-id="1b60c-119">На боковой панели навигации выберите **Сертификаты и секреты в** **статье Управление**.</span><span class="sxs-lookup"><span data-stu-id="1b60c-119">On the sidebar navigation, select **Certificates and secrets** under **Manage**.</span></span>

1. <span data-ttu-id="1b60c-120">Выберите **секретную кнопку "Новый клиент".**</span><span class="sxs-lookup"><span data-stu-id="1b60c-120">Select the **New client secret button**.</span></span> <span data-ttu-id="1b60c-121">Установите *описание* для любого имени, установите **Истекает** значение в отсеве и выберите **Добавить**.</span><span class="sxs-lookup"><span data-stu-id="1b60c-121">Set *Description* to any name, set **Expires** to any value in the dropdown and choose **Add**.</span></span>

    ![Снимок экрана, показывающий процесс создания нового секрета клиента на портале Azure.](images/data-connect-aad-certs-secrets.png)

    - <span data-ttu-id="1b60c-123">После создания секрета клиента убедитесь,  что вы сохраните значение в безопасном месте, так как оно больше не будет доступно позже, и вам потребуется создать новое.</span><span class="sxs-lookup"><span data-stu-id="1b60c-123">After the client secret is created, make sure you save the **Value** somewhere safe, as it will no longer be available later, and you will need to create a new one.</span></span>
    - <span data-ttu-id="1b60c-124">Это будет ссылаться в качестве основного ключа службы.</span><span class="sxs-lookup"><span data-stu-id="1b60c-124">This will be referenced as the service principal key.</span></span>

1. <span data-ttu-id="1b60c-125">На боковой панели навигации для приложения выберите **Owners**.</span><span class="sxs-lookup"><span data-stu-id="1b60c-125">On the sidebar navigation for the application, select **Owners**.</span></span>

1. <span data-ttu-id="1b60c-126">Убедитесь, что ваша учетная запись указана как владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="1b60c-126">Verify that your account is listed as an owner for the application.</span></span> <span data-ttu-id="1b60c-127">Если он не указан как владелец, добавьте его.</span><span class="sxs-lookup"><span data-stu-id="1b60c-127">If it isn't listed as an owner, add it.</span></span>

    ![Снимок экрана, на котором пользователь проверяет, установлен ли его учетная запись в качестве владельца для регистрации приложений на портале Azure.](images/data-connect-aad-app-owners.png)
