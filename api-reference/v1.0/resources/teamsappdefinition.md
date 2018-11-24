# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="7963c-101">Тип ресурса teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="7963c-101">teamsAppDefinition resource type</span></span>



<span data-ttu-id="7963c-102">Подробные сведения о одной версии [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="7963c-102">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7963c-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="7963c-103">Properties</span></span>

| <span data-ttu-id="7963c-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="7963c-104">Property</span></span>            | <span data-ttu-id="7963c-105">Тип</span><span class="sxs-lookup"><span data-stu-id="7963c-105">Type</span></span>     | <span data-ttu-id="7963c-106">Описание</span><span class="sxs-lookup"><span data-stu-id="7963c-106">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="7963c-107">id</span><span class="sxs-lookup"><span data-stu-id="7963c-107">id</span></span>                  | <span data-ttu-id="7963c-108">строка</span><span class="sxs-lookup"><span data-stu-id="7963c-108">string</span></span>   | <span data-ttu-id="7963c-109">Уникальный идентификатор (не appid команды).</span><span class="sxs-lookup"><span data-stu-id="7963c-109">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="7963c-110">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="7963c-110">teamsAppId</span></span>          | <span data-ttu-id="7963c-111">string</span><span class="sxs-lookup"><span data-stu-id="7963c-111">string</span></span>   | <span data-ttu-id="7963c-112">Идентификатор в манифесте приложения группы.</span><span class="sxs-lookup"><span data-stu-id="7963c-112">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="7963c-113">displayName</span><span class="sxs-lookup"><span data-stu-id="7963c-113">displayName</span></span>         | <span data-ttu-id="7963c-114">строка</span><span class="sxs-lookup"><span data-stu-id="7963c-114">string</span></span>   | <span data-ttu-id="7963c-115">Имя приложения, предоставляемый разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="7963c-115">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="7963c-116">version</span><span class="sxs-lookup"><span data-stu-id="7963c-116">version</span></span>             | <span data-ttu-id="7963c-117">string</span><span class="sxs-lookup"><span data-stu-id="7963c-117">string</span></span>   | <span data-ttu-id="7963c-118">Номер версии приложения.</span><span class="sxs-lookup"><span data-stu-id="7963c-118">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7963c-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7963c-119">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "teamsAppId": "string",
  "displayName": "Test App",
  "version": "1.0.0",
}
```

# <a name="see-also"></a><span data-ttu-id="7963c-120">См. также</span><span class="sxs-lookup"><span data-stu-id="7963c-120">See also</span></span>

- [<span data-ttu-id="7963c-121">teamsApp</span><span class="sxs-lookup"><span data-stu-id="7963c-121">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="7963c-122">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="7963c-122">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="7963c-123">teamsTab</span><span class="sxs-lookup"><span data-stu-id="7963c-123">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

