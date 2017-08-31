# <a name="hashes-resource-type"></a><span data-ttu-id="c8db5-101">Тип ресурса хэшей</span><span class="sxs-lookup"><span data-stu-id="c8db5-101">Hashes resource type</span></span>

<span data-ttu-id="c8db5-102">Ресурс **хэшей** группирует доступных хэши в единую структуру для элемента.</span><span class="sxs-lookup"><span data-stu-id="c8db5-102">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="c8db5-103">**Примечание.** Не все службы предоставляют значение для всех свойств хэша в списке.</span><span class="sxs-lookup"><span data-stu-id="c8db5-103">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8db5-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c8db5-104">JSON representation</span></span>

<span data-ttu-id="c8db5-105">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8db5-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "sha1Hash", "crc32Hash", "quickXorHash" ],
  "@odata.type": "microsoft.graph.hashes"
}-->

```json
{
  "crc32Hash": "string",
  "sha1Hash": "string",
  "quickXorHash": "string"
}
```


## <a name="properties"></a><span data-ttu-id="c8db5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c8db5-106">Properties</span></span>

| <span data-ttu-id="c8db5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8db5-107">Property</span></span>         | <span data-ttu-id="c8db5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c8db5-108">Type</span></span>   | <span data-ttu-id="c8db5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c8db5-109">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="c8db5-110">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="c8db5-110">**sha1Hash**</span></span>     | <span data-ttu-id="c8db5-111">String</span><span class="sxs-lookup"><span data-stu-id="c8db5-111">String</span></span> | <span data-ttu-id="c8db5-p101">Хэш SHA1 для содержимого файла (если доступно). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8db5-p101">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="c8db5-114">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="c8db5-114">**crc32Hash**</span></span>    | <span data-ttu-id="c8db5-115">String</span><span class="sxs-lookup"><span data-stu-id="c8db5-115">String</span></span> | <span data-ttu-id="c8db5-p102">Значение CRC32 файла (если доступно). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8db5-p102">The CRC32 value of the file (if available). Read-only.</span></span>            |
| <span data-ttu-id="c8db5-118">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="c8db5-118">**quickXorHash**</span></span> | <span data-ttu-id="c8db5-119">String</span><span class="sxs-lookup"><span data-stu-id="c8db5-119">String</span></span> | <span data-ttu-id="c8db5-p103">Особый хэш файла, который можно использовать, чтобы определить, было ли изменено содержимое файла (если доступно). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8db5-p103">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="c8db5-p104">**Примечание.** В некоторых случаях значения хэша могут быть недоступны. Если это так, значения хэша для определенного элемента будут обновлены после загрузки элемента.</span><span class="sxs-lookup"><span data-stu-id="c8db5-p104">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>


## <a name="remarks"></a><span data-ttu-id="c8db5-124">Заметки</span><span class="sxs-lookup"><span data-stu-id="c8db5-124">Remarks</span></span>

<span data-ttu-id="c8db5-p105">В OneDrive для бизнеса хэши **sha1Hash** и **crc32Hash** недоступны. В OneDrive персональный хэш **quickXorHash** недоступен.</span><span class="sxs-lookup"><span data-stu-id="c8db5-p105">In OneDrive for Business, **sha1Hash** and **crc32Hash** are not available. In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="c8db5-127">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="c8db5-127">For more information about the facets on a [driveItem](driveitem.md), see driveItem.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hashes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
