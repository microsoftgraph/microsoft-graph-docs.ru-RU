# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="6f6b3-101">Тип ресурса omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="6f6b3-101">omaSettingInteger resource type</span></span>

> <span data-ttu-id="6f6b3-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6f6b3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f6b3-103">Определение целого числа параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="6f6b3-103">OMA Settings Integer definition.</span></span>

<span data-ttu-id="6f6b3-104">Наследуется от ресурса [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6f6b3-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6f6b3-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f6b3-105">Properties</span></span>
|<span data-ttu-id="6f6b3-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f6b3-106">Property</span></span>|<span data-ttu-id="6f6b3-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6f6b3-107">Type</span></span>|<span data-ttu-id="6f6b3-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6f6b3-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f6b3-109">displayName</span><span class="sxs-lookup"><span data-stu-id="6f6b3-109">displayName</span></span>|<span data-ttu-id="6f6b3-110">Строка</span><span class="sxs-lookup"><span data-stu-id="6f6b3-110">String</span></span>|<span data-ttu-id="6f6b3-111">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="6f6b3-111">Display Name.</span></span> <span data-ttu-id="6f6b3-112">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6f6b3-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="6f6b3-113">description</span><span class="sxs-lookup"><span data-stu-id="6f6b3-113">description</span></span>|<span data-ttu-id="6f6b3-114">Строка</span><span class="sxs-lookup"><span data-stu-id="6f6b3-114">String</span></span>|<span data-ttu-id="6f6b3-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="6f6b3-115">Description.</span></span> <span data-ttu-id="6f6b3-116">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6f6b3-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="6f6b3-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="6f6b3-117">omaUri</span></span>|<span data-ttu-id="6f6b3-118">Строка</span><span class="sxs-lookup"><span data-stu-id="6f6b3-118">String</span></span>|<span data-ttu-id="6f6b3-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="6f6b3-119">OMA.</span></span> <span data-ttu-id="6f6b3-120">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6f6b3-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="6f6b3-121">value</span><span class="sxs-lookup"><span data-stu-id="6f6b3-121">value</span></span>|<span data-ttu-id="6f6b3-122">Int32</span><span class="sxs-lookup"><span data-stu-id="6f6b3-122">Int32</span></span>|<span data-ttu-id="6f6b3-123">Значение.</span><span class="sxs-lookup"><span data-stu-id="6f6b3-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f6b3-124">Связи</span><span class="sxs-lookup"><span data-stu-id="6f6b3-124">Relationships</span></span>
<span data-ttu-id="6f6b3-125">Нет</span><span class="sxs-lookup"><span data-stu-id="6f6b3-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6f6b3-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f6b3-126">JSON Representation</span></span>
<span data-ttu-id="6f6b3-127">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f6b3-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```



