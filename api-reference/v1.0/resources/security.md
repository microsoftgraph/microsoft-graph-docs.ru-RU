# <a name="security-resource-type"></a><span data-ttu-id="76350-101">тип ресурса безопасности</span><span class="sxs-lookup"><span data-stu-id="76350-101">security resource type</span></span>

<span data-ttu-id="76350-102">Ресурс безопасности — это точка входа для объектной модели Security.</span><span class="sxs-lookup"><span data-stu-id="76350-102">The security resource is the entry point for the Security object model.</span></span> <span data-ttu-id="76350-103">Она выводит одноэлементный ресурс безопасности.</span><span class="sxs-lookup"><span data-stu-id="76350-103">It returns a singleton security resource.</span></span> <span data-ttu-id="76350-104">Не содержит свойства, которые можно использовать.</span><span class="sxs-lookup"><span data-stu-id="76350-104">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="76350-105">Методы</span><span class="sxs-lookup"><span data-stu-id="76350-105">Methods</span></span>

| <span data-ttu-id="76350-106">Метод</span><span class="sxs-lookup"><span data-stu-id="76350-106">Method</span></span>       | <span data-ttu-id="76350-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="76350-107">Return Type</span></span> | <span data-ttu-id="76350-108">Описание</span><span class="sxs-lookup"><span data-stu-id="76350-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="76350-109">|||UNTRANSLATED_CONTENT_START|||List alerts|||UNTRANSLATED_CONTENT_END|||</span><span class="sxs-lookup"><span data-stu-id="76350-109">List alerts</span></span>](../api/alert_list.md) | <span data-ttu-id="76350-110">коллекция [alert](alert.md)</span><span class="sxs-lookup"><span data-stu-id="76350-110">[alert](alert.md) collection</span></span> | <span data-ttu-id="76350-111">Получение коллекции объектов alert.</span><span class="sxs-lookup"><span data-stu-id="76350-111">Get a licenseDetails object collection.</span></span> |
| [<span data-ttu-id="76350-112">получить оповещения</span><span class="sxs-lookup"><span data-stu-id="76350-112">get alerts</span></span>](../api/alert_get.md) | <span data-ttu-id="76350-113">коллекция [alert](alert.md)</span><span class="sxs-lookup"><span data-stu-id="76350-113">[alert](alert.md) collection</span></span> | <span data-ttu-id="76350-114">Получить объект alert.</span><span class="sxs-lookup"><span data-stu-id="76350-114">Get a alert object.</span></span> |
| [<span data-ttu-id="76350-115">Обновление оповещений</span><span class="sxs-lookup"><span data-stu-id="76350-115">Update alerts</span></span>](../api/alert_update.md) | <span data-ttu-id="76350-116">коллекция [alert](alert.md)</span><span class="sxs-lookup"><span data-stu-id="76350-116">[alert](alert.md) collection</span></span> | <span data-ttu-id="76350-117">Получить объект alert.</span><span class="sxs-lookup"><span data-stu-id="76350-117">Get a alert object.</span></span> |

## <a name="properties"></a><span data-ttu-id="76350-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="76350-118">Properties</span></span>
<span data-ttu-id="76350-119">Нет</span><span class="sxs-lookup"><span data-stu-id="76350-119">None</span></span>

## <a name="relationships"></a><span data-ttu-id="76350-120">Связи</span><span class="sxs-lookup"><span data-stu-id="76350-120">Relationships</span></span>
| <span data-ttu-id="76350-121">Связь</span><span class="sxs-lookup"><span data-stu-id="76350-121">Relationship</span></span> | <span data-ttu-id="76350-122">Тип</span><span class="sxs-lookup"><span data-stu-id="76350-122">Type</span></span>        | <span data-ttu-id="76350-123">Описание</span><span class="sxs-lookup"><span data-stu-id="76350-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="76350-124">оповещения</span><span class="sxs-lookup"><span data-stu-id="76350-124">alerts</span></span>|<span data-ttu-id="76350-125">коллекция [alert](alert.md)</span><span class="sxs-lookup"><span data-stu-id="76350-125">[alert](alert.md) collection</span></span>| <span data-ttu-id="76350-p102">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="76350-p102">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="76350-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="76350-128">JSON representation</span></span>
<span data-ttu-id="76350-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76350-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="76350-130">Пример</span><span class="sxs-lookup"><span data-stu-id="76350-130">Example</span></span>

<span data-ttu-id="76350-131">Ресурс**безопасности** доступен в корневом каталоге Graph.</span><span class="sxs-lookup"><span data-stu-id="76350-131">The **security** resource is available at the root of the graph.</span></span>

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/security
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "security resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->