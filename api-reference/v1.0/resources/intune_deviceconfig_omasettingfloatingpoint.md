# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="c5a15-101">Тип ресурса omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="c5a15-101">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="c5a15-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c5a15-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5a15-103">Определение плавающей запятой параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="c5a15-103">OMA Settings Floating Point definition.</span></span>

<span data-ttu-id="c5a15-104">Наследуется от ресурса [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c5a15-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c5a15-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c5a15-105">Properties</span></span>
|<span data-ttu-id="c5a15-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5a15-106">Property</span></span>|<span data-ttu-id="c5a15-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c5a15-107">Type</span></span>|<span data-ttu-id="c5a15-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c5a15-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5a15-109">displayName</span><span class="sxs-lookup"><span data-stu-id="c5a15-109">displayName</span></span>|<span data-ttu-id="c5a15-110">String (строка)</span><span class="sxs-lookup"><span data-stu-id="c5a15-110">String</span></span>|<span data-ttu-id="c5a15-111">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="c5a15-111">Display Name.</span></span> <span data-ttu-id="c5a15-112">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c5a15-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="c5a15-113">description</span><span class="sxs-lookup"><span data-stu-id="c5a15-113">description</span></span>|<span data-ttu-id="c5a15-114">String (строка)</span><span class="sxs-lookup"><span data-stu-id="c5a15-114">String</span></span>|<span data-ttu-id="c5a15-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="c5a15-115">Description.</span></span> <span data-ttu-id="c5a15-116">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c5a15-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="c5a15-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="c5a15-117">omaUri</span></span>|<span data-ttu-id="c5a15-118">String (строка)</span><span class="sxs-lookup"><span data-stu-id="c5a15-118">String</span></span>|<span data-ttu-id="c5a15-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="c5a15-119">OMA.</span></span> <span data-ttu-id="c5a15-120">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c5a15-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="c5a15-121">value</span><span class="sxs-lookup"><span data-stu-id="c5a15-121">value</span></span>|<span data-ttu-id="c5a15-122">Single</span><span class="sxs-lookup"><span data-stu-id="c5a15-122">Single</span></span>|<span data-ttu-id="c5a15-123">Значение.</span><span class="sxs-lookup"><span data-stu-id="c5a15-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5a15-124">Связи</span><span class="sxs-lookup"><span data-stu-id="c5a15-124">Relationships</span></span>
<span data-ttu-id="c5a15-125">Нет</span><span class="sxs-lookup"><span data-stu-id="c5a15-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c5a15-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c5a15-126">JSON Representation</span></span>
<span data-ttu-id="c5a15-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5a15-127">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.omaSetting",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1.5
}
```



