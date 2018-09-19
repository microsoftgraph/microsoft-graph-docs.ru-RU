# <a name="cloudappsecuritystate-resource-type"></a><span data-ttu-id="03506-101">тип ресурса cloudAppSecurityState</span><span class="sxs-lookup"><span data-stu-id="03506-101">cloudAppSecurityState resource type</span></span>

<span data-ttu-id="03506-102">Содержит информацию о состоянии облачного приложения (destinationServiceName, destinationServiceIp).</span><span class="sxs-lookup"><span data-stu-id="03506-102">Contains stateful information about the cloud application (destinationServiceName, destinationServiceIp).</span></span>

## <a name="properties"></a><span data-ttu-id="03506-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="03506-103">Properties</span></span>

| <span data-ttu-id="03506-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="03506-104">Property</span></span>     | <span data-ttu-id="03506-105">Тип</span><span class="sxs-lookup"><span data-stu-id="03506-105">Type</span></span>        | <span data-ttu-id="03506-106">Описание</span><span class="sxs-lookup"><span data-stu-id="03506-106">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="03506-107">destinationServiceIp</span><span class="sxs-lookup"><span data-stu-id="03506-107">destinationServiceIp</span></span>|<span data-ttu-id="03506-108">Строка</span><span class="sxs-lookup"><span data-stu-id="03506-108">String</span></span>|<span data-ttu-id="03506-109">Конечный IP-адрес подключения к облачному приложению / службе.</span><span class="sxs-lookup"><span data-stu-id="03506-109">Destination IP Address of the connection to the cloud application/service.</span></span>|
|<span data-ttu-id="03506-110">destinationServiceName</span><span class="sxs-lookup"><span data-stu-id="03506-110">destinationServiceName</span></span>|<span data-ttu-id="03506-111">Строка</span><span class="sxs-lookup"><span data-stu-id="03506-111">String</span></span>|<span data-ttu-id="03506-112">Имя облачного приложения / службы (например «Salesforce», «DropBox» и т.д.).</span><span class="sxs-lookup"><span data-stu-id="03506-112">Cloud application/service name (for example "Salesforce", "DropBox", etc.).</span></span>|
|<span data-ttu-id="03506-113">riskScore</span><span class="sxs-lookup"><span data-stu-id="03506-113">riskScore</span></span>|<span data-ttu-id="03506-114">Строка</span><span class="sxs-lookup"><span data-stu-id="03506-114">String</span></span>|<span data-ttu-id="03506-115">Указанная поставщиком / рассчитанная оценка рисков для облачного приложения / службы.</span><span class="sxs-lookup"><span data-stu-id="03506-115">Provider-generated/calculated risk score of the Cloud Application/Service.</span></span> <span data-ttu-id="03506-116">Рекомендуемый диапазон значений: от 0 до 1, что соответствует величине в процентах.</span><span class="sxs-lookup"><span data-stu-id="03506-116">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="03506-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="03506-117">JSON representation</span></span>

<span data-ttu-id="03506-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03506-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecurityState"
}-->

```json
{
  "destinationServiceIp": "String",
  "destinationServiceName": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->