# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="25b78-101">Тип ресурса omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="25b78-101">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="25b78-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="25b78-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="25b78-103">Определение даты и времени параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="25b78-103">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="25b78-104">Наследуется от ресурса [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="25b78-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="25b78-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="25b78-105">Properties</span></span>
|<span data-ttu-id="25b78-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="25b78-106">Property</span></span>|<span data-ttu-id="25b78-107">Тип</span><span class="sxs-lookup"><span data-stu-id="25b78-107">Type</span></span>|<span data-ttu-id="25b78-108">Описание</span><span class="sxs-lookup"><span data-stu-id="25b78-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25b78-109">displayName</span><span class="sxs-lookup"><span data-stu-id="25b78-109">displayName</span></span>|<span data-ttu-id="25b78-110">Строка</span><span class="sxs-lookup"><span data-stu-id="25b78-110">String</span></span>|<span data-ttu-id="25b78-111">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="25b78-111">Display Name.</span></span> <span data-ttu-id="25b78-112">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="25b78-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="25b78-113">description</span><span class="sxs-lookup"><span data-stu-id="25b78-113">description</span></span>|<span data-ttu-id="25b78-114">Строка</span><span class="sxs-lookup"><span data-stu-id="25b78-114">String</span></span>|<span data-ttu-id="25b78-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="25b78-115">Description.</span></span> <span data-ttu-id="25b78-116">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="25b78-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="25b78-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="25b78-117">omaUri</span></span>|<span data-ttu-id="25b78-118">Строка</span><span class="sxs-lookup"><span data-stu-id="25b78-118">String</span></span>|<span data-ttu-id="25b78-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="25b78-119">OMA.</span></span> <span data-ttu-id="25b78-120">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="25b78-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="25b78-121">value</span><span class="sxs-lookup"><span data-stu-id="25b78-121">value</span></span>|<span data-ttu-id="25b78-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25b78-122">DateTimeOffset</span></span>|<span data-ttu-id="25b78-123">Значение.</span><span class="sxs-lookup"><span data-stu-id="25b78-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="25b78-124">Связи</span><span class="sxs-lookup"><span data-stu-id="25b78-124">Relationships</span></span>
<span data-ttu-id="25b78-125">Нет</span><span class="sxs-lookup"><span data-stu-id="25b78-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="25b78-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="25b78-126">JSON Representation</span></span>
<span data-ttu-id="25b78-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25b78-127">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
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








