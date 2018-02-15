# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="844f9-101">Тип ресурса omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="844f9-101">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="844f9-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="844f9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="844f9-103">Определение строки параметра OMA в формате XML.</span><span class="sxs-lookup"><span data-stu-id="844f9-103">OMA Settings StringXML definition.</span></span>

<span data-ttu-id="844f9-104">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="844f9-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="844f9-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="844f9-105">Properties</span></span>
|<span data-ttu-id="844f9-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="844f9-106">Property</span></span>|<span data-ttu-id="844f9-107">Тип</span><span class="sxs-lookup"><span data-stu-id="844f9-107">Type</span></span>|<span data-ttu-id="844f9-108">Описание</span><span class="sxs-lookup"><span data-stu-id="844f9-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="844f9-109">displayName</span><span class="sxs-lookup"><span data-stu-id="844f9-109">displayName</span></span>|<span data-ttu-id="844f9-110">String</span><span class="sxs-lookup"><span data-stu-id="844f9-110">String</span></span>|<span data-ttu-id="844f9-111">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="844f9-111">Display Name</span></span> <span data-ttu-id="844f9-112">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="844f9-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="844f9-113">description</span><span class="sxs-lookup"><span data-stu-id="844f9-113">description</span></span>|<span data-ttu-id="844f9-114">String</span><span class="sxs-lookup"><span data-stu-id="844f9-114">String</span></span>|<span data-ttu-id="844f9-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="844f9-115">Description</span></span> <span data-ttu-id="844f9-116">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="844f9-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="844f9-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="844f9-117">omaUri</span></span>|<span data-ttu-id="844f9-118">String</span><span class="sxs-lookup"><span data-stu-id="844f9-118">String</span></span>|<span data-ttu-id="844f9-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="844f9-119">OMA.</span></span> <span data-ttu-id="844f9-120">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="844f9-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="844f9-121">fileName</span><span class="sxs-lookup"><span data-stu-id="844f9-121">fileName</span></span>|<span data-ttu-id="844f9-122">String</span><span class="sxs-lookup"><span data-stu-id="844f9-122">String</span></span>|<span data-ttu-id="844f9-123">Имя файла, связанное со свойством Value (XML).</span><span class="sxs-lookup"><span data-stu-id="844f9-123">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="844f9-124">value</span><span class="sxs-lookup"><span data-stu-id="844f9-124">value</span></span>|<span data-ttu-id="844f9-125">Двоичный</span><span class="sxs-lookup"><span data-stu-id="844f9-125">Binary</span></span>|<span data-ttu-id="844f9-126">Значение</span><span class="sxs-lookup"><span data-stu-id="844f9-126">Value</span></span> <span data-ttu-id="844f9-127">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="844f9-127">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="844f9-128">Связи</span><span class="sxs-lookup"><span data-stu-id="844f9-128">Relationships</span></span>
<span data-ttu-id="844f9-129">Нет</span><span class="sxs-lookup"><span data-stu-id="844f9-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="844f9-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="844f9-130">JSON Representation</span></span>
<span data-ttu-id="844f9-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="844f9-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.omaSettingStringXml"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingStringXml",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "binary"
}
```



