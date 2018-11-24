# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="c258a-101">Тип ресурса omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="c258a-101">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="c258a-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c258a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c258a-103">Определение параметров OMA в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="c258a-103">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="c258a-104">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c258a-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c258a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c258a-105">Properties</span></span>
|<span data-ttu-id="c258a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c258a-106">Property</span></span>|<span data-ttu-id="c258a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c258a-107">Type</span></span>|<span data-ttu-id="c258a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c258a-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c258a-109">displayName</span><span class="sxs-lookup"><span data-stu-id="c258a-109">displayName</span></span>|<span data-ttu-id="c258a-110">String</span><span class="sxs-lookup"><span data-stu-id="c258a-110">String</span></span>|<span data-ttu-id="c258a-111">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="c258a-111">Display Name.</span></span> <span data-ttu-id="c258a-112">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c258a-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="c258a-113">description</span><span class="sxs-lookup"><span data-stu-id="c258a-113">description</span></span>|<span data-ttu-id="c258a-114">String</span><span class="sxs-lookup"><span data-stu-id="c258a-114">String</span></span>|<span data-ttu-id="c258a-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="c258a-115">Description.</span></span> <span data-ttu-id="c258a-116">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c258a-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="c258a-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="c258a-117">omaUri</span></span>|<span data-ttu-id="c258a-118">String</span><span class="sxs-lookup"><span data-stu-id="c258a-118">String</span></span>|<span data-ttu-id="c258a-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="c258a-119">OMA.</span></span> <span data-ttu-id="c258a-120">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c258a-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="c258a-121">fileName</span><span class="sxs-lookup"><span data-stu-id="c258a-121">fileName</span></span>|<span data-ttu-id="c258a-122">String</span><span class="sxs-lookup"><span data-stu-id="c258a-122">String</span></span>|<span data-ttu-id="c258a-123">Имя файла, связанное со свойством Value (CER, </span><span class="sxs-lookup"><span data-stu-id="c258a-123">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="c258a-124">\*.CRT</span><span class="sxs-lookup"><span data-stu-id="c258a-124">\*.crt</span></span> | <span data-ttu-id="c258a-125">\*.p7b</span><span class="sxs-lookup"><span data-stu-id="c258a-125">\*.p7b</span></span> | <span data-ttu-id="c258a-126">\* .bin).</span><span class="sxs-lookup"><span data-stu-id="c258a-126">\*.bin).</span></span>|
|<span data-ttu-id="c258a-127">value</span><span class="sxs-lookup"><span data-stu-id="c258a-127">value</span></span>|<span data-ttu-id="c258a-128">String</span><span class="sxs-lookup"><span data-stu-id="c258a-128">String</span></span>|<span data-ttu-id="c258a-129">Значение</span><span class="sxs-lookup"><span data-stu-id="c258a-129">Value.</span></span> <span data-ttu-id="c258a-130">(строка в кодировке Base64).</span><span class="sxs-lookup"><span data-stu-id="c258a-130">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c258a-131">Связи</span><span class="sxs-lookup"><span data-stu-id="c258a-131">Relationships</span></span>
<span data-ttu-id="c258a-132">None</span><span class="sxs-lookup"><span data-stu-id="c258a-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c258a-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c258a-133">JSON Representation</span></span>
<span data-ttu-id="c258a-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c258a-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBase64",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "String"
}
```



