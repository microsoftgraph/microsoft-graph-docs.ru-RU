# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="fa9c8-101">Тип ресурса omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="fa9c8-101">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="fa9c8-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fa9c8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa9c8-103">Определение плавающей запятой параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="fa9c8-103">OMA Settings Floating Point definition.</span></span>

<span data-ttu-id="fa9c8-104">Наследуется от ресурса [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fa9c8-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fa9c8-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa9c8-105">Properties</span></span>
|<span data-ttu-id="fa9c8-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa9c8-106">Property</span></span>|<span data-ttu-id="fa9c8-107">Тип</span><span class="sxs-lookup"><span data-stu-id="fa9c8-107">Type</span></span>|<span data-ttu-id="fa9c8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fa9c8-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa9c8-109">displayName</span><span class="sxs-lookup"><span data-stu-id="fa9c8-109">displayName</span></span>|<span data-ttu-id="fa9c8-110">String (строка)</span><span class="sxs-lookup"><span data-stu-id="fa9c8-110">String</span></span>|<span data-ttu-id="fa9c8-111">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="fa9c8-111">Display Name.</span></span> <span data-ttu-id="fa9c8-112">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fa9c8-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="fa9c8-113">описание</span><span class="sxs-lookup"><span data-stu-id="fa9c8-113">description</span></span>|<span data-ttu-id="fa9c8-114">String (строка)</span><span class="sxs-lookup"><span data-stu-id="fa9c8-114">String</span></span>|<span data-ttu-id="fa9c8-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="fa9c8-115">Description.</span></span> <span data-ttu-id="fa9c8-116">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fa9c8-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="fa9c8-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="fa9c8-117">omaUri</span></span>|<span data-ttu-id="fa9c8-118">String (строка)</span><span class="sxs-lookup"><span data-stu-id="fa9c8-118">String</span></span>|<span data-ttu-id="fa9c8-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="fa9c8-119">OMA.</span></span> <span data-ttu-id="fa9c8-120">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fa9c8-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="fa9c8-121">value</span><span class="sxs-lookup"><span data-stu-id="fa9c8-121">value</span></span>|<span data-ttu-id="fa9c8-122">Single</span><span class="sxs-lookup"><span data-stu-id="fa9c8-122">Single</span></span>|<span data-ttu-id="fa9c8-123">Значение.</span><span class="sxs-lookup"><span data-stu-id="fa9c8-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa9c8-124">Связи</span><span class="sxs-lookup"><span data-stu-id="fa9c8-124">Relationships</span></span>
<span data-ttu-id="fa9c8-125">Нет</span><span class="sxs-lookup"><span data-stu-id="fa9c8-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fa9c8-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fa9c8-126">JSON Representation</span></span>
<span data-ttu-id="fa9c8-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa9c8-127">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```








