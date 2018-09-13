# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="0b17e-101">Тип ресурса fileSecurityState</span><span class="sxs-lookup"><span data-stu-id="0b17e-101">fileSecurityState resource type</span></span>

<span data-ttu-id="0b17e-102">Содержит информацию о файле (не процессе), связанную с оповещением.</span><span class="sxs-lookup"><span data-stu-id="0b17e-102">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="0b17e-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="0b17e-103">Properties</span></span>

| <span data-ttu-id="0b17e-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b17e-104">Property</span></span>   | <span data-ttu-id="0b17e-105">Тип</span><span class="sxs-lookup"><span data-stu-id="0b17e-105">Type</span></span>|<span data-ttu-id="0b17e-106">Описание</span><span class="sxs-lookup"><span data-stu-id="0b17e-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b17e-107">fileHash</span><span class="sxs-lookup"><span data-stu-id="0b17e-107">fileHash</span></span>|[<span data-ttu-id="0b17e-108">fileHash</span><span class="sxs-lookup"><span data-stu-id="0b17e-108">fileHash</span></span>](filehash.md)|<span data-ttu-id="0b17e-109">Сложный тип, содержащий хэши файлов (криптографические и чувствительные к расположению).</span><span class="sxs-lookup"><span data-stu-id="0b17e-109">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="0b17e-110">name</span><span class="sxs-lookup"><span data-stu-id="0b17e-110">name</span></span>|<span data-ttu-id="0b17e-111">String</span><span class="sxs-lookup"><span data-stu-id="0b17e-111">String</span></span>|<span data-ttu-id="0b17e-112">Имя файла (без пути).</span><span class="sxs-lookup"><span data-stu-id="0b17e-112">File name (without path).</span></span>|
|<span data-ttu-id="0b17e-113">path</span><span class="sxs-lookup"><span data-stu-id="0b17e-113">path</span></span>|<span data-ttu-id="0b17e-114">String</span><span class="sxs-lookup"><span data-stu-id="0b17e-114">String</span></span>|<span data-ttu-id="0b17e-115">Полный путь к файлу или объекту imageFile.</span><span class="sxs-lookup"><span data-stu-id="0b17e-115">Full file path of the stencil file</span></span>|
|<span data-ttu-id="0b17e-116">riskScore</span><span class="sxs-lookup"><span data-stu-id="0b17e-116">riskScore</span></span>|<span data-ttu-id="0b17e-117">String</span><span class="sxs-lookup"><span data-stu-id="0b17e-117">String</span></span>|<span data-ttu-id="0b17e-118">Сгенерированная/расчитанная поставщиком оценка риска для файла оповещений.</span><span class="sxs-lookup"><span data-stu-id="0b17e-118">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="0b17e-119">Рекомендуемый диапазон значений: от 0 до 1, что соответствует величине в процентах.</span><span class="sxs-lookup"><span data-stu-id="0b17e-119">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b17e-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0b17e-120">JSON representation</span></span>

<span data-ttu-id="0b17e-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b17e-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileSecurityState"
}-->

```json
{
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "name": "String",
  "path": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->