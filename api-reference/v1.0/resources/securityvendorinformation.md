# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="cfc10-101">Тип ресурса securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="cfc10-101">securityVendorInformation resource type</span></span>

<span data-ttu-id="cfc10-102">Содержит сведения о безопасности продуктов и услуг поставщика, поставщик и subprovider (например, поставщика = корпорации Майкрософт; поставщика = ATP Защитник Windows; subProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="cfc10-102">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="cfc10-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="cfc10-103">Properties</span></span>

| <span data-ttu-id="cfc10-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="cfc10-104">Property</span></span>   | <span data-ttu-id="cfc10-105">Тип</span><span class="sxs-lookup"><span data-stu-id="cfc10-105">Type</span></span>|<span data-ttu-id="cfc10-106">Описание</span><span class="sxs-lookup"><span data-stu-id="cfc10-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cfc10-107">Поставщик</span><span class="sxs-lookup"><span data-stu-id="cfc10-107">provider</span></span> |<span data-ttu-id="cfc10-108">String</span><span class="sxs-lookup"><span data-stu-id="cfc10-108">String</span></span>|<span data-ttu-id="cfc10-109">Определенного поставщика (продуктов и услуг - не поставщика организации); Например WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="cfc10-109">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="cfc10-110">providerVersion</span><span class="sxs-lookup"><span data-stu-id="cfc10-110">providerVersion</span></span>|<span data-ttu-id="cfc10-111">String</span><span class="sxs-lookup"><span data-stu-id="cfc10-111">String</span></span>|<span data-ttu-id="cfc10-112">Версия поставщика или subprovider, если он существует, создавшее оповещение.</span><span class="sxs-lookup"><span data-stu-id="cfc10-112">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="cfc10-113">*Required*</span><span class="sxs-lookup"><span data-stu-id="cfc10-113">*Required*</span></span>|
|<span data-ttu-id="cfc10-114">subProvider</span><span class="sxs-lookup"><span data-stu-id="cfc10-114">subProvider</span></span>|<span data-ttu-id="cfc10-115">String</span><span class="sxs-lookup"><span data-stu-id="cfc10-115">String</span></span>|<span data-ttu-id="cfc10-116">Определенные subprovider (в разделе статистической обработки поставщика); Например WindowsDefenderATP.SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="cfc10-116">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="cfc10-117">поставщика</span><span class="sxs-lookup"><span data-stu-id="cfc10-117">vendor</span></span> |<span data-ttu-id="cfc10-118">String</span><span class="sxs-lookup"><span data-stu-id="cfc10-118">String</span></span>|<span data-ttu-id="cfc10-119">Имя оповещения поставщика (например, Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="cfc10-119">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="cfc10-120">*Required*</span><span class="sxs-lookup"><span data-stu-id="cfc10-120">*Required*</span></span>|


## <a name="json-representation"></a><span data-ttu-id="cfc10-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cfc10-121">JSON representation</span></span>

<span data-ttu-id="cfc10-122">Соответствовать является представлением JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="cfc10-122">The folllowing is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityVendorInformation"
}-->

```json
{
  "provider": "String",
  "providerVersion": "String",
  "subProvider": "String",
  "vendor": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
