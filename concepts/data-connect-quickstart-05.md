<!-- markdownlint-disable MD002 MD041 -->

<span data-ttu-id="61eef-101">Следующим шагом является использование фабрики данных Azure для создания конвейера для извлечения данных из Microsoft 365 в учетную запись служба хранилища Azure с помощью подключение к данным Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="61eef-101">The next step is to use the Azure Data Factory to create a pipeline to extract the data from Microsoft 365 to the Azure Storage account using Microsoft Graph data connect.</span></span>

## <a name="create-an-azure-data-factory-pipeline"></a><span data-ttu-id="61eef-102">Создание конвейера Фабрики данных Azure</span><span class="sxs-lookup"><span data-stu-id="61eef-102">Create an Azure Data Factory pipeline</span></span>

1. <span data-ttu-id="61eef-103">Откройте браузер и перейдите на портал [Azure.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="61eef-103">Open a browser and go to your [Azure Portal](https://portal.azure.com/).</span></span>

1. <span data-ttu-id="61eef-104">Впишитесь в использование учетной записи **с правами глобального** администратора для клиентов Azure и Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="61eef-104">Sign in using an account with **Global administrator** rights to your Azure and Microsoft 365 tenants.</span></span>

1. <span data-ttu-id="61eef-105">На боковой панели навигации выберите **Создать ресурс**.</span><span class="sxs-lookup"><span data-stu-id="61eef-105">On the sidebar navigation, select **Create a resource**.</span></span>

1. <span data-ttu-id="61eef-106">Найдите **тип ресурса Фабрика** данных и используйте для его создания следующие значения, а затем выберите **Create**.</span><span class="sxs-lookup"><span data-stu-id="61eef-106">Find the **Data Factory** resource type and use the following values to create it, then select **Create**.</span></span>

    1. <span data-ttu-id="61eef-107">**Подписка:** выберите подписку Azure</span><span class="sxs-lookup"><span data-stu-id="61eef-107">**Subscription**: select your Azure subscription</span></span>
    2. <span data-ttu-id="61eef-108">**Группа ресурсов:** GraphDataConnect</span><span class="sxs-lookup"><span data-stu-id="61eef-108">**Resource group**: GraphDataConnect</span></span>
    3. <span data-ttu-id="61eef-109">**Регион:** выберите регион Azure в том же регионе, что и Microsoft 365 регионе</span><span class="sxs-lookup"><span data-stu-id="61eef-109">**Region**: pick an Azure region in the same region as your Microsoft 365 region</span></span>
    4. <span data-ttu-id="61eef-110">**Имя:** dfM365toBlobStorage</span><span class="sxs-lookup"><span data-stu-id="61eef-110">**Name**: dfM365toBlobStorage</span></span>
    5. <span data-ttu-id="61eef-111">**Версия:** V2</span><span class="sxs-lookup"><span data-stu-id="61eef-111">**Version**: V2</span></span>

        ![Снимок экрана, показывающий успешное создание новой службы Фабрики данных Azure на портале Azure.](images/data-connect-adf-create.png)

    6. <span data-ttu-id="61eef-113">На **вкладке конфигурации Git** убедитесь, что вы либо настраивали Git, либо выберите параметр _Configure Git позже._</span><span class="sxs-lookup"><span data-stu-id="61eef-113">In the **Git configuration** tab, make sure you either configure Git or select the option _Configure Git later_.</span></span>

1. <span data-ttu-id="61eef-114">После создания ресурса Фабрика данных Azure выберите плитку **Author и Monitor** для запуска редактора полного экрана Azure Data Factory.</span><span class="sxs-lookup"><span data-stu-id="61eef-114">After the Azure Data Factory resource is created, select the **Author and Monitor** tile to launch the Azure Data Factory full screen editor.</span></span>

    ![Снимок экрана, на котором показан пользовательский интерфейс Azure Portal для службы фабрики данных.](images/data-connect-adf-auth-and-mon.png)

1. <span data-ttu-id="61eef-117">Переключение с **"Обзор"** на **"Управление** опытом", выбрав его из левой навигации.</span><span class="sxs-lookup"><span data-stu-id="61eef-117">Switch from the **Overview** to the **Manage** experience by selecting it from the left-hand navigation.</span></span>

1. <span data-ttu-id="61eef-118">По умолчанию фабрика данных Azure будет использовать время запуска интеграции, которое автоматически разрешит область.</span><span class="sxs-lookup"><span data-stu-id="61eef-118">By default, the Azure Data Factory will use an integration runtime that is auto-resolving the region.</span></span> <span data-ttu-id="61eef-119">Поскольку для Подключение данных требуется, чтобы ваш источник и назначение, а также время запуска интеграции существовали в одном Microsoft 365 регионе, рекомендуется создать новое время запуска интеграции с фиксированным регионом.</span><span class="sxs-lookup"><span data-stu-id="61eef-119">Because Data Connect requires that your source and destination, and integration runtime to exist in the same Microsoft 365 region, we recommend that you create a new integration runtime with a fixed region.</span></span>

    1. <span data-ttu-id="61eef-120">Выберите **время запуска**  >  **интеграции New**.</span><span class="sxs-lookup"><span data-stu-id="61eef-120">Select **Integration runtimes** > **New**.</span></span>
    2. <span data-ttu-id="61eef-121">Выберите **Azure, самообуправление и** выберите **Продолжить**.</span><span class="sxs-lookup"><span data-stu-id="61eef-121">Select **Azure, Self-Hosted** and select **Continue**.</span></span>
    3. <span data-ttu-id="61eef-122">Выберите **Azure** для сетевой среды и выберите **Продолжить**.</span><span class="sxs-lookup"><span data-stu-id="61eef-122">Select **Azure** for network environment and select **Continue**.</span></span>

        ![Снимок экрана, на котором показан пользовательский интерфейс Azure Portal для службы фабрики данных.](images/data-connect-adf-network.png)

    4. <span data-ttu-id="61eef-125">Чтобы заполнить форму на окончательном экране, используйте следующие сведения, а затем выберите **Create**.</span><span class="sxs-lookup"><span data-stu-id="61eef-125">Use the following details to complete the form on the final screen and then select **Create**.</span></span>

        - <span data-ttu-id="61eef-126">**Имя:** имя времени запуска интеграции</span><span class="sxs-lookup"><span data-stu-id="61eef-126">**Name**: name of your integration runtime</span></span>
        - <span data-ttu-id="61eef-127">**Описание:** введите описание</span><span class="sxs-lookup"><span data-stu-id="61eef-127">**Description**: enter a description</span></span>
        - <span data-ttu-id="61eef-128">**Регион:** выберите регион, который соответствует вашему Microsoft 365 региону</span><span class="sxs-lookup"><span data-stu-id="61eef-128">**Region**: select the region that matches your Microsoft 365 region</span></span>
        - <span data-ttu-id="61eef-129">**Виртуальная конфигурация сети (предварительный просмотр)**: Отключено</span><span class="sxs-lookup"><span data-stu-id="61eef-129">**Virtual network configuration (preview)**: Disabled</span></span>

1. <span data-ttu-id="61eef-130">Переключиться с **"Управление"** на **"Автор",** выбрав его из левой навигации.</span><span class="sxs-lookup"><span data-stu-id="61eef-130">Switch from the **Manage** to the **Author** experience by selecting it from the left-hand navigation.</span></span>
1. <span data-ttu-id="61eef-131">Создайте новый конвейер, выбрав значок **плюс,** а затем **конвейер.**</span><span class="sxs-lookup"><span data-stu-id="61eef-131">Create a new pipeline by selecting the **plus** icon, then **pipeline**.</span></span>

    ![Снимок экрана, на котором показан пользовательский интерфейс портала Azure для службы фабрики данных.](images/data-connect-adf-pipeline-create.png)

    - <span data-ttu-id="61eef-134">**Перетащите действие Copy Data** из раздела Перемещение и **Преобразование** на поверхность разработки.</span><span class="sxs-lookup"><span data-stu-id="61eef-134">Drag the **Copy Data** activity from the **Move and Transform** section onto the design surface.</span></span>

        ![Снимок экрана, на котором показан пользовательский интерфейс портала Azure для службы фабрики данных.](images/data-connect-adf-pipeline-copy-data.png)

    - <span data-ttu-id="61eef-137">Выберите действие в конструкторе.</span><span class="sxs-lookup"><span data-stu-id="61eef-137">Select the activity in the designer.</span></span>
    - <span data-ttu-id="61eef-138">Выберите **вкладку General** и назови ей имя и описание.</span><span class="sxs-lookup"><span data-stu-id="61eef-138">Select the **General** tab and give it a name and description.</span></span>

      - <span data-ttu-id="61eef-139">**Имя:** CopyFromM365toBlobStorage</span><span class="sxs-lookup"><span data-stu-id="61eef-139">**Name**: CopyFromM365toBlobStorage</span></span>
      - <span data-ttu-id="61eef-140">**Описание.** Описание, необходимое.</span><span class="sxs-lookup"><span data-stu-id="61eef-140">**Description**: A description you want.</span></span>

    - <span data-ttu-id="61eef-141">В области редактора действий ниже конструктора выберите вкладку **Source,** а затем выберите **New**.</span><span class="sxs-lookup"><span data-stu-id="61eef-141">In the activity editor pane below the designer, select the **Source** tab, then select **New**.</span></span>
    - <span data-ttu-id="61eef-142">Найдите набор **Office 365,** выберите его и выберите кнопку **Продолжить.**</span><span class="sxs-lookup"><span data-stu-id="61eef-142">Locate the dataset **Office 365**, select it and then select the **Continue** button.</span></span>

        ![Снимок экрана, на котором показан пользовательский интерфейс портала Azure для службы фабрики данных.](images/data-connect-adf-pipeline-dataset.png)

    - <span data-ttu-id="61eef-145">Конструктор обновляет вкладку **Source** с помощью параметров Microsoft 365 соединители.</span><span class="sxs-lookup"><span data-stu-id="61eef-145">The designer will update the **Source** tab with the Microsoft 365 connector settings.</span></span>
    - <span data-ttu-id="61eef-146">Выберите параметр **Open** рядом с **полем Исходный набор** данных.</span><span class="sxs-lookup"><span data-stu-id="61eef-146">Select the **Open** option next to the **Source dataset** field.</span></span>
    - <span data-ttu-id="61eef-147">В параметрах таблицы выберите вкладку **Подключение,** а затем **кнопку New.**</span><span class="sxs-lookup"><span data-stu-id="61eef-147">In the table settings, select the **Connection** tab, then the **New** button.</span></span>
    - <span data-ttu-id="61eef-148">В диалоговом окте, который отображается, введите ранее созданный **ID** приложения Azure  AD и секретный **ID** в полях основных ИД служб и основных ключевых ключевых служб соответственно, а затем выберите  **Создать**.</span><span class="sxs-lookup"><span data-stu-id="61eef-148">In the dialog that appears, enter the previously created Azure AD application's **Application ID** and **Secret ID** in the **Service principal ID** and **Service principal key** fields respectively, then select **Create**.</span></span>
    - <span data-ttu-id="61eef-149">Выберите время запуска интеграции, созданное ранее в **Подключение** при отсеве времени интеграции.</span><span class="sxs-lookup"><span data-stu-id="61eef-149">Select the integration runtime you previously created in the **Connect via integration runtime** dropdown.</span></span>

        ![Снимок экрана, на котором показан пользовательский интерфейс портала Azure для службы фабрики данных.](images/data-connect-adf-linked-service.png)

    - <span data-ttu-id="61eef-152">После создания Microsoft 365 для поля **Таблицы** выберите **BasicDataSet_v0. Message_v0**.</span><span class="sxs-lookup"><span data-stu-id="61eef-152">After creating the Microsoft 365 connection, for the **Table** field, select **BasicDataSet_v0.Message_v0**.</span></span>
    - <span data-ttu-id="61eef-153">Переключение **с Office365Table** на **источник > Pipeline.**</span><span class="sxs-lookup"><span data-stu-id="61eef-153">Switch from **Office365Table** to **Pipeline > Source**.</span></span> <span data-ttu-id="61eef-154">Используйте следующие значения для фильтра **Date.**</span><span class="sxs-lookup"><span data-stu-id="61eef-154">Use the following values for the **Date filter**.</span></span>

      - <span data-ttu-id="61eef-155">**Имя столбца:** CreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="61eef-155">**Column name**: CreatedDateTime</span></span>
      - <span data-ttu-id="61eef-156">**Время начала (UTC)**: выберите дату до текущей даты</span><span class="sxs-lookup"><span data-stu-id="61eef-156">**Start time (UTC)**: select a date sometime prior to the current date</span></span>
      - <span data-ttu-id="61eef-157">**Время окончания (UTC)**: выберите текущую дату</span><span class="sxs-lookup"><span data-stu-id="61eef-157">**End time (UTC)**: select the current date</span></span>
      - <span data-ttu-id="61eef-158">Выберите **схему импорта** в разделе _Выходные столбцы._</span><span class="sxs-lookup"><span data-stu-id="61eef-158">Select **Import schema** in the _Output columns_ section.</span></span>

    - <span data-ttu-id="61eef-159">Выберите действие **копирования** данных на вкладке конвейера, а затем вкладки **Sink.**</span><span class="sxs-lookup"><span data-stu-id="61eef-159">Select the **Copy data** activity in the pipeline tab, then select the **Sink** tab.</span></span>

      - <span data-ttu-id="61eef-160">Выберите **кнопку New,** выберите **служба хранилища Azure Blob** и выберите кнопку **Продолжить.**</span><span class="sxs-lookup"><span data-stu-id="61eef-160">Select the **New** button, select **Azure Blob Storage**, and then select the **Continue** button.</span></span>
      - <span data-ttu-id="61eef-161">Выберите **двоичный** формат для данных, а затем выберите кнопку **Продолжить.**</span><span class="sxs-lookup"><span data-stu-id="61eef-161">Select **Binary** as the format for the data and then select the **Continue** button.</span></span>
      - <span data-ttu-id="61eef-162">Дайте набору данных имя **M365JsonFile** и создайте новую связанную службу, если она еще не существует.</span><span class="sxs-lookup"><span data-stu-id="61eef-162">Give the dataset the name **M365JsonFile** and create new linked service if it does not exist already.</span></span>

    - <span data-ttu-id="61eef-163">В таблице выберите вкладку **Подключение,** а затем выберите **New**.</span><span class="sxs-lookup"><span data-stu-id="61eef-163">In the table select the **Connection** tab, then select **New**.</span></span>
    - <span data-ttu-id="61eef-164">Установите следующие значения в диалоговом окантове, а затем выберите **Finish**.</span><span class="sxs-lookup"><span data-stu-id="61eef-164">Set the following values in the dialog, then select **Finish**.</span></span>

        - <span data-ttu-id="61eef-165">**Метод проверки подлинности:** руководитель службы</span><span class="sxs-lookup"><span data-stu-id="61eef-165">**Authentication method**: Service principal</span></span>
        - <span data-ttu-id="61eef-166">**Подписка Azure:** выберите все</span><span class="sxs-lookup"><span data-stu-id="61eef-166">**Azure subscription**: Select all</span></span>
        - <span data-ttu-id="61eef-167">**служба хранилища учетной записи:** mgdcm365datastore</span><span class="sxs-lookup"><span data-stu-id="61eef-167">**Storage account name**: mgdcm365datastore</span></span>
          - <span data-ttu-id="61eef-168">Это учетная запись хранилища, созданная ранее в этом упражнении.</span><span class="sxs-lookup"><span data-stu-id="61eef-168">This is the storage account created earlier in this exercise.</span></span>
        - <span data-ttu-id="61eef-169">**Клиент:** введите ID клиента Azure</span><span class="sxs-lookup"><span data-stu-id="61eef-169">**Tenant**: enter the ID of your Azure tenant</span></span>
        - <span data-ttu-id="61eef-170">**Основной ID службы:** введите ID созданного ранее приложения Azure AD</span><span class="sxs-lookup"><span data-stu-id="61eef-170">**Service principal ID**: enter the ID of the Azure AD application you previously created</span></span>
        - <span data-ttu-id="61eef-171">**Основной ключ службы:** введите клавишу hashed приложения Azure AD, созданного ранее</span><span class="sxs-lookup"><span data-stu-id="61eef-171">**Service principal key**: enter the hashed key of the Azure AD application you previously created</span></span>

    - <span data-ttu-id="61eef-172">Рядом с **полем Путь к файлу** выберите **Просмотр**.</span><span class="sxs-lookup"><span data-stu-id="61eef-172">Next to the **File path** field, select **Browse**.</span></span>
    - <span data-ttu-id="61eef-173">Выберите имя созданного ранее контейнера хранения.</span><span class="sxs-lookup"><span data-stu-id="61eef-173">Select the name of the storage container you created previously.</span></span>

      ![Снимок экрана, на котором показан пользовательский интерфейс портала Azure для службы фабрики данных.](images/data-connect-adf-sa-fp-config.png)

1. <span data-ttu-id="61eef-176">Создав конвейер, выберите кнопку **Проверка всех** в верхней части конструктора.</span><span class="sxs-lookup"><span data-stu-id="61eef-176">With the pipeline created, select the **Validate All** button at the top of the designer.</span></span>

1. <span data-ttu-id="61eef-177">После проверки (и устранения всех найденных проблем) выберите кнопку **Опубликовать** все в верхней части конструктора.</span><span class="sxs-lookup"><span data-stu-id="61eef-177">After validating (and fixing any issues that were found), select the **Publish All** button at the top of the designer.</span></span>

## <a name="run-the-azure-data-factory-pipeline"></a><span data-ttu-id="61eef-178">Запуск конвейера фабрики данных Azure</span><span class="sxs-lookup"><span data-stu-id="61eef-178">Run the Azure Data Factory Pipeline</span></span>

<span data-ttu-id="61eef-179">С помощью созданного конвейера пришло время запустить его.</span><span class="sxs-lookup"><span data-stu-id="61eef-179">With the pipeline created, now it is time to run it.</span></span>

> [!NOTE]
> <span data-ttu-id="61eef-180">Для появления запроса на согласие может занять несколько минут, и для всего процесса (запуска, запроса согласия и утверждения согласия, завершаемого запуском конвейера) требуется более 40 минут.</span><span class="sxs-lookup"><span data-stu-id="61eef-180">It can take several minutes for the consent request to appear and it is not uncommon for the entire process (start, requesting consent and after approving the consent completing the pipeline run) to take over 40 minutes.</span></span>

1. <span data-ttu-id="61eef-181">В конструкторе Фабрики данных Azure с открытым конвейером выберите **добавить триггер**> Trigger Now .</span><span class="sxs-lookup"><span data-stu-id="61eef-181">In the Azure Data Factory designer, with the pipeline open, select **Add trigger > Trigger Now**.</span></span>

    ![Снимок экрана, показывающий пользовательский интерфейс портала Azure для службы Фабрика данных, чтобы показать, как активировать триггер в конвейере.](images/data-connect-adf-run-trigger.png)

1. <span data-ttu-id="61eef-183">После запуска задания из меню боковой панели выберите **Монитор,** чтобы просмотреть текущие запущенные задания.</span><span class="sxs-lookup"><span data-stu-id="61eef-183">After starting the job, from the sidebar menu, select **Monitor** to view current running jobs.</span></span>

1. <span data-ttu-id="61eef-184">На панели навигации слева найдите вкладку **Запуск конвейера** и выберите ее.</span><span class="sxs-lookup"><span data-stu-id="61eef-184">On the left-side navigation bar, locate the **Pipeline runs** tab and select it.</span></span> <span data-ttu-id="61eef-185">Выберите конвейер в столбце **Имя конвейера,** чтобы просмотреть **выполняется действие.**</span><span class="sxs-lookup"><span data-stu-id="61eef-185">Select the pipeline under the **Pipeline name** column to view the **Activity runs**.</span></span> <span data-ttu-id="61eef-186">Этот конвейер будет показываться в _процессе выполнения_.</span><span class="sxs-lookup"><span data-stu-id="61eef-186">This pipeline will show as _In progress_.</span></span>

    ![Снимок экрана, на котором показан пользовательский интерфейс портала Azure для фабрики данных, показан список запусков конвейера.](images/data-connect-adf-pipeline-runs.png)

1. <span data-ttu-id="61eef-188">После просмотра **выполняется действие,** перейдите в раздел _Действия выполняется,_ который расположен в нижней части страницы.</span><span class="sxs-lookup"><span data-stu-id="61eef-188">After you are in the **Activity runs** view, go to the _Activity runs_ section, which is located in the bottom side of the page.</span></span>

1. <span data-ttu-id="61eef-189">Наведите **курсор над именем Activity** и выберите параметр Googles.</span><span class="sxs-lookup"><span data-stu-id="61eef-189">Hover over the **Activity name** and select the googles option.</span></span> <span data-ttu-id="61eef-190">В этом случае будет приведена **вкладка Details.**</span><span class="sxs-lookup"><span data-stu-id="61eef-190">This will bring up the **Details** tab.</span></span>

    ![Снимок экрана, на котором показан пользовательский интерфейс Azure Portal для работы фабрики данных, пользователь выбирает googles в имени действия, чтобы открыть вкладку сведений.](images/data-connect-adf-pipeline-details.png)

1. <span data-ttu-id="61eef-192">На экране **Details** посмотрите на состояние действия конвейера, как посветилось на следующем изображении.</span><span class="sxs-lookup"><span data-stu-id="61eef-192">In the **Details** screen, look for the status of the pipeline activity as highlighted in the following image.</span></span> <span data-ttu-id="61eef-193">В этом случае вы можете увидеть, что он находится в состоянии **RequestingConsent**.</span><span class="sxs-lookup"><span data-stu-id="61eef-193">In this case you can see it is in a state of **RequestingConsent**.</span></span>

    ![Снимок экрана, на котором показан пользовательский интерфейс портала Azure для службы Фабрика данных, где состояние нагрузки запроса установлено на "RequestingConsent".](images/data-connect-adf-wait-for-approval.png)

1. <span data-ttu-id="61eef-195">На этом этапе запуск действий будет внутренне приостановлен, пока кто-то вручную не утвердит запрос на согласие через центр администрирования Microsoft 365 или через PowerShell.</span><span class="sxs-lookup"><span data-stu-id="61eef-195">At this point, the activity run is internally paused until someone manually approves the consent request via the Microsoft 365 admin center or via PowerShell.</span></span>
