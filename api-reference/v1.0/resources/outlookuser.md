# <a name="outlookuser-resource-type"></a><span data-ttu-id="2a475-101">Тип ресурса outlookUser</span><span class="sxs-lookup"><span data-stu-id="2a475-101">outlookUser resource type</span></span>


<span data-ttu-id="2a475-102">Представляет службы Outlook, доступные пользователю.</span><span class="sxs-lookup"><span data-stu-id="2a475-102">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="2a475-103">Методы</span><span class="sxs-lookup"><span data-stu-id="2a475-103">Methods</span></span>

| <span data-ttu-id="2a475-104">Метод</span><span class="sxs-lookup"><span data-stu-id="2a475-104">Method</span></span>           | <span data-ttu-id="2a475-105">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2a475-105">Return Type</span></span>    |<span data-ttu-id="2a475-106">Описание</span><span class="sxs-lookup"><span data-stu-id="2a475-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2a475-107">Создание категории</span><span class="sxs-lookup"><span data-stu-id="2a475-107">Create category</span></span>](../api/outlookuser_post_mastercategories.md) | [<span data-ttu-id="2a475-108">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="2a475-108">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="2a475-109">Создание объекта **outlookCategory** в основном списке категорий пользователя.</span><span class="sxs-lookup"><span data-stu-id="2a475-109">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="2a475-110">Перечисление категорий</span><span class="sxs-lookup"><span data-stu-id="2a475-110">List categories</span></span>](../api/outlookuser_list_mastercategories.md) | <span data-ttu-id="2a475-111">Коллекция [outlookCategory](outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="2a475-111">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="2a475-112">Получение всех категорий, определенных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="2a475-112">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="2a475-113">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="2a475-113">supportedLanguages</span></span>](../api/outlookuser_supportedlanguages.md) | <span data-ttu-id="2a475-114">Коллекция [localeInfo](localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="2a475-114">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="2a475-115">Получение списка языковых стандартов и языков, который поддерживается для пользователя, в соответствии с настройкой на сервере почтовых ящиков этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="2a475-115">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="2a475-116">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="2a475-116">supportedTimeZones</span></span>](../api/outlookuser_supportedtimezones.md) | <span data-ttu-id="2a475-117">Коллекция [timeZoneInformation](timezoneinformation.md)</span><span class="sxs-lookup"><span data-stu-id="2a475-117">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="2a475-118">Получение списка часовых поясов, который поддерживается для пользователя, в соответствии с настройкой на сервере почтовых ящиков этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="2a475-118">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="2a475-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="2a475-119">Properties</span></span>
<span data-ttu-id="2a475-120">Нет</span><span class="sxs-lookup"><span data-stu-id="2a475-120">None</span></span>

## <a name="relationships"></a><span data-ttu-id="2a475-121">Связи</span><span class="sxs-lookup"><span data-stu-id="2a475-121">Relationships</span></span>
| <span data-ttu-id="2a475-122">Связь</span><span class="sxs-lookup"><span data-stu-id="2a475-122">Relationship</span></span> | <span data-ttu-id="2a475-123">Тип</span><span class="sxs-lookup"><span data-stu-id="2a475-123">Type</span></span>   |<span data-ttu-id="2a475-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2a475-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a475-125">masterCategories</span><span class="sxs-lookup"><span data-stu-id="2a475-125">masterCategories</span></span>|<span data-ttu-id="2a475-126">Коллекция [outlookCategory](../resources/outlookCategory.md)</span><span class="sxs-lookup"><span data-stu-id="2a475-126">[outlookCategory](../resources/outlookCategory.md) collection</span></span>| <span data-ttu-id="2a475-127">Список категорий, определенных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="2a475-127">A list of categories defined for the user.</span></span> | 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->