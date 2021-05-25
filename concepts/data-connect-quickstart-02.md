<!-- markdownlint-disable MD002 MD041 -->

<span data-ttu-id="864cc-101">Перед использованием microsoft Graph данных Подключение в первый раз, необходимо настроить Microsoft 365 клиента.</span><span class="sxs-lookup"><span data-stu-id="864cc-101">Prior to using Microsoft Graph Data Connect for the first time, you need to configure your Microsoft 365 tenant.</span></span> <span data-ttu-id="864cc-102">Это включает включение службы и настройку группы безопасности с разрешениями на утверждение запросов на извлечение данных.</span><span class="sxs-lookup"><span data-stu-id="864cc-102">This involves turning on the service and configuring a security group with permissions to approve data extraction requests.</span></span>

## <a name="grant-azure-ad-users-the-global-administrator-role"></a><span data-ttu-id="864cc-103">Предоставление пользователям Azure AD роли глобального администратора</span><span class="sxs-lookup"><span data-stu-id="864cc-103">Grant Azure AD users the Global administrator role</span></span>

<span data-ttu-id="864cc-104">На этом шаге вы убедитесь, что два Microsoft 365 клиента имеют роль **глобального администратора.**</span><span class="sxs-lookup"><span data-stu-id="864cc-104">In this step, you will ensure that two users in your Microsoft 365 tenant have the **Global administrator** role enabled.</span></span>

