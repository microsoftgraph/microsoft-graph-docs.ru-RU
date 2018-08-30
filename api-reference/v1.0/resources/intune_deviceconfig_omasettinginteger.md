# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="9288c-101">Тип ресурса omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="9288c-101">omaSettingInteger resource type</span></span>

> <span data-ttu-id="9288c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9288c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9288c-103">Определение целого числа параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="9288c-103">OMA Settings Integer definition.</span></span>

<span data-ttu-id="9288c-104">Наследуется от ресурса [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9288c-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9288c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9288c-105">Properties</span></span>
|<span data-ttu-id="9288c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9288c-106">Property</span></span>|<span data-ttu-id="9288c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9288c-107">Type</span></span>|<span data-ttu-id="9288c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9288c-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9288c-109">displayName</span><span class="sxs-lookup"><span data-stu-id="9288c-109">displayName</span></span>|<span data-ttu-id="9288c-110">Cтрока</span><span class="sxs-lookup"><span data-stu-id="9288c-110">String</span></span>|<span data-ttu-id="9288c-111">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="9288c-111">Display Name.</span></span> <span data-ttu-id="9288c-112">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9288c-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="9288c-113">description</span><span class="sxs-lookup"><span data-stu-id="9288c-113">description</span></span>|<span data-ttu-id="9288c-114">Cтрока</span><span class="sxs-lookup"><span data-stu-id="9288c-114">String</span></span>|<span data-ttu-id="9288c-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="9288c-115">Description.</span></span> <span data-ttu-id="9288c-116">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9288c-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="9288c-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="9288c-117">omaUri</span></span>|<span data-ttu-id="9288c-118">Cтрока</span><span class="sxs-lookup"><span data-stu-id="9288c-118">String</span></span>|<span data-ttu-id="9288c-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="9288c-119">OMA.</span></span> <span data-ttu-id="9288c-120">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9288c-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="9288c-121">value</span><span class="sxs-lookup"><span data-stu-id="9288c-121">value</span></span>|<span data-ttu-id="9288c-122">Int32</span><span class="sxs-lookup"><span data-stu-id="9288c-122">Int32</span></span>|<span data-ttu-id="9288c-123">Значение.</span><span class="sxs-lookup"><span data-stu-id="9288c-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9288c-124">Связи</span><span class="sxs-lookup"><span data-stu-id="9288c-124">Relationships</span></span>
<span data-ttu-id="9288c-125">Нет</span><span class="sxs-lookup"><span data-stu-id="9288c-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9288c-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9288c-126">JSON Representation</span></span>
<span data-ttu-id="9288c-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9288c-127">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.omaSetting",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```



