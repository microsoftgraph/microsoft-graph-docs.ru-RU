# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="fbc24-101">Тип ресурса omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="fbc24-101">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="fbc24-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fbc24-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fbc24-103">Определение даты и времени параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="fbc24-103">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="fbc24-104">Наследуется от ресурса [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fbc24-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fbc24-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="fbc24-105">Properties</span></span>
|<span data-ttu-id="fbc24-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="fbc24-106">Property</span></span>|<span data-ttu-id="fbc24-107">Тип</span><span class="sxs-lookup"><span data-stu-id="fbc24-107">Type</span></span>|<span data-ttu-id="fbc24-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fbc24-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbc24-109">displayName</span><span class="sxs-lookup"><span data-stu-id="fbc24-109">displayName</span></span>|<span data-ttu-id="fbc24-110">Строка</span><span class="sxs-lookup"><span data-stu-id="fbc24-110">String</span></span>|<span data-ttu-id="fbc24-111">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="fbc24-111">Display Name</span></span> <span data-ttu-id="fbc24-112">Наследуется от ресурса [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fbc24-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="fbc24-113">description</span><span class="sxs-lookup"><span data-stu-id="fbc24-113">description</span></span>|<span data-ttu-id="fbc24-114">Строка</span><span class="sxs-lookup"><span data-stu-id="fbc24-114">String</span></span>|<span data-ttu-id="fbc24-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="fbc24-115">Description</span></span> <span data-ttu-id="fbc24-116">Наследуется от ресурса [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fbc24-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="fbc24-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="fbc24-117">omaUri</span></span>|<span data-ttu-id="fbc24-118">Строка</span><span class="sxs-lookup"><span data-stu-id="fbc24-118">String</span></span>|<span data-ttu-id="fbc24-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="fbc24-119">OMA.</span></span> <span data-ttu-id="fbc24-120">Наследуется от ресурса [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fbc24-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="fbc24-121">value</span><span class="sxs-lookup"><span data-stu-id="fbc24-121">value</span></span>|<span data-ttu-id="fbc24-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbc24-122">DateTimeOffset</span></span>|<span data-ttu-id="fbc24-123">Значение.</span><span class="sxs-lookup"><span data-stu-id="fbc24-123">Value</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbc24-124">Связи</span><span class="sxs-lookup"><span data-stu-id="fbc24-124">Relationships</span></span>
<span data-ttu-id="fbc24-125">Нет</span><span class="sxs-lookup"><span data-stu-id="fbc24-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fbc24-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fbc24-126">JSON Representation</span></span>
<span data-ttu-id="fbc24-127">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fbc24-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String (timestamp)"
}
```



