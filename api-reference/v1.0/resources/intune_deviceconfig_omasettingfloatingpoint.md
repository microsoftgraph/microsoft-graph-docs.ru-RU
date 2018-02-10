# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="81c07-101">Тип ресурса omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="81c07-101">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="81c07-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="81c07-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81c07-103">Определение плавающей запятой параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="81c07-103">OMA Settings Floating Point definition.</span></span>

<span data-ttu-id="81c07-104">Наследуется от ресурса [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="81c07-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="81c07-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="81c07-105">Properties</span></span>
|<span data-ttu-id="81c07-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="81c07-106">Property</span></span>|<span data-ttu-id="81c07-107">Тип</span><span class="sxs-lookup"><span data-stu-id="81c07-107">Type</span></span>|<span data-ttu-id="81c07-108">Описание</span><span class="sxs-lookup"><span data-stu-id="81c07-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81c07-109">displayName</span><span class="sxs-lookup"><span data-stu-id="81c07-109">displayName</span></span>|<span data-ttu-id="81c07-110">Строка</span><span class="sxs-lookup"><span data-stu-id="81c07-110">String</span></span>|<span data-ttu-id="81c07-111">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="81c07-111">Display Name</span></span> <span data-ttu-id="81c07-112">Наследуется от ресурса [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="81c07-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="81c07-113">description</span><span class="sxs-lookup"><span data-stu-id="81c07-113">description</span></span>|<span data-ttu-id="81c07-114">Строка</span><span class="sxs-lookup"><span data-stu-id="81c07-114">String</span></span>|<span data-ttu-id="81c07-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="81c07-115">Description</span></span> <span data-ttu-id="81c07-116">Наследуется от ресурса [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="81c07-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="81c07-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="81c07-117">omaUri</span></span>|<span data-ttu-id="81c07-118">Строка</span><span class="sxs-lookup"><span data-stu-id="81c07-118">String</span></span>|<span data-ttu-id="81c07-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="81c07-119">OMA.</span></span> <span data-ttu-id="81c07-120">Наследуется от ресурса [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="81c07-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="81c07-121">value</span><span class="sxs-lookup"><span data-stu-id="81c07-121">value</span></span>|<span data-ttu-id="81c07-122">Single</span><span class="sxs-lookup"><span data-stu-id="81c07-122">Single</span></span>|<span data-ttu-id="81c07-123">Значение.</span><span class="sxs-lookup"><span data-stu-id="81c07-123">Value</span></span>|

## <a name="relationships"></a><span data-ttu-id="81c07-124">Связи</span><span class="sxs-lookup"><span data-stu-id="81c07-124">Relationships</span></span>
<span data-ttu-id="81c07-125">Нет</span><span class="sxs-lookup"><span data-stu-id="81c07-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="81c07-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="81c07-126">JSON Representation</span></span>
<span data-ttu-id="81c07-127">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81c07-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```



