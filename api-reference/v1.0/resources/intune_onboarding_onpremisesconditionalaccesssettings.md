# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="f0dcc-101">Тип ресурса onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="f0dcc-101">onPremisesConditionalAccessSettings resource type</span></span>

> <span data-ttu-id="f0dcc-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f0dcc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0dcc-103">Одноэлементный объект, представляющий параметры условного доступа к локальной среде Exchange для клиента.</span><span class="sxs-lookup"><span data-stu-id="f0dcc-103">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="f0dcc-104">Методы</span><span class="sxs-lookup"><span data-stu-id="f0dcc-104">Methods</span></span>
|<span data-ttu-id="f0dcc-105">Метод</span><span class="sxs-lookup"><span data-stu-id="f0dcc-105">Method</span></span>|<span data-ttu-id="f0dcc-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f0dcc-106">Return Type</span></span>|<span data-ttu-id="f0dcc-107">Описание</span><span class="sxs-lookup"><span data-stu-id="f0dcc-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f0dcc-108">Получение объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="f0dcc-108">Get onPremisesConditionalAccessSettings</span></span>](../api/intune_onboarding_onpremisesconditionalaccesssettings_get.md)|[<span data-ttu-id="f0dcc-109">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="f0dcc-109">onPremisesConditionalAccessSettings</span></span>](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|<span data-ttu-id="f0dcc-110">Чтение свойств и связей объекта [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="f0dcc-110">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="f0dcc-111">Обновление объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="f0dcc-111">Update onPremisesConditionalAccessSettings</span></span>](../api/intune_onboarding_onpremisesconditionalaccesssettings_update.md)|[<span data-ttu-id="f0dcc-112">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="f0dcc-112">onPremisesConditionalAccessSettings</span></span>](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|<span data-ttu-id="f0dcc-113">Обновление свойств объекта [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="f0dcc-113">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f0dcc-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="f0dcc-114">Properties</span></span>
|<span data-ttu-id="f0dcc-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0dcc-115">Property</span></span>|<span data-ttu-id="f0dcc-116">Тип</span><span class="sxs-lookup"><span data-stu-id="f0dcc-116">Type</span></span>|<span data-ttu-id="f0dcc-117">Описание</span><span class="sxs-lookup"><span data-stu-id="f0dcc-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0dcc-118">ИД</span><span class="sxs-lookup"><span data-stu-id="f0dcc-118">id</span></span>|<span data-ttu-id="f0dcc-119">string</span><span class="sxs-lookup"><span data-stu-id="f0dcc-119">String</span></span>|<span data-ttu-id="f0dcc-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f0dcc-120">Not yet documented</span></span>|
|<span data-ttu-id="f0dcc-121">включено</span><span class="sxs-lookup"><span data-stu-id="f0dcc-121">enabled</span></span>|<span data-ttu-id="f0dcc-122">Логический</span><span class="sxs-lookup"><span data-stu-id="f0dcc-122">Boolean</span></span>|<span data-ttu-id="f0dcc-123">Указывает, включен ли в этой организации условный доступ к локальной среде</span><span class="sxs-lookup"><span data-stu-id="f0dcc-123">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="f0dcc-124">includedGroups</span><span class="sxs-lookup"><span data-stu-id="f0dcc-124">includedGroups</span></span>|<span data-ttu-id="f0dcc-125">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="f0dcc-125">Guid collection</span></span>|<span data-ttu-id="f0dcc-126">Группы пользователей, для которых включается условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="f0dcc-126">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="f0dcc-127">У всех пользователей в этих группах должны быть управляемые мобильные устройства, соответствующие требованиям для доступа к почте.</span><span class="sxs-lookup"><span data-stu-id="f0dcc-127">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="f0dcc-128">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="f0dcc-128">excludedGroups</span></span>|<span data-ttu-id="f0dcc-129">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="f0dcc-129">Guid collection</span></span>|<span data-ttu-id="f0dcc-130">Группы пользователей, на которые не распространяется условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="f0dcc-130">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="f0dcc-131">На всех пользователей из этих группах не будет распространяться политика условного доступа.</span><span class="sxs-lookup"><span data-stu-id="f0dcc-131">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="f0dcc-132">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="f0dcc-132">overrideDefaultRule</span></span>|<span data-ttu-id="f0dcc-133">Логический</span><span class="sxs-lookup"><span data-stu-id="f0dcc-133">Boolean</span></span>|<span data-ttu-id="f0dcc-134">Указывает, следует ли переопределять правило доступа по умолчанию при разрешении устройства, чтобы обеспечить предоставление доступа.</span><span class="sxs-lookup"><span data-stu-id="f0dcc-134">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0dcc-135">Связи</span><span class="sxs-lookup"><span data-stu-id="f0dcc-135">Relationships</span></span>
<span data-ttu-id="f0dcc-136">Нет</span><span class="sxs-lookup"><span data-stu-id="f0dcc-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f0dcc-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f0dcc-137">JSON Representation</span></span>
<span data-ttu-id="f0dcc-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0dcc-138">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremisesConditionalAccessSettings"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "String (identifier)",
  "enabled": true,
  "includedGroups": [
    "Guid"
  ],
  "excludedGroups": [
    "Guid"
  ],
  "overrideDefaultRule": true
}
```








