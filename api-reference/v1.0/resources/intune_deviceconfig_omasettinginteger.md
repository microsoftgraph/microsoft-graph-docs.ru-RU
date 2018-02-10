# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="7c0a0-101">Тип ресурса omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="7c0a0-101">omaSettingInteger resource type</span></span>

> <span data-ttu-id="7c0a0-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7c0a0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7c0a0-103">Определение целого числа параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="7c0a0-103">OMA Settings Integer definition.</span></span>

<span data-ttu-id="7c0a0-104">Наследуется от ресурса [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="7c0a0-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7c0a0-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c0a0-105">Properties</span></span>
|<span data-ttu-id="7c0a0-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c0a0-106">Property</span></span>|<span data-ttu-id="7c0a0-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7c0a0-107">Type</span></span>|<span data-ttu-id="7c0a0-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7c0a0-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c0a0-109">displayName</span><span class="sxs-lookup"><span data-stu-id="7c0a0-109">displayName</span></span>|<span data-ttu-id="7c0a0-110">Строка</span><span class="sxs-lookup"><span data-stu-id="7c0a0-110">String</span></span>|<span data-ttu-id="7c0a0-111">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="7c0a0-111">Display Name</span></span> <span data-ttu-id="7c0a0-112">Наследуется от ресурса [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="7c0a0-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="7c0a0-113">description</span><span class="sxs-lookup"><span data-stu-id="7c0a0-113">description</span></span>|<span data-ttu-id="7c0a0-114">Строка</span><span class="sxs-lookup"><span data-stu-id="7c0a0-114">String</span></span>|<span data-ttu-id="7c0a0-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="7c0a0-115">Description</span></span> <span data-ttu-id="7c0a0-116">Наследуется от ресурса [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="7c0a0-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="7c0a0-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="7c0a0-117">omaUri</span></span>|<span data-ttu-id="7c0a0-118">Строка</span><span class="sxs-lookup"><span data-stu-id="7c0a0-118">String</span></span>|<span data-ttu-id="7c0a0-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="7c0a0-119">OMA.</span></span> <span data-ttu-id="7c0a0-120">Наследуется от ресурса [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="7c0a0-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="7c0a0-121">value</span><span class="sxs-lookup"><span data-stu-id="7c0a0-121">value</span></span>|<span data-ttu-id="7c0a0-122">Int32</span><span class="sxs-lookup"><span data-stu-id="7c0a0-122">Int32</span></span>|<span data-ttu-id="7c0a0-123">Значение.</span><span class="sxs-lookup"><span data-stu-id="7c0a0-123">Value</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c0a0-124">Связи</span><span class="sxs-lookup"><span data-stu-id="7c0a0-124">Relationships</span></span>
<span data-ttu-id="7c0a0-125">Нет</span><span class="sxs-lookup"><span data-stu-id="7c0a0-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7c0a0-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7c0a0-126">JSON Representation</span></span>
<span data-ttu-id="7c0a0-127">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c0a0-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



