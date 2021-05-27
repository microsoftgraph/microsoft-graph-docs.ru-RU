<!-- markdownlint-disable MD002 MD025 MD041 -->

<span data-ttu-id="3cca9-101">Создайте вертикали поиска и типы результатов для настройки результатов поиска в Microsoft SharePoint, Microsoft Office и Microsoft Search в Bing, чтобы пользователям было проще находить сведения, которые они могут видеть.</span><span class="sxs-lookup"><span data-stu-id="3cca9-101">Create search verticals and result types to customize the search results in Microsoft SharePoint, Microsoft Office, and Microsoft Search in Bing, to make it easier for users to find the information that they have permission to see.</span></span>

## <a name="create-a-vertical"></a><span data-ttu-id="3cca9-102">Создание вертикали</span><span class="sxs-lookup"><span data-stu-id="3cca9-102">Create a vertical</span></span>

<span data-ttu-id="3cca9-103">Чтобы создать и включить вертикаль поиска на [](https://admin.microsoft.com/) уровне организации, вопишитесь в центр администрирования Microsoft 365 с помощью роли глобального администратора и сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="3cca9-103">To create and enable a search vertical at the organization level, sign in to the [Microsoft 365 Admin center](https://admin.microsoft.com/) using the global administrator role, and do the following:</span></span>

1. <span data-ttu-id="3cca9-104">Перейдите **Параметры**  >  **поиск &**  >  **настройки.**</span><span class="sxs-lookup"><span data-stu-id="3cca9-104">Go to **Settings** > **Search & intelligence** > **Customizations**.</span></span>
2. <span data-ttu-id="3cca9-105">Перейдите **в Vertical** и нажмите **кнопку Добавить.**</span><span class="sxs-lookup"><span data-stu-id="3cca9-105">Go to **Vertical** and click the **Add** button.</span></span>
3. <span data-ttu-id="3cca9-106">Укай следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="3cca9-106">Provide the following details:</span></span>
  * <span data-ttu-id="3cca9-107">**Назови вертикаль:** Части прибора.</span><span class="sxs-lookup"><span data-stu-id="3cca9-107">**Name the vertical:** Appliance Parts.</span></span>

   ![Снимок экрана раздела "Имя вертикали"](images/connectors-images/build11.png)

  * <span data-ttu-id="3cca9-109">**Источник контента.** Соединитектор, созданный с помощью приложения.</span><span class="sxs-lookup"><span data-stu-id="3cca9-109">**Content source**: The connector created with the app.</span></span> <span data-ttu-id="3cca9-110">(Запас частей)</span><span class="sxs-lookup"><span data-stu-id="3cca9-110">(Parts Inventory)</span></span>

   ![Снимок экрана раздела "Источник контента"](images/connectors-images/build12.png)

  * <span data-ttu-id="3cca9-112">**Добавление запроса.** Оставьте пустым.</span><span class="sxs-lookup"><span data-stu-id="3cca9-112">**Add a query**: Leave blank.</span></span>

   ![Снимок экрана раздела "Добавление запроса"](images/connectors-images/build13.png)

  * <span data-ttu-id="3cca9-114">**Фильтры.** Оставьте пустым.</span><span class="sxs-lookup"><span data-stu-id="3cca9-114">**Filters**: Leave blank.</span></span>

   ![Снимок экрана раздела "Фильтры"](images/connectors-images/build14.png)

## <a name="create-a-result-type"></a><span data-ttu-id="3cca9-116">Создание типа результатов</span><span class="sxs-lookup"><span data-stu-id="3cca9-116">Create a result type</span></span>

<span data-ttu-id="3cca9-117">Чтобы создать тип результатов:</span><span class="sxs-lookup"><span data-stu-id="3cca9-117">To create a result type:</span></span>

1. <span data-ttu-id="3cca9-118">Перейдите **Параметры**  >  **поиск &**  >  **настройки.**</span><span class="sxs-lookup"><span data-stu-id="3cca9-118">Go to **Settings** > **Search & intelligence** > **Customizations**.</span></span>
2. <span data-ttu-id="3cca9-119">Перейдите на **вкладку типа результатов** и нажмите **кнопку Добавить.**</span><span class="sxs-lookup"><span data-stu-id="3cca9-119">Go to the **result type** tab and click the **Add** button.</span></span>
3. <span data-ttu-id="3cca9-120">Укай следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="3cca9-120">Provide the following details:</span></span>

  * <span data-ttu-id="3cca9-121">**Имя:** Часть прибора</span><span class="sxs-lookup"><span data-stu-id="3cca9-121">**Name**: Appliance Part</span></span>

   ![Снимок экрана раздела "Имя типа результата"](images/connectors-images/build15.png)

  * <span data-ttu-id="3cca9-123">**Источник контента.** Соединитектор, созданный в приложении.</span><span class="sxs-lookup"><span data-stu-id="3cca9-123">**Content source**: The connector created in the app.</span></span>

   ![Снимок экрана раздела "Выбор источника контента"](images/connectors-images/build16.png)

  * <span data-ttu-id="3cca9-125">**Правила**: Нет</span><span class="sxs-lookup"><span data-stu-id="3cca9-125">**Rules**: None</span></span>

   ![Снимок экрана раздела "Набор правил"](images/connectors-images/build17.png)

  * <span data-ttu-id="3cca9-127">Вклеить содержимое [result-type.jsв](https://github.com/microsoftgraph/msgraph-search-connector-sample/blob/master/result-type.json) текстовый ящик конструктора макета.</span><span class="sxs-lookup"><span data-stu-id="3cca9-127">Paste contents of [result-type.json](https://github.com/microsoftgraph/msgraph-search-connector-sample/blob/master/result-type.json) into the layout designer textbox.</span></span>

   ![Снимок экрана раздела "Макет дизайна"](images/connectors-images/build18.png)
