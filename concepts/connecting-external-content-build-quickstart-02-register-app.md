<!-- markdownlint-disable MD002 MD041 -->

<span data-ttu-id="6f8d6-101">После того как все необходимые условия будут созданы, вы сможете зарегистрировать приложение в центре администрирования Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6f8d6-101">After all the prerequisites are in place, you will be able to register an application in the Azure AD admin center.</span></span> <span data-ttu-id="6f8d6-102">Регистрация необходима для проверки подлинности приложения и его использования для звонков в API соединителов Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6f8d6-102">The registration is necessary in order to authenticate the application and use it to make calls to the Microsoft Graph connectors API.</span></span>

1. <span data-ttu-id="6f8d6-103">Перейдите в [центр Azure Active Directory администратора](https://aad.portal.azure.com/) и войдите в учетную запись администратора.</span><span class="sxs-lookup"><span data-stu-id="6f8d6-103">Go to the [Azure Active Directory admin center](https://aad.portal.azure.com/) and sign in with an administrator account.</span></span>
2. <span data-ttu-id="6f8d6-104">На левой области выберите **Azure Active Directory,** а в статье **Управление** выберите **регистрации приложений.**</span><span class="sxs-lookup"><span data-stu-id="6f8d6-104">On the left pane, select **Azure Active Directory**, and under **Manage**, select **App registrations**.</span></span>
3. <span data-ttu-id="6f8d6-105">Выберите **Новая регистрация**.</span><span class="sxs-lookup"><span data-stu-id="6f8d6-105">Select **New registration**.</span></span>

    ![Снимок экрана, показывающий раздел "Регистрация приложений"](images/connectors-images/build2.png)

4. <span data-ttu-id="6f8d6-107">**Заполняем форму приложения Register** со следующими значениями, а затем выберите **Register**.</span><span class="sxs-lookup"><span data-stu-id="6f8d6-107">Complete the **Register an application** form with the following values, then select **Register**.</span></span>

    <span data-ttu-id="6f8d6-108">а)</span><span class="sxs-lookup"><span data-stu-id="6f8d6-108">a.</span></span> <span data-ttu-id="6f8d6-109">**Имя:** Соединители запасов частей</span><span class="sxs-lookup"><span data-stu-id="6f8d6-109">**Name**: Parts Inventory Connector</span></span>

    <span data-ttu-id="6f8d6-110">б)</span><span class="sxs-lookup"><span data-stu-id="6f8d6-110">b.</span></span> <span data-ttu-id="6f8d6-111">**Поддерживаемые типы** учетных записей. Учетные записи только в этом организационном каталоге (только Microsoft — один клиент)</span><span class="sxs-lookup"><span data-stu-id="6f8d6-111">**Supported account types**: Accounts in this organizational directory only (Microsoft only - Single tenant)</span></span>

    <span data-ttu-id="6f8d6-112">В.</span><span class="sxs-lookup"><span data-stu-id="6f8d6-112">c.</span></span> <span data-ttu-id="6f8d6-113">**Перенаправление URI:** оставьте пустым</span><span class="sxs-lookup"><span data-stu-id="6f8d6-113">**Redirect URI**: Leave blank</span></span>

    ![Снимок экрана, показывающий раздел "Регистрация приложения"](images/connectors-images/build3-contoso-register-app.png)

5. <span data-ttu-id="6f8d6-115">На странице обзор соединители запасов частей скопируйте значения **ID приложения (клиента) и directory (tenant) ID.**</span><span class="sxs-lookup"><span data-stu-id="6f8d6-115">On the Parts Inventory Connector overview page, copy the values of **Application (client) ID and Directory (tenant) ID**.</span></span> <span data-ttu-id="6f8d6-116">Вам потребуется и то, и другое в следующем разделе.</span><span class="sxs-lookup"><span data-stu-id="6f8d6-116">You will need both in the following section.</span></span>

    ![Снимок экрана, показывающий раздел "Соединители запасов частей"](images/connectors-images/build3-contoso-partsinv.png)

6. <span data-ttu-id="6f8d6-118">Выберите **разрешения API в** статье **Управление**.</span><span class="sxs-lookup"><span data-stu-id="6f8d6-118">Select **API Permissions** under **Manage**.</span></span>
7. <span data-ttu-id="6f8d6-119">Выберите **Добавить разрешение,** а затем выберите **Microsoft Graph.**</span><span class="sxs-lookup"><span data-stu-id="6f8d6-119">Select **Add a permission**, then select **Microsoft Graph**.</span></span>
8. <span data-ttu-id="6f8d6-120">Выберите **разрешения приложения,** а затем выберите **разрешение ExternalItem.ReadWrite.All.**</span><span class="sxs-lookup"><span data-stu-id="6f8d6-120">Select **Application permissions**, then select the **ExternalItem.ReadWrite.All** permission.</span></span> <span data-ttu-id="6f8d6-121">Выберите **Добавить разрешения**.</span><span class="sxs-lookup"><span data-stu-id="6f8d6-121">Select **Add permissions**.</span></span>

    ![Снимок экрана, показывающий раздел "Разрешения API запроса"](images/connectors-images/build4.png)

9. <span data-ttu-id="6f8d6-123">Выберите **согласие администратора гранта для {TENANT},** а затем выберите **Да** при запросе.</span><span class="sxs-lookup"><span data-stu-id="6f8d6-123">Select **Grant admin consent for {TENANT},** then select **Yes** when prompted.</span></span>

    ![Снимок экрана, показывающий раздел "Разрешения api соединитетеля запасов частей"](images/connectors-images/build5.png)

10. <span data-ttu-id="6f8d6-125">Выберите **секреты &amp; сертификатов в** статье **Управление,** а затем выберите новый секрет **клиента.**</span><span class="sxs-lookup"><span data-stu-id="6f8d6-125">Select **Certificates &amp; secrets** under **Manage** , then select **New client secret**.</span></span>
11. <span data-ttu-id="6f8d6-126">Введите описание и выберите срок действия секрета, а затем выберите **Добавить**.</span><span class="sxs-lookup"><span data-stu-id="6f8d6-126">Enter a description and choose an expiration time for the secret, then select **Add**.</span></span>

    ![Снимок экрана, показывающий раздел "Сертифиции и секреты соединитетеля запасов частей"](images/connectors-images/build6.png)

12. <span data-ttu-id="6f8d6-128">Скопируйте и сохраните новый секрет, он потребуется в следующем разделе.</span><span class="sxs-lookup"><span data-stu-id="6f8d6-128">Copy and save the new secret, you will need it in the following section.</span></span>
