# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="b7035-101">Тип ресурса omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="b7035-101">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="b7035-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b7035-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b7035-103">Определение даты и времени параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="b7035-103">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="b7035-104">Наследуется от ресурса [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b7035-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b7035-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b7035-105">Properties</span></span>
|<span data-ttu-id="b7035-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7035-106">Property</span></span>|<span data-ttu-id="b7035-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b7035-107">Type</span></span>|<span data-ttu-id="b7035-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b7035-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7035-109">displayName</span><span class="sxs-lookup"><span data-stu-id="b7035-109">displayName</span></span>|<span data-ttu-id="b7035-110">Строка​</span><span class="sxs-lookup"><span data-stu-id="b7035-110">String</span></span>|<span data-ttu-id="b7035-111">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="b7035-111">Display Name.</span></span> <span data-ttu-id="b7035-112">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b7035-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="b7035-113">description</span><span class="sxs-lookup"><span data-stu-id="b7035-113">description</span></span>|<span data-ttu-id="b7035-114">Строка​</span><span class="sxs-lookup"><span data-stu-id="b7035-114">String</span></span>|<span data-ttu-id="b7035-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="b7035-115">Description.</span></span> <span data-ttu-id="b7035-116">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b7035-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="b7035-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="b7035-117">omaUri</span></span>|<span data-ttu-id="b7035-118">Строка​</span><span class="sxs-lookup"><span data-stu-id="b7035-118">String</span></span>|<span data-ttu-id="b7035-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="b7035-119">OMA.</span></span> <span data-ttu-id="b7035-120">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b7035-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="b7035-121">value</span><span class="sxs-lookup"><span data-stu-id="b7035-121">value</span></span>|<span data-ttu-id="b7035-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7035-122">DateTimeOffset</span></span>|<span data-ttu-id="b7035-123">Значение.</span><span class="sxs-lookup"><span data-stu-id="b7035-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7035-124">Связи</span><span class="sxs-lookup"><span data-stu-id="b7035-124">Relationships</span></span>
<span data-ttu-id="b7035-125">Нет</span><span class="sxs-lookup"><span data-stu-id="b7035-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b7035-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b7035-126">JSON Representation</span></span>
<span data-ttu-id="b7035-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7035-127">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.omaSetting",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String (timestamp)"
}
```



