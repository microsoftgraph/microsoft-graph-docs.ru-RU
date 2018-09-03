# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="0f885-101">Тип ресурса omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="0f885-101">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="0f885-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0f885-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f885-103">Логическое определение параметров OMA.</span><span class="sxs-lookup"><span data-stu-id="0f885-103">OMA Settings Boolean definition.</span></span>

<span data-ttu-id="0f885-104">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0f885-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0f885-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f885-105">Properties</span></span>
|<span data-ttu-id="0f885-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f885-106">Property</span></span>|<span data-ttu-id="0f885-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0f885-107">Type</span></span>|<span data-ttu-id="0f885-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0f885-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f885-109">displayName</span><span class="sxs-lookup"><span data-stu-id="0f885-109">displayName</span></span>|<span data-ttu-id="0f885-110">String</span><span class="sxs-lookup"><span data-stu-id="0f885-110">String</span></span>|<span data-ttu-id="0f885-111">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="0f885-111">Display Name.</span></span> <span data-ttu-id="0f885-112">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0f885-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="0f885-113">description</span><span class="sxs-lookup"><span data-stu-id="0f885-113">description</span></span>|<span data-ttu-id="0f885-114">String</span><span class="sxs-lookup"><span data-stu-id="0f885-114">String</span></span>|<span data-ttu-id="0f885-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="0f885-115">Description.</span></span> <span data-ttu-id="0f885-116">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0f885-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="0f885-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="0f885-117">omaUri</span></span>|<span data-ttu-id="0f885-118">String</span><span class="sxs-lookup"><span data-stu-id="0f885-118">String</span></span>|<span data-ttu-id="0f885-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="0f885-119">OMA.</span></span> <span data-ttu-id="0f885-120">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0f885-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="0f885-121">value</span><span class="sxs-lookup"><span data-stu-id="0f885-121">value</span></span>|<span data-ttu-id="0f885-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f885-122">Boolean</span></span>|<span data-ttu-id="0f885-123">Значение</span><span class="sxs-lookup"><span data-stu-id="0f885-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f885-124">Связи</span><span class="sxs-lookup"><span data-stu-id="0f885-124">Relationships</span></span>
<span data-ttu-id="0f885-125">Нет</span><span class="sxs-lookup"><span data-stu-id="0f885-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0f885-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f885-126">JSON Representation</span></span>
<span data-ttu-id="0f885-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f885-127">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.omaSetting",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": true
}
```



