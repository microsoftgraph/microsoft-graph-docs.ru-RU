# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="afbd4-101">Тип ресурса onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="afbd4-101">onPremisesConditionalAccessSettings resource type</span></span>

> <span data-ttu-id="afbd4-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="afbd4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="afbd4-103">Одноэлементный объект, представляющий параметры условного доступа к локальной среде Exchange для клиента.</span><span class="sxs-lookup"><span data-stu-id="afbd4-103">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="afbd4-104">Методы</span><span class="sxs-lookup"><span data-stu-id="afbd4-104">Methods</span></span>
|<span data-ttu-id="afbd4-105">Метод</span><span class="sxs-lookup"><span data-stu-id="afbd4-105">Method</span></span>|<span data-ttu-id="afbd4-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="afbd4-106">Return Type</span></span>|<span data-ttu-id="afbd4-107">Описание</span><span class="sxs-lookup"><span data-stu-id="afbd4-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="afbd4-108">Получение объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="afbd4-108">Get onPremisesConditionalAccessSettings</span></span>](../api/intune_onboarding_onpremisesconditionalaccesssettings_get.md)|[<span data-ttu-id="afbd4-109">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="afbd4-109">onPremisesConditionalAccessSettings</span></span>](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|<span data-ttu-id="afbd4-110">Чтение свойств и связей объекта [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="afbd4-110">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="afbd4-111">Обновление объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="afbd4-111">Update onPremisesConditionalAccessSettings</span></span>](../api/intune_onboarding_onpremisesconditionalaccesssettings_update.md)|[<span data-ttu-id="afbd4-112">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="afbd4-112">onPremisesConditionalAccessSettings</span></span>](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|<span data-ttu-id="afbd4-113">Обновление свойств объекта [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="afbd4-113">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="afbd4-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="afbd4-114">Properties</span></span>
|<span data-ttu-id="afbd4-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="afbd4-115">Property</span></span>|<span data-ttu-id="afbd4-116">Тип</span><span class="sxs-lookup"><span data-stu-id="afbd4-116">Type</span></span>|<span data-ttu-id="afbd4-117">Описание</span><span class="sxs-lookup"><span data-stu-id="afbd4-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afbd4-118">id</span><span class="sxs-lookup"><span data-stu-id="afbd4-118">id</span></span>|<span data-ttu-id="afbd4-119">String</span><span class="sxs-lookup"><span data-stu-id="afbd4-119">String</span></span>|<span data-ttu-id="afbd4-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="afbd4-120">Not yet documented</span></span>|
|<span data-ttu-id="afbd4-121">enabled</span><span class="sxs-lookup"><span data-stu-id="afbd4-121">enabled</span></span>|<span data-ttu-id="afbd4-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="afbd4-122">Boolean</span></span>|<span data-ttu-id="afbd4-123">Указывает, включен ли в этой организации условный доступ к локальной среде</span><span class="sxs-lookup"><span data-stu-id="afbd4-123">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="afbd4-124">includedGroups</span><span class="sxs-lookup"><span data-stu-id="afbd4-124">includedGroups</span></span>|<span data-ttu-id="afbd4-125">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="afbd4-125">Guid collection</span></span>|<span data-ttu-id="afbd4-126">Группы пользователей, для которых включается условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="afbd4-126">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="afbd4-127">У всех пользователей в этих группах должны быть управляемые мобильные устройства, соответствующие требованиям для доступа к почте.</span><span class="sxs-lookup"><span data-stu-id="afbd4-127">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="afbd4-128">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="afbd4-128">excludedGroups</span></span>|<span data-ttu-id="afbd4-129">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="afbd4-129">Guid collection</span></span>|<span data-ttu-id="afbd4-130">Группы пользователей, на которые не распространяется условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="afbd4-130">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="afbd4-131">На всех пользователей из этих группах не будет распространяться политика условного доступа.</span><span class="sxs-lookup"><span data-stu-id="afbd4-131">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="afbd4-132">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="afbd4-132">overrideDefaultRule</span></span>|<span data-ttu-id="afbd4-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="afbd4-133">Boolean</span></span>|<span data-ttu-id="afbd4-134">Указывает, следует ли переопределять правило доступа по умолчанию при разрешении устройства, чтобы обеспечить предоставление доступа.</span><span class="sxs-lookup"><span data-stu-id="afbd4-134">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="afbd4-135">Связи</span><span class="sxs-lookup"><span data-stu-id="afbd4-135">Relationships</span></span>
<span data-ttu-id="afbd4-136">Нет</span><span class="sxs-lookup"><span data-stu-id="afbd4-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="afbd4-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="afbd4-137">JSON Representation</span></span>
<span data-ttu-id="afbd4-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="afbd4-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremisesConditionalAccessSettings"
}
-->
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



