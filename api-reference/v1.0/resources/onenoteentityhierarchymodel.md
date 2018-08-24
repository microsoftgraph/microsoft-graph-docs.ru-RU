# <a name="onenoteentityhierarchymodel-resource"></a><span data-ttu-id="9a852-101">Ресурс onenoteEntityHierarchyModel</span><span class="sxs-lookup"><span data-stu-id="9a852-101">onenoteEntityHierarchyModel resource</span></span>

<span data-ttu-id="9a852-102">Это базовый тип для сущностей OneNote.</span><span class="sxs-lookup"><span data-stu-id="9a852-102">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a852-103">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9a852-103">JSON representation</span></span>

<span data-ttu-id="9a852-104">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a852-104">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.onenoteEntitySchemaObjectModel",
  "optionalProperties": [
    "self"
  ],
  "@odata.type": "microsoft.graph.onenoteEntityHierarchyModel"
}-->

```json
{
  "displayName": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="9a852-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9a852-105">Properties</span></span>
## <a name="properties"></a><span data-ttu-id="9a852-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9a852-106">Properties</span></span>
| <span data-ttu-id="9a852-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a852-107">Property</span></span>     | <span data-ttu-id="9a852-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9a852-108">Type</span></span>   |<span data-ttu-id="9a852-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9a852-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a852-110">displayName</span><span class="sxs-lookup"><span data-stu-id="9a852-110">displayName</span></span>|<span data-ttu-id="9a852-111">Строка</span><span class="sxs-lookup"><span data-stu-id="9a852-111">String</span></span>|<span data-ttu-id="9a852-112">Имя записной книжки.</span><span class="sxs-lookup"><span data-stu-id="9a852-112">The name of the notebook.</span></span>|
|<span data-ttu-id="9a852-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="9a852-113">createdBy</span></span>|[<span data-ttu-id="9a852-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="9a852-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="9a852-p101">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9a852-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="9a852-117">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="9a852-117">lastModifiedBy</span></span>|[<span data-ttu-id="9a852-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="9a852-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="9a852-p102">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9a852-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="9a852-121">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a852-121">lastModifiedDateTime</span></span>|<span data-ttu-id="9a852-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a852-122">DateTimeOffset</span></span>|<span data-ttu-id="9a852-p103">Дата и время последнего изменения записной книжки. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9a852-p103">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|

<!-- uuid: 8b1af557-1a7c-4432-86eb-94989c2d4b54
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->