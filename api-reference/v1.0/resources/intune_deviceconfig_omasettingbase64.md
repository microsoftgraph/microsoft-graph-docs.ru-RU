# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="d0b1b-101">Тип ресурса omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="d0b1b-101">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="d0b1b-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d0b1b-103">Определение параметров OMA в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-103">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="d0b1b-104">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d0b1b-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d0b1b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d0b1b-105">Properties</span></span>
|<span data-ttu-id="d0b1b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0b1b-106">Property</span></span>|<span data-ttu-id="d0b1b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d0b1b-107">Type</span></span>|<span data-ttu-id="d0b1b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d0b1b-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0b1b-109">displayName</span><span class="sxs-lookup"><span data-stu-id="d0b1b-109">displayName</span></span>|<span data-ttu-id="d0b1b-110">Строка</span><span class="sxs-lookup"><span data-stu-id="d0b1b-110">String</span></span>|<span data-ttu-id="d0b1b-111">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-111">Display Name.</span></span> <span data-ttu-id="d0b1b-112">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d0b1b-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="d0b1b-113">description</span><span class="sxs-lookup"><span data-stu-id="d0b1b-113">description</span></span>|<span data-ttu-id="d0b1b-114">Строка</span><span class="sxs-lookup"><span data-stu-id="d0b1b-114">String</span></span>|<span data-ttu-id="d0b1b-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-115">Description.</span></span> <span data-ttu-id="d0b1b-116">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d0b1b-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="d0b1b-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="d0b1b-117">omaUri</span></span>|<span data-ttu-id="d0b1b-118">Строка</span><span class="sxs-lookup"><span data-stu-id="d0b1b-118">String</span></span>|<span data-ttu-id="d0b1b-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-119">OMA.</span></span> <span data-ttu-id="d0b1b-120">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d0b1b-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="d0b1b-121">fileName</span><span class="sxs-lookup"><span data-stu-id="d0b1b-121">fileName</span></span>|<span data-ttu-id="d0b1b-122">Строка</span><span class="sxs-lookup"><span data-stu-id="d0b1b-122">String</span></span>|<span data-ttu-id="d0b1b-123">Имя файла, связанное со свойством Value (CER,</span><span class="sxs-lookup"><span data-stu-id="d0b1b-123">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="d0b1b-124">CRT).</span><span class="sxs-lookup"><span data-stu-id="d0b1b-124">\*.crt ).</span></span>|
|<span data-ttu-id="d0b1b-125">value</span><span class="sxs-lookup"><span data-stu-id="d0b1b-125">value</span></span>|<span data-ttu-id="d0b1b-126">Строка</span><span class="sxs-lookup"><span data-stu-id="d0b1b-126">String</span></span>|<span data-ttu-id="d0b1b-127">Значение</span><span class="sxs-lookup"><span data-stu-id="d0b1b-127">Value.</span></span> <span data-ttu-id="d0b1b-128">(строка в кодировке Base64).</span><span class="sxs-lookup"><span data-stu-id="d0b1b-128">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0b1b-129">Связи</span><span class="sxs-lookup"><span data-stu-id="d0b1b-129">Relationships</span></span>
<span data-ttu-id="d0b1b-130">Нет</span><span class="sxs-lookup"><span data-stu-id="d0b1b-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d0b1b-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d0b1b-131">JSON Representation</span></span>
<span data-ttu-id="d0b1b-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-132">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.omaSetting",
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



