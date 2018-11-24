# <a name="omasettingstring-resource-type"></a><span data-ttu-id="78d4a-101">Тип ресурса omaSettingString</span><span class="sxs-lookup"><span data-stu-id="78d4a-101">omaSettingString resource type</span></span>

> <span data-ttu-id="78d4a-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="78d4a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78d4a-103">Определение строки параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="78d4a-103">OMA Settings String definition.</span></span>

<span data-ttu-id="78d4a-104">Наследуется от ресурса [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="78d4a-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="78d4a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="78d4a-105">Properties</span></span>
|<span data-ttu-id="78d4a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="78d4a-106">Property</span></span>|<span data-ttu-id="78d4a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="78d4a-107">Type</span></span>|<span data-ttu-id="78d4a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="78d4a-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78d4a-109">displayName</span><span class="sxs-lookup"><span data-stu-id="78d4a-109">displayName</span></span>|<span data-ttu-id="78d4a-110">Строка</span><span class="sxs-lookup"><span data-stu-id="78d4a-110">String</span></span>|<span data-ttu-id="78d4a-111">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="78d4a-111">Display Name.</span></span> <span data-ttu-id="78d4a-112">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="78d4a-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="78d4a-113">description</span><span class="sxs-lookup"><span data-stu-id="78d4a-113">description</span></span>|<span data-ttu-id="78d4a-114">Строка</span><span class="sxs-lookup"><span data-stu-id="78d4a-114">String</span></span>|<span data-ttu-id="78d4a-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="78d4a-115">Description.</span></span> <span data-ttu-id="78d4a-116">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="78d4a-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="78d4a-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="78d4a-117">omaUri</span></span>|<span data-ttu-id="78d4a-118">Строка</span><span class="sxs-lookup"><span data-stu-id="78d4a-118">String</span></span>|<span data-ttu-id="78d4a-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="78d4a-119">OMA.</span></span> <span data-ttu-id="78d4a-120">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="78d4a-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="78d4a-121">value</span><span class="sxs-lookup"><span data-stu-id="78d4a-121">value</span></span>|<span data-ttu-id="78d4a-122">Строка</span><span class="sxs-lookup"><span data-stu-id="78d4a-122">String</span></span>|<span data-ttu-id="78d4a-123">Значение.</span><span class="sxs-lookup"><span data-stu-id="78d4a-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78d4a-124">Связи</span><span class="sxs-lookup"><span data-stu-id="78d4a-124">Relationships</span></span>
<span data-ttu-id="78d4a-125">Нет</span><span class="sxs-lookup"><span data-stu-id="78d4a-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="78d4a-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="78d4a-126">JSON Representation</span></span>
<span data-ttu-id="78d4a-127">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="78d4a-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```