- <span data-ttu-id="864cc-105">[Встроенная роль глобального администратора](/azure/active-directory/roles/permissions-reference#global-administrator).</span><span class="sxs-lookup"><span data-stu-id="864cc-105">[Global Administrator built-in role](/azure/active-directory/roles/permissions-reference#global-administrator).</span></span>
- <span data-ttu-id="864cc-106">[Повышение доступности для получения роли глобального администратора.](/azure/role-based-access-control/elevate-access-global-admin)</span><span class="sxs-lookup"><span data-stu-id="864cc-106">[Elevate access to gain the Global Administrator role](/azure/role-based-access-control/elevate-access-global-admin).</span></span>

## <a name="configure-microsoft-graph-data-connect-consent-request-approver-group"></a><span data-ttu-id="864cc-107">Настройка группы утверждения запроса Graph данных Подключение Майкрософт</span><span class="sxs-lookup"><span data-stu-id="864cc-107">Configure Microsoft Graph Data Connect consent request approver group</span></span>

<span data-ttu-id="864cc-108">На этом шаге вы настроите Microsoft 365 клиента, чтобы включить использование Microsoft Graph data Подключение.</span><span class="sxs-lookup"><span data-stu-id="864cc-108">In this step, you will setup your Microsoft 365 tenant to enable usage of Microsoft Graph Data Connect.</span></span>

1. <span data-ttu-id="864cc-109">Откройте браузер и перейдите [на Microsoft 365 Портал администрирования.](https://admin.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="864cc-109">Open a browser and go to your [Microsoft 365 Admin Portal](https://admin.microsoft.com/).</span></span>

1. <span data-ttu-id="864cc-110">На боковой панели навигации выберите **Active Groups**.</span><span class="sxs-lookup"><span data-stu-id="864cc-110">On the sidebar navigation, select **Active Groups**.</span></span>
  
    ![Снимок экрана, на котором показаны активные группы Microsoft 365 центра администрирования.](images/data-connect-m365-act-grp.png)

1. <span data-ttu-id="864cc-112">Выберите **кнопку Добавить группу.**</span><span class="sxs-lookup"><span data-stu-id="864cc-112">Select the **Add a group** button.</span></span>

1. <span data-ttu-id="864cc-113">Создайте новую группу  безопасности с поддержкой почты и выберите кнопку **Добавить.**</span><span class="sxs-lookup"><span data-stu-id="864cc-113">Use the following to create the new **mail-enabled** security group and select the **Add** button.</span></span>
   - <span data-ttu-id="864cc-114">**Тип:** безопасность с поддержкой почты</span><span class="sxs-lookup"><span data-stu-id="864cc-114">**Type**: Mail-enabled security</span></span>

    ![Снимок экрана, на котором пользователь выбирает безопасность с включенной почтой для новой группы в центре Microsoft 365 администратора.](images/data-connect-m365-mail-sec.png)

   - <span data-ttu-id="864cc-116">**Имя:** Одобрение запроса на согласие</span><span class="sxs-lookup"><span data-stu-id="864cc-116">**Name**: Consent Request Approvers</span></span>

    ![Снимок экрана, на котором пользователь дает группе имя "Утверждения запросов на согласие" в центре Microsoft 365 администрирования.](images/data-connect-m365-cons-apprv.png)

   - <span data-ttu-id="864cc-118">**Префикс электронной почты:** consentrequestapprovers</span><span class="sxs-lookup"><span data-stu-id="864cc-118">**Email Prefix**: consentrequestapprovers</span></span>

    ![Снимок экрана с изображением пользователя, создав адрес электронной почты для ранее созданной группы в центре Microsoft 365 администратора.](images/data-connect-m365-cons-apprv-pref.png)

1. <span data-ttu-id="864cc-120">**Это может занять до часа,** прежде чем вновь созданная группа появляется в списке.</span><span class="sxs-lookup"><span data-stu-id="864cc-120">**It can take up to an hour** before the newly created group shows up in the list.</span></span> <span data-ttu-id="864cc-121">После создания группы выберите ее.</span><span class="sxs-lookup"><span data-stu-id="864cc-121">When the group has been created, select it.</span></span>

1. <span data-ttu-id="864cc-122">Снова перейдите **к параметру Active groups** и найдите только что созданную группу.</span><span class="sxs-lookup"><span data-stu-id="864cc-122">Go to the **Active groups** option again and search for the group you just created.</span></span>

1. <span data-ttu-id="864cc-123">Выберите группу и на **вкладке Участники,** выберите **Просмотр всех и управление участниками.**</span><span class="sxs-lookup"><span data-stu-id="864cc-123">Select the group and in the **Members** tab, select **View all and manage members**.</span></span>

1. <span data-ttu-id="864cc-124">Добавьте двух пользователей, которые включили роль **глобального администратора** в эту новую группу.</span><span class="sxs-lookup"><span data-stu-id="864cc-124">Add the two users that you enabled the **Global administrator** role to this new group.</span></span>

## <a name="enable-microsoft-graph-data-connect-in-your-microsoft-365-tenant"></a><span data-ttu-id="864cc-125">Включить microsoft Graph data Подключение в Microsoft 365 клиенте</span><span class="sxs-lookup"><span data-stu-id="864cc-125">Enable Microsoft Graph Data Connect in your Microsoft 365 tenant</span></span>

<span data-ttu-id="864cc-126">На этом шаге вы включаете службу Microsoft Graph data Подключение на Microsoft 365 клиента.</span><span class="sxs-lookup"><span data-stu-id="864cc-126">In this step, you will enable the Microsoft Graph Data Connect service on your Microsoft 365 tenant.</span></span>

1. <span data-ttu-id="864cc-127">В то время как вы все еще подписаны на портал администрирования Microsoft 365, выберите **пункт меню параметров Параметры > Org.**</span><span class="sxs-lookup"><span data-stu-id="864cc-127">While you are still signed in to the Microsoft 365 Admin Portal, select the **Settings > Org settings** menu item.</span></span>

1. <span data-ttu-id="864cc-128">Выберите **службу Microsoft Graph data Подключение.**</span><span class="sxs-lookup"><span data-stu-id="864cc-128">Select the **Microsoft Graph Data Connect** service.</span></span>

    ![Снимок экрана, показывающий "Службы" в лезвии "Параметры Org".](images/data-connect-m365-mgdc-toggle.png)

1. <span data-ttu-id="864cc-131">Выберите почтовый ящик, включив Graph **microsoft Подключение** для всей организации, чтобы включить Подключение.</span><span class="sxs-lookup"><span data-stu-id="864cc-131">Select the checkbox that says **turn Microsoft Graph Data Connect on or off for your entire organization** to enable Data Connect.</span></span>

    ![Снимок экрана, на котором показывая почтовый ящик, который необходимо тикать, чтобы включить Подключение для всей организации.](images/data-connect-m365-enable-mgdc-for-org.png)

1. <span data-ttu-id="864cc-133">Введите **утверждения запросов** на согласие (или имя группы,  созданной ранее) в группе пользователей для принятия решений об утверждении и выбора **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="864cc-133">Enter **Consent Request Approvers** (or the name of the group you created previously) in the **group of users to make approval decisions** and select **Save**.</span></span>
