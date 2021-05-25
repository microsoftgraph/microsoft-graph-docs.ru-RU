<!-- markdownlint-disable MD002 MD041 -->

<span data-ttu-id="05723-101">На этом шаге будет служба хранилища Azure учетная запись, подключение к данным Microsoft Graph будет хранить данные, извлеченные из Microsoft 365 для дальнейшей обработки.</span><span class="sxs-lookup"><span data-stu-id="05723-101">In this step you will create an Azure Storage account where Microsoft Graph data connect will store the data extracted from Microsoft 365 for further processing.</span></span>

1. <span data-ttu-id="05723-102">Откройте браузер и перейдите на портал [Azure.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="05723-102">Open a browser and go to your [Azure Portal](https://portal.azure.com/).</span></span>

1. <span data-ttu-id="05723-103">Впишитесь в использование учетной записи **с правами глобального** администратора для клиентов Azure и Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="05723-103">Sign in using an account with **Global administrator** rights to your Azure and Microsoft 365 tenants.</span></span>

1. <span data-ttu-id="05723-104">На боковой панели навигации выберите **Создать ресурс**.</span><span class="sxs-lookup"><span data-stu-id="05723-104">On the sidebar navigation, select **Create a resource**.</span></span>

1. <span data-ttu-id="05723-105">Найдите **тип служба хранилища** учетной записи и создайте его с помощью следующих значений, а затем выберите Обзор + **создание**.</span><span class="sxs-lookup"><span data-stu-id="05723-105">Find the **Storage Account** resource type and use the following values to create it, then select **Review + create**.</span></span>

    - <span data-ttu-id="05723-106">**Подписка:** выберите подписку Azure</span><span class="sxs-lookup"><span data-stu-id="05723-106">**Subscription**: select your Azure subscription</span></span>
    - <span data-ttu-id="05723-107">**Группа ресурсов:** GraphDataConnect (или выберите существующую группу ресурсов)</span><span class="sxs-lookup"><span data-stu-id="05723-107">**Resource group**: GraphDataConnect (or select an existing resource group)</span></span>
    - <span data-ttu-id="05723-108">**служба хранилища учетной записи:** mgdcm365datastore</span><span class="sxs-lookup"><span data-stu-id="05723-108">**Storage account name**: mgdcm365datastore</span></span>
    - <span data-ttu-id="05723-109">**Регион:** выберите регион Azure в том же регионе, что и Microsoft 365 регионе</span><span class="sxs-lookup"><span data-stu-id="05723-109">**Region**: pick an Azure region in the same region as your Microsoft 365 region</span></span>
    - <span data-ttu-id="05723-110">**Производительность:** стандартный</span><span class="sxs-lookup"><span data-stu-id="05723-110">**Performance**: Standard</span></span>
    - <span data-ttu-id="05723-111">**Избыточность:** хранилище с геоотековой избыточной памятью (GRS)</span><span class="sxs-lookup"><span data-stu-id="05723-111">**Redundancy**: Geo-redundant storage (GRS)</span></span>
    - <span data-ttu-id="05723-112">**Расширенный вкладка**:</span><span class="sxs-lookup"><span data-stu-id="05723-112">**Advanced tab**:</span></span>
      - <span data-ttu-id="05723-113">**Уровень доступа**: Hot</span><span class="sxs-lookup"><span data-stu-id="05723-113">**Access tier**: Hot</span></span>

1. <span data-ttu-id="05723-114">Просмотрите, что параметры соответствуют тем, которые были показаны на предыдущем шаге, и выберите **Create**.</span><span class="sxs-lookup"><span data-stu-id="05723-114">Review that the settings match those shown in the previous step and select **Create**.</span></span>

1. <span data-ttu-id="05723-115">После создания служба хранилища Azure учетной записи предоставить приложению Azure AD ранее созданный надлежащий доступ к нему.</span><span class="sxs-lookup"><span data-stu-id="05723-115">After the Azure Storage account has been created, grant the Azure AD application previously created the proper access to it.</span></span>

    1. <span data-ttu-id="05723-116">Выберите служба хранилища Azure **учетную запись.**</span><span class="sxs-lookup"><span data-stu-id="05723-116">Select the **Azure Storage account**.</span></span>
    2. <span data-ttu-id="05723-117">В меню боковой панели выберите **управление доступом (IAM).**</span><span class="sxs-lookup"><span data-stu-id="05723-117">On the sidebar menu, select **Access control (IAM)**.</span></span>
    3. <span data-ttu-id="05723-118">Выберите **кнопку Добавить** в **блоке Добавление назначения ролей.**</span><span class="sxs-lookup"><span data-stu-id="05723-118">Select the **Add** button in the **Add a role assignment** block.</span></span>
    4. <span data-ttu-id="05723-119">Используйте следующие значения, чтобы найти приложение, которое было выбрано ранее, чтобы предоставить ему роль **служба хранилища Blob Data Contributor,** а затем выберите **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="05723-119">Use the following values to find the application you previously selected to grant it the **Storage Blob Data Contributor** role, then select **Save**.</span></span>

        - <span data-ttu-id="05723-120">**Роль**: служба хранилища Blob Data Contributor</span><span class="sxs-lookup"><span data-stu-id="05723-120">**Role**: Storage Blob Data Contributor</span></span>
        - <span data-ttu-id="05723-121">**Назначение доступа** к: пользователю, группе или основной службе</span><span class="sxs-lookup"><span data-stu-id="05723-121">**Assign access to**: User, group or service principal</span></span>
        - <span data-ttu-id="05723-122">**Выберите**: подключение к данным Microsoft Graph передачи данных (имя созданного ранее приложения Azure AD)</span><span class="sxs-lookup"><span data-stu-id="05723-122">**Select**: Microsoft Graph data connect Data Transfer (the name of the Azure AD application you created previously)</span></span>

        ![Снимок экрана, показывающий правильное назначение ролей приложению для Microsoft Graph Data Подключение в служба хранилища Azure учетной записи на портале Azure.](images/data-connect-azure-storage-role.png)

1. <span data-ttu-id="05723-124">Создайте новый контейнер в учетной записи **mgdcm365datastore** служба хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="05723-124">Create a new container in the **mgdcm365datastore** Azure Storage account.</span></span>

    1. <span data-ttu-id="05723-125">Выберите **учетную запись mgdcm365datastore** служба хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="05723-125">Select the **mgdcm365datastore** Azure Storage account.</span></span>
    2. <span data-ttu-id="05723-126">В меню боковой панели выберите **Контейнеры** в разделе **служба Blob.**</span><span class="sxs-lookup"><span data-stu-id="05723-126">On the sidebar menu, select **Containers** under the **Blob** service section.</span></span>
    3. <span data-ttu-id="05723-127">Выберите **кнопку +Container** в верхней части страницы и используйте следующие значения, а затем выберите **Создать**.</span><span class="sxs-lookup"><span data-stu-id="05723-127">Select the **+Container** button at the top of the page and use the following values and then select **Create**.</span></span>

        - <span data-ttu-id="05723-128">**Имя:** m365mails</span><span class="sxs-lookup"><span data-stu-id="05723-128">**Name**: m365mails</span></span>
        - <span data-ttu-id="05723-129">**Уровень общего доступа:** частный (без анонимного доступа)</span><span class="sxs-lookup"><span data-stu-id="05723-129">**Public access level**: Private (no anonymous access)</span></span>

        ![Снимок экрана, показывающий создание нового контейнера m365mails в контейнерах blob служба хранилища учетной записи на портале Azure.](images/data-connect-azure-storage-container.png)
