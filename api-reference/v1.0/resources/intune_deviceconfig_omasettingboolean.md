# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="4a205-101">Тип ресурса omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="4a205-101">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="4a205-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4a205-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a205-103">Логическое определение параметров OMA.</span><span class="sxs-lookup"><span data-stu-id="4a205-103">OMA Settings Boolean definition.</span></span>

<span data-ttu-id="4a205-104">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4a205-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4a205-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4a205-105">Properties</span></span>
|<span data-ttu-id="4a205-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a205-106">Property</span></span>|<span data-ttu-id="4a205-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4a205-107">Type</span></span>|<span data-ttu-id="4a205-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4a205-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a205-109">displayName</span><span class="sxs-lookup"><span data-stu-id="4a205-109">displayName</span></span>|<span data-ttu-id="4a205-110">String</span><span class="sxs-lookup"><span data-stu-id="4a205-110">String</span></span>|<span data-ttu-id="4a205-111">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="4a205-111">Display Name.</span></span> <span data-ttu-id="4a205-112">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4a205-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="4a205-113">description</span><span class="sxs-lookup"><span data-stu-id="4a205-113">description</span></span>|<span data-ttu-id="4a205-114">String</span><span class="sxs-lookup"><span data-stu-id="4a205-114">String</span></span>|<span data-ttu-id="4a205-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="4a205-115">Description.</span></span> <span data-ttu-id="4a205-116">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4a205-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="4a205-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="4a205-117">omaUri</span></span>|<span data-ttu-id="4a205-118">String</span><span class="sxs-lookup"><span data-stu-id="4a205-118">String</span></span>|<span data-ttu-id="4a205-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="4a205-119">OMA.</span></span> <span data-ttu-id="4a205-120">Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4a205-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="4a205-121">value</span><span class="sxs-lookup"><span data-stu-id="4a205-121">value</span></span>|<span data-ttu-id="4a205-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a205-122">Boolean</span></span>|<span data-ttu-id="4a205-123">Значение</span><span class="sxs-lookup"><span data-stu-id="4a205-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a205-124">Связи</span><span class="sxs-lookup"><span data-stu-id="4a205-124">Relationships</span></span>
<span data-ttu-id="4a205-125">Нет</span><span class="sxs-lookup"><span data-stu-id="4a205-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4a205-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4a205-126">JSON Representation</span></span>
<span data-ttu-id="4a205-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a205-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": true
}
```



