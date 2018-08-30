# <a name="publicationfacet-resource-type"></a><span data-ttu-id="b523a-101">Тип ресурса publicationFacet</span><span class="sxs-lookup"><span data-stu-id="b523a-101">PublicationFacet resource type</span></span>

<span data-ttu-id="b523a-102">Ресурс **publicationFacet** содержит сведения о состоянии публикации ресурса [driveItemVersion](driveitemversion.md) или [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="b523a-102">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b523a-103">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b523a-103">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.publicationFacet"
}-->

```json
{
  "level": "published | checkout",
  "versionId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="b523a-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="b523a-104">Properties</span></span>

|   <span data-ttu-id="b523a-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="b523a-105">Property</span></span>    |  <span data-ttu-id="b523a-106">Тип</span><span class="sxs-lookup"><span data-stu-id="b523a-106">Type</span></span>  | <span data-ttu-id="b523a-107">Описание</span><span class="sxs-lookup"><span data-stu-id="b523a-107">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="b523a-108">**level**</span><span class="sxs-lookup"><span data-stu-id="b523a-108">**level**</span></span>     | <span data-ttu-id="b523a-109">Cтрока</span><span class="sxs-lookup"><span data-stu-id="b523a-109">String</span></span> | <span data-ttu-id="b523a-110">Состояние публикации для данного документа.</span><span class="sxs-lookup"><span data-stu-id="b523a-110">The state of publication for this document.</span></span> <span data-ttu-id="b523a-111">Возможные значения: `published` или `checkout`.</span><span class="sxs-lookup"><span data-stu-id="b523a-111">Either `published` or `checkout`.</span></span> <span data-ttu-id="b523a-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b523a-112">Read-only.</span></span>  |
| <span data-ttu-id="b523a-113">**versionId**</span><span class="sxs-lookup"><span data-stu-id="b523a-113">**versionId**</span></span> | <span data-ttu-id="b523a-114">Cтрока</span><span class="sxs-lookup"><span data-stu-id="b523a-114">String</span></span> | <span data-ttu-id="b523a-115">Уникальный идентификатор для версии, отображаемый для текущего вызывающего объекта.</span><span class="sxs-lookup"><span data-stu-id="b523a-115">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="b523a-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b523a-116">Read-only.</span></span>  |


<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "suppressions": [
    " Warning: /api-reference/v1.0/resources/publicationfacet.md:
      Found potential enums in resource example that weren't defined in a table:(published,checkout) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Photo"
} -->
