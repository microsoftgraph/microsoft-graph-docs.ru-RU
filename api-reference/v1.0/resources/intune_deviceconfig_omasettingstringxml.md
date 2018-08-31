# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="a0f62-101">Тип ресурса omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="a0f62-101">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="a0f62-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a0f62-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0f62-103">Определение строки параметра OMA в формате XML.</span><span class="sxs-lookup"><span data-stu-id="a0f62-103">OMA Settings StringXML definition.</span></span>

<span data-ttu-id="a0f62-104">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a0f62-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a0f62-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a0f62-105">Properties</span></span>
|<span data-ttu-id="a0f62-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0f62-106">Property</span></span>|<span data-ttu-id="a0f62-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a0f62-107">Type</span></span>|<span data-ttu-id="a0f62-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a0f62-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0f62-109">displayName</span><span class="sxs-lookup"><span data-stu-id="a0f62-109">displayName</span></span>|<span data-ttu-id="a0f62-110">Строка​</span><span class="sxs-lookup"><span data-stu-id="a0f62-110">String</span></span>|<span data-ttu-id="a0f62-111">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="a0f62-111">Display Name.</span></span> <span data-ttu-id="a0f62-112">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a0f62-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="a0f62-113">description</span><span class="sxs-lookup"><span data-stu-id="a0f62-113">description</span></span>|<span data-ttu-id="a0f62-114">Строка​</span><span class="sxs-lookup"><span data-stu-id="a0f62-114">String</span></span>|<span data-ttu-id="a0f62-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="a0f62-115">Description.</span></span> <span data-ttu-id="a0f62-116">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a0f62-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="a0f62-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="a0f62-117">omaUri</span></span>|<span data-ttu-id="a0f62-118">Строка​</span><span class="sxs-lookup"><span data-stu-id="a0f62-118">String</span></span>|<span data-ttu-id="a0f62-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="a0f62-119">OMA.</span></span> <span data-ttu-id="a0f62-120">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a0f62-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="a0f62-121">fileName</span><span class="sxs-lookup"><span data-stu-id="a0f62-121">fileName</span></span>|<span data-ttu-id="a0f62-122">Строка​</span><span class="sxs-lookup"><span data-stu-id="a0f62-122">String</span></span>|<span data-ttu-id="a0f62-123">Имя файла, связанное со свойством Value (XML).</span><span class="sxs-lookup"><span data-stu-id="a0f62-123">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="a0f62-124">value</span><span class="sxs-lookup"><span data-stu-id="a0f62-124">value</span></span>|<span data-ttu-id="a0f62-125">Двоичный</span><span class="sxs-lookup"><span data-stu-id="a0f62-125">Binary</span></span>|<span data-ttu-id="a0f62-126">Значение</span><span class="sxs-lookup"><span data-stu-id="a0f62-126">Value.</span></span> <span data-ttu-id="a0f62-127">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="a0f62-127">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0f62-128">Связи</span><span class="sxs-lookup"><span data-stu-id="a0f62-128">Relationships</span></span>
<span data-ttu-id="a0f62-129">Нет</span><span class="sxs-lookup"><span data-stu-id="a0f62-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a0f62-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a0f62-130">JSON Representation</span></span>
<span data-ttu-id="a0f62-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0f62-131">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.omaSetting",
  "@odata.type": "microsoft.graph.omaSettingStringXml"
}-->
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



