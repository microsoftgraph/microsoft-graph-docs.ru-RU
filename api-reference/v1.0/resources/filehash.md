# <a name="filehash-resource-type"></a><span data-ttu-id="23346-101">Тип ресурса fileHash</span><span class="sxs-lookup"><span data-stu-id="23346-101">fileHash resource type</span></span>

<span data-ttu-id="23346-102">Содержит информацию с отслеживанием состояния хэш-значений файлов (криптографических и чувствительных к расположению).</span><span class="sxs-lookup"><span data-stu-id="23346-102">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="23346-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="23346-103">Properties</span></span>

| <span data-ttu-id="23346-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="23346-104">Property</span></span>     | <span data-ttu-id="23346-105">Тип</span><span class="sxs-lookup"><span data-stu-id="23346-105">Type</span></span>        | <span data-ttu-id="23346-106">Описание</span><span class="sxs-lookup"><span data-stu-id="23346-106">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="23346-107">hashType</span><span class="sxs-lookup"><span data-stu-id="23346-107">hashType</span></span>|<span data-ttu-id="23346-108">fileHashType</span><span class="sxs-lookup"><span data-stu-id="23346-108">fileHashType</span></span>|<span data-ttu-id="23346-109">Тип хэш-функции файла.</span><span class="sxs-lookup"><span data-stu-id="23346-109">File hash type.</span></span> <span data-ttu-id="23346-110">Возможные значения: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span><span class="sxs-lookup"><span data-stu-id="23346-110">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="23346-111">hashValue</span><span class="sxs-lookup"><span data-stu-id="23346-111">hashValue</span></span>|<span data-ttu-id="23346-112">String</span><span class="sxs-lookup"><span data-stu-id="23346-112">String</span></span>|<span data-ttu-id="23346-113">Значение файлового хэша.</span><span class="sxs-lookup"><span data-stu-id="23346-113">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="23346-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="23346-114">JSON representation</span></span>

<span data-ttu-id="23346-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23346-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileHash"
}-->

```json
{
  "hashType": "@odata.type: microsoft.graph.fileHashType",
  "hashValue": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileHash resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->