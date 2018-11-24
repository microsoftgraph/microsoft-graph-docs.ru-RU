# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="45a53-101">Тип ресурса omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="45a53-101">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="45a53-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="45a53-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45a53-103">Определение плавающей запятой параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="45a53-103">OMA Settings Floating Point definition.</span></span>

<span data-ttu-id="45a53-104">Наследуется от ресурса [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="45a53-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="45a53-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="45a53-105">Properties</span></span>
|<span data-ttu-id="45a53-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="45a53-106">Property</span></span>|<span data-ttu-id="45a53-107">Тип</span><span class="sxs-lookup"><span data-stu-id="45a53-107">Type</span></span>|<span data-ttu-id="45a53-108">Описание</span><span class="sxs-lookup"><span data-stu-id="45a53-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45a53-109">displayName</span><span class="sxs-lookup"><span data-stu-id="45a53-109">displayName</span></span>|<span data-ttu-id="45a53-110">Строка</span><span class="sxs-lookup"><span data-stu-id="45a53-110">String</span></span>|<span data-ttu-id="45a53-111">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="45a53-111">Display Name.</span></span> <span data-ttu-id="45a53-112">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="45a53-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="45a53-113">description</span><span class="sxs-lookup"><span data-stu-id="45a53-113">description</span></span>|<span data-ttu-id="45a53-114">Строка</span><span class="sxs-lookup"><span data-stu-id="45a53-114">String</span></span>|<span data-ttu-id="45a53-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="45a53-115">Description.</span></span> <span data-ttu-id="45a53-116">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="45a53-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="45a53-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="45a53-117">omaUri</span></span>|<span data-ttu-id="45a53-118">Строка</span><span class="sxs-lookup"><span data-stu-id="45a53-118">String</span></span>|<span data-ttu-id="45a53-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="45a53-119">OMA.</span></span> <span data-ttu-id="45a53-120">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="45a53-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="45a53-121">value</span><span class="sxs-lookup"><span data-stu-id="45a53-121">value</span></span>|<span data-ttu-id="45a53-122">Single</span><span class="sxs-lookup"><span data-stu-id="45a53-122">Single</span></span>|<span data-ttu-id="45a53-123">Значение.</span><span class="sxs-lookup"><span data-stu-id="45a53-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45a53-124">Связи</span><span class="sxs-lookup"><span data-stu-id="45a53-124">Relationships</span></span>
<span data-ttu-id="45a53-125">Нет</span><span class="sxs-lookup"><span data-stu-id="45a53-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="45a53-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="45a53-126">JSON Representation</span></span>
<span data-ttu-id="45a53-127">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45a53-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```



