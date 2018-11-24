# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="ed730-101">Тип ресурса omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="ed730-101">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="ed730-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ed730-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed730-103">Определение строки параметра OMA в формате XML.</span><span class="sxs-lookup"><span data-stu-id="ed730-103">OMA Settings StringXML definition.</span></span>

<span data-ttu-id="ed730-104">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ed730-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ed730-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ed730-105">Properties</span></span>
|<span data-ttu-id="ed730-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed730-106">Property</span></span>|<span data-ttu-id="ed730-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ed730-107">Type</span></span>|<span data-ttu-id="ed730-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ed730-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed730-109">displayName</span><span class="sxs-lookup"><span data-stu-id="ed730-109">displayName</span></span>|<span data-ttu-id="ed730-110">String</span><span class="sxs-lookup"><span data-stu-id="ed730-110">String</span></span>|<span data-ttu-id="ed730-111">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="ed730-111">Display Name.</span></span> <span data-ttu-id="ed730-112">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ed730-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="ed730-113">description</span><span class="sxs-lookup"><span data-stu-id="ed730-113">description</span></span>|<span data-ttu-id="ed730-114">String</span><span class="sxs-lookup"><span data-stu-id="ed730-114">String</span></span>|<span data-ttu-id="ed730-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="ed730-115">Description.</span></span> <span data-ttu-id="ed730-116">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ed730-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="ed730-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="ed730-117">omaUri</span></span>|<span data-ttu-id="ed730-118">String</span><span class="sxs-lookup"><span data-stu-id="ed730-118">String</span></span>|<span data-ttu-id="ed730-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="ed730-119">OMA.</span></span> <span data-ttu-id="ed730-120">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ed730-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="ed730-121">fileName</span><span class="sxs-lookup"><span data-stu-id="ed730-121">fileName</span></span>|<span data-ttu-id="ed730-122">String</span><span class="sxs-lookup"><span data-stu-id="ed730-122">String</span></span>|<span data-ttu-id="ed730-123">Имя файла, связанное со свойством Value (XML).</span><span class="sxs-lookup"><span data-stu-id="ed730-123">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="ed730-124">value</span><span class="sxs-lookup"><span data-stu-id="ed730-124">value</span></span>|<span data-ttu-id="ed730-125">Двоичный</span><span class="sxs-lookup"><span data-stu-id="ed730-125">Binary</span></span>|<span data-ttu-id="ed730-126">Значение</span><span class="sxs-lookup"><span data-stu-id="ed730-126">Value.</span></span> <span data-ttu-id="ed730-127">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="ed730-127">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed730-128">Связи</span><span class="sxs-lookup"><span data-stu-id="ed730-128">Relationships</span></span>
<span data-ttu-id="ed730-129">Нет</span><span class="sxs-lookup"><span data-stu-id="ed730-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ed730-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ed730-130">JSON Representation</span></span>
<span data-ttu-id="ed730-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed730-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
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



