# <a name="baseitemversion-resource-type"></a><span data-ttu-id="81555-101">Тип ресурса baseItemVersion</span><span class="sxs-lookup"><span data-stu-id="81555-101">BaseItemVersion resource type</span></span>

<span data-ttu-id="81555-102">Ресурс **baseItemVersion** представляет предыдущую версию элемента или записи.</span><span class="sxs-lookup"><span data-stu-id="81555-102">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="81555-103">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="81555-103">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.baseItemVersion",
  "@type.aka": "oneDrive.baseItemVersion"
}-->

```json
{
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="81555-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="81555-104">Properties</span></span>

|      <span data-ttu-id="81555-105">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="81555-105">Property name</span></span>       |                         <span data-ttu-id="81555-106">Тип</span><span class="sxs-lookup"><span data-stu-id="81555-106">Type</span></span>                         |                               <span data-ttu-id="81555-107">Описание</span><span class="sxs-lookup"><span data-stu-id="81555-107">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="81555-108">**id**</span><span class="sxs-lookup"><span data-stu-id="81555-108">**id**</span></span>                   | <span data-ttu-id="81555-109">string (строка)</span><span class="sxs-lookup"><span data-stu-id="81555-109">string</span></span>                                               | <span data-ttu-id="81555-110">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="81555-110">The ID of the version.</span></span> <span data-ttu-id="81555-111">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81555-111">Read-only.</span></span>                                       |
| <span data-ttu-id="81555-112">****lastModifiedBy**;**</span><span class="sxs-lookup"><span data-stu-id="81555-112">**lastModifiedBy**</span></span>       | [<span data-ttu-id="81555-113">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="81555-113">IdentitySet</span></span>](../resources/identitySet.md)           | <span data-ttu-id="81555-114">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="81555-114">Identity of the user which last modified the version.</span></span> <span data-ttu-id="81555-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81555-115">Read-only.</span></span>        |
| <span data-ttu-id="81555-116">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="81555-116">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="81555-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81555-117">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="81555-118">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="81555-118">Date and time the version was last modified.</span></span> <span data-ttu-id="81555-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81555-119">Read-only.</span></span>                 |
| <span data-ttu-id="81555-120">**publication**</span><span class="sxs-lookup"><span data-stu-id="81555-120">**publication**</span></span>          | [<span data-ttu-id="81555-121">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="81555-121">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="81555-122">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="81555-122">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="81555-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81555-123">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
