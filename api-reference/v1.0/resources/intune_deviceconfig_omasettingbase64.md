# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="565e4-101">Тип ресурса omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="565e4-101">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="565e4-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="565e4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="565e4-103">Определение параметров OMA в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="565e4-103">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="565e4-104">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="565e4-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="565e4-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="565e4-105">Properties</span></span>
|<span data-ttu-id="565e4-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="565e4-106">Property</span></span>|<span data-ttu-id="565e4-107">Тип</span><span class="sxs-lookup"><span data-stu-id="565e4-107">Type</span></span>|<span data-ttu-id="565e4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="565e4-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="565e4-109">displayName</span><span class="sxs-lookup"><span data-stu-id="565e4-109">displayName</span></span>|<span data-ttu-id="565e4-110">Строка</span><span class="sxs-lookup"><span data-stu-id="565e4-110">String</span></span>|<span data-ttu-id="565e4-111">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="565e4-111">Display Name.</span></span> <span data-ttu-id="565e4-112">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="565e4-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="565e4-113">описание</span><span class="sxs-lookup"><span data-stu-id="565e4-113">description</span></span>|<span data-ttu-id="565e4-114">Строка</span><span class="sxs-lookup"><span data-stu-id="565e4-114">String</span></span>|<span data-ttu-id="565e4-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="565e4-115">Description.</span></span> <span data-ttu-id="565e4-116">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="565e4-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="565e4-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="565e4-117">omaUri</span></span>|<span data-ttu-id="565e4-118">Строка</span><span class="sxs-lookup"><span data-stu-id="565e4-118">String</span></span>|<span data-ttu-id="565e4-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="565e4-119">OMA.</span></span> <span data-ttu-id="565e4-120">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="565e4-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="565e4-121">fileName</span><span class="sxs-lookup"><span data-stu-id="565e4-121">fileName</span></span>|<span data-ttu-id="565e4-122">Строка</span><span class="sxs-lookup"><span data-stu-id="565e4-122">String</span></span>|<span data-ttu-id="565e4-123">Имя файла, связанное со свойством Value (CER,</span><span class="sxs-lookup"><span data-stu-id="565e4-123">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="565e4-124">CRT</span><span class="sxs-lookup"><span data-stu-id="565e4-124">.crt</span></span> | <span data-ttu-id="565e4-125">P7B</span><span class="sxs-lookup"><span data-stu-id="565e4-125">\*.p7b</span></span> | <span data-ttu-id="565e4-126">\*.bin).</span><span class="sxs-lookup"><span data-stu-id="565e4-126">\BIN</span></span>|
|<span data-ttu-id="565e4-127">value</span><span class="sxs-lookup"><span data-stu-id="565e4-127">value</span></span>|<span data-ttu-id="565e4-128">Строка</span><span class="sxs-lookup"><span data-stu-id="565e4-128">String</span></span>|<span data-ttu-id="565e4-129">Значение</span><span class="sxs-lookup"><span data-stu-id="565e4-129">Value.</span></span> <span data-ttu-id="565e4-130">(строка в кодировке Base64).</span><span class="sxs-lookup"><span data-stu-id="565e4-130">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="565e4-131">Связи</span><span class="sxs-lookup"><span data-stu-id="565e4-131">Relationships</span></span>
<span data-ttu-id="565e4-132">Нет</span><span class="sxs-lookup"><span data-stu-id="565e4-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="565e4-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="565e4-133">JSON Representation</span></span>
<span data-ttu-id="565e4-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="565e4-134">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}-->
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








