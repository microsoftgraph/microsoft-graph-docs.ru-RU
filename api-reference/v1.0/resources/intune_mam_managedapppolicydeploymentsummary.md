# <a name="managedapppolicydeploymentsummary-resource-type"></a><span data-ttu-id="226df-101">Тип ресурса managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="226df-101">managedAppPolicyDeploymentSummary resource type</span></span>

> <span data-ttu-id="226df-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="226df-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="226df-103">ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="226df-103">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
## <a name="methods"></a><span data-ttu-id="226df-104">Методы</span><span class="sxs-lookup"><span data-stu-id="226df-104">Methods</span></span>
|<span data-ttu-id="226df-105">Метод</span><span class="sxs-lookup"><span data-stu-id="226df-105">Method</span></span>|<span data-ttu-id="226df-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="226df-106">Return Type</span></span>|<span data-ttu-id="226df-107">Описание</span><span class="sxs-lookup"><span data-stu-id="226df-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="226df-108">Получение объекта managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="226df-108">Get managedAppPolicyDeploymentSummary</span></span>](../api/intune_mam_managedapppolicydeploymentsummary_get.md)|[<span data-ttu-id="226df-109">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="226df-109">managedAppPolicyDeploymentSummary</span></span>](../resources/intune_mam_managedapppolicydeploymentsummary.md)|<span data-ttu-id="226df-110">Чтение свойств и связей объекта [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="226df-110">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) object.</span></span>|
|[<span data-ttu-id="226df-111">Обновление объекта managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="226df-111">Update managedAppPolicyDeploymentSummary</span></span>](../api/intune_mam_managedapppolicydeploymentsummary_update.md)|[<span data-ttu-id="226df-112">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="226df-112">managedAppPolicyDeploymentSummary</span></span>](../resources/intune_mam_managedapppolicydeploymentsummary.md)|<span data-ttu-id="226df-113">Обновление свойств объекта [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="226df-113">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="226df-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="226df-114">Properties</span></span>
|<span data-ttu-id="226df-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="226df-115">Property</span></span>|<span data-ttu-id="226df-116">Тип</span><span class="sxs-lookup"><span data-stu-id="226df-116">Type</span></span>|<span data-ttu-id="226df-117">Описание</span><span class="sxs-lookup"><span data-stu-id="226df-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="226df-118">displayName</span><span class="sxs-lookup"><span data-stu-id="226df-118">displayName</span></span>|<span data-ttu-id="226df-119">String (строка)</span><span class="sxs-lookup"><span data-stu-id="226df-119">String</span></span>|<span data-ttu-id="226df-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="226df-120">Not yet documented</span></span>|
|<span data-ttu-id="226df-121">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="226df-121">configurationDeployedUserCount</span></span>|<span data-ttu-id="226df-122">Int32</span><span class="sxs-lookup"><span data-stu-id="226df-122">Int32</span></span>|<span data-ttu-id="226df-123">Н/Д</span><span class="sxs-lookup"><span data-stu-id="226df-123">Not yet documented</span></span>|
|<span data-ttu-id="226df-124">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="226df-124">lastRefreshTime</span></span>|<span data-ttu-id="226df-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="226df-125">DateTimeOffset</span></span>|<span data-ttu-id="226df-126">Н/Д</span><span class="sxs-lookup"><span data-stu-id="226df-126">Not yet documented</span></span>|
|<span data-ttu-id="226df-127">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="226df-127">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="226df-128">Коллекция [managedAppPolicyDeploymentSummaryPerApp](../resources/intune_mam_managedapppolicydeploymentsummaryperapp.md)</span><span class="sxs-lookup"><span data-stu-id="226df-128">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune_mam_managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="226df-129">Н/Д</span><span class="sxs-lookup"><span data-stu-id="226df-129">Not yet documented</span></span>|
|<span data-ttu-id="226df-130">ИД</span><span class="sxs-lookup"><span data-stu-id="226df-130">id</span></span>|<span data-ttu-id="226df-131">String (строка)</span><span class="sxs-lookup"><span data-stu-id="226df-131">String</span></span>|<span data-ttu-id="226df-132">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="226df-132">Key of the entity.</span></span>|
|<span data-ttu-id="226df-133">версия</span><span class="sxs-lookup"><span data-stu-id="226df-133">version</span></span>|<span data-ttu-id="226df-134">String (строка)</span><span class="sxs-lookup"><span data-stu-id="226df-134">String</span></span>|<span data-ttu-id="226df-135">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="226df-135">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="226df-136">Связи</span><span class="sxs-lookup"><span data-stu-id="226df-136">Relationships</span></span>
<span data-ttu-id="226df-137">Нет</span><span class="sxs-lookup"><span data-stu-id="226df-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="226df-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="226df-138">JSON Representation</span></span>
<span data-ttu-id="226df-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="226df-139">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
  "displayName": "String",
  "configurationDeployedUserCount": 1024,
  "lastRefreshTime": "String (timestamp)",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "String"
      },
      "configurationAppliedUserCount": 1024
    }
  ],
  "id": "String (identifier)",
  "version": "String"
}
```








