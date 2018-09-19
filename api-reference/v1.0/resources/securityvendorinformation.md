# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="5acc5-101">Тип ресурса securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="5acc5-101">securityVendorInformation resource type</span></span>

<span data-ttu-id="5acc5-102">Содержит сведения о безопасности продуктов и услуг производителя, поставщика и субпоставщика (например, производитель=Майкрософт; поставщик=ATP Защитник Windows; субпоставщик=AppLocker).</span><span class="sxs-lookup"><span data-stu-id="5acc5-102">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="5acc5-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="5acc5-103">Properties</span></span>

| <span data-ttu-id="5acc5-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="5acc5-104">Property</span></span>   | <span data-ttu-id="5acc5-105">Тип</span><span class="sxs-lookup"><span data-stu-id="5acc5-105">Type</span></span>|<span data-ttu-id="5acc5-106">Описание</span><span class="sxs-lookup"><span data-stu-id="5acc5-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5acc5-107">provider \*</span><span class="sxs-lookup"><span data-stu-id="5acc5-107">provider \*</span></span>|<span data-ttu-id="5acc5-108">String</span><span class="sxs-lookup"><span data-stu-id="5acc5-108">String</span></span>|<span data-ttu-id="5acc5-109">Определенный поставщик (продуктов/услуг - не организация-производитель); например, WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="5acc5-109">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="5acc5-110">providerVersion</span><span class="sxs-lookup"><span data-stu-id="5acc5-110">providerVersion</span></span>|<span data-ttu-id="5acc5-111">String</span><span class="sxs-lookup"><span data-stu-id="5acc5-111">String</span></span>|<span data-ttu-id="5acc5-112">Версия поставщика или субпоставщика (при наличии), которая создала оповещение.</span><span class="sxs-lookup"><span data-stu-id="5acc5-112">Version of the provider or subprovider, if it exists, that generated the alert.</span></span>|
|<span data-ttu-id="5acc5-113">subProvider</span><span class="sxs-lookup"><span data-stu-id="5acc5-113">subProvider</span></span>|<span data-ttu-id="5acc5-114">String</span><span class="sxs-lookup"><span data-stu-id="5acc5-114">String</span></span>|<span data-ttu-id="5acc5-115">Определенный субпоставщик (в разделе статистической обработки поставщика); например, WindowsDefenderATP.SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="5acc5-115">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="5acc5-116">vendor \*</span><span class="sxs-lookup"><span data-stu-id="5acc5-116">vendor \*</span></span>|<span data-ttu-id="5acc5-117">String</span><span class="sxs-lookup"><span data-stu-id="5acc5-117">String</span></span>|<span data-ttu-id="5acc5-118">Имя оповещения производителя (например, Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="5acc5-118">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span>|
<span data-ttu-id="5acc5-119">(\* указывает на обязательный характер.)</span><span class="sxs-lookup"><span data-stu-id="5acc5-119">(\* Indicates a mandatory field.)</span></span>

## <a name="json-representation"></a><span data-ttu-id="5acc5-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5acc5-120">JSON representation</span></span>

<span data-ttu-id="5acc5-121">Далее отображено представление ресурса JSON.</span><span class="sxs-lookup"><span data-stu-id="5acc5-121">The following is a JSON representation of the resource.</span></span>
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
