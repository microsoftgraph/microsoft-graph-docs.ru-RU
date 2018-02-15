# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="47a50-101">Тип ресурса managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="47a50-101">managedAppPolicy resource type</span></span>

> <span data-ttu-id="47a50-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="47a50-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47a50-103">Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.</span><span class="sxs-lookup"><span data-stu-id="47a50-103">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="47a50-104">Методы</span><span class="sxs-lookup"><span data-stu-id="47a50-104">Methods</span></span>
|<span data-ttu-id="47a50-105">Метод</span><span class="sxs-lookup"><span data-stu-id="47a50-105">Method</span></span>|<span data-ttu-id="47a50-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="47a50-106">Return Type</span></span>|<span data-ttu-id="47a50-107">Описание</span><span class="sxs-lookup"><span data-stu-id="47a50-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="47a50-108">Список объектов managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="47a50-108">List managedAppPolicies</span></span>](../api/intune_mam_managedapppolicy_list.md)|<span data-ttu-id="47a50-109">Коллекция [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="47a50-109">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="47a50-110">Список свойств и связей объектов [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="47a50-110">List properties and relationships of the [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="47a50-111">Получение объекта managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="47a50-111">Get managedAppPolicy</span></span>](../api/intune_mam_managedapppolicy_get.md)|[<span data-ttu-id="47a50-112">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="47a50-112">managedAppPolicy</span></span>](../resources/intune_mam_managedapppolicy.md)|<span data-ttu-id="47a50-113">Чтение свойств и связей объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="47a50-113">Read properties and relationships of [plannerTaskDetails](../resources/intune_mam_managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="47a50-114">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="47a50-114">targetApps action</span></span>](../api/intune_mam_managedapppolicy_targetapps.md)|<span data-ttu-id="47a50-115">Нет</span><span class="sxs-lookup"><span data-stu-id="47a50-115">None</span></span>|<span data-ttu-id="47a50-116">Н/Д</span><span class="sxs-lookup"><span data-stu-id="47a50-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="47a50-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="47a50-117">Properties</span></span>
|<span data-ttu-id="47a50-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="47a50-118">Property</span></span>|<span data-ttu-id="47a50-119">Тип</span><span class="sxs-lookup"><span data-stu-id="47a50-119">Type</span></span>|<span data-ttu-id="47a50-120">Описание</span><span class="sxs-lookup"><span data-stu-id="47a50-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47a50-121">displayName</span><span class="sxs-lookup"><span data-stu-id="47a50-121">displayName</span></span>|<span data-ttu-id="47a50-122">String</span><span class="sxs-lookup"><span data-stu-id="47a50-122">String</span></span>|<span data-ttu-id="47a50-123">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="47a50-123">Policy display name.</span></span>|
|<span data-ttu-id="47a50-124">description</span><span class="sxs-lookup"><span data-stu-id="47a50-124">description</span></span>|<span data-ttu-id="47a50-125">String</span><span class="sxs-lookup"><span data-stu-id="47a50-125">String</span></span>|<span data-ttu-id="47a50-126">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="47a50-126">The policy's description.</span></span>|
|<span data-ttu-id="47a50-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="47a50-127">createdDateTime</span></span>|<span data-ttu-id="47a50-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47a50-128">DateTimeOffset</span></span>|<span data-ttu-id="47a50-129">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="47a50-129">The date and time the group was created.</span></span>|
|<span data-ttu-id="47a50-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="47a50-130">lastModifiedDateTime</span></span>|<span data-ttu-id="47a50-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47a50-131">DateTimeOffset</span></span>|<span data-ttu-id="47a50-132">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="47a50-132">Last time the policy was modified.</span></span>|
|<span data-ttu-id="47a50-133">id</span><span class="sxs-lookup"><span data-stu-id="47a50-133">id</span></span>|<span data-ttu-id="47a50-134">String</span><span class="sxs-lookup"><span data-stu-id="47a50-134">String</span></span>|<span data-ttu-id="47a50-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="47a50-135">Key of the setting.</span></span>|
|<span data-ttu-id="47a50-136">version</span><span class="sxs-lookup"><span data-stu-id="47a50-136">version</span></span>|<span data-ttu-id="47a50-137">String</span><span class="sxs-lookup"><span data-stu-id="47a50-137">String</span></span>|<span data-ttu-id="47a50-138">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="47a50-138">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47a50-139">Связи</span><span class="sxs-lookup"><span data-stu-id="47a50-139">Relationships</span></span>
<span data-ttu-id="47a50-140">Нет</span><span class="sxs-lookup"><span data-stu-id="47a50-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="47a50-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47a50-141">JSON Representation</span></span>
<span data-ttu-id="47a50-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47a50-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicy",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String"
}
```



