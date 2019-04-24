---
title: Тип ресурса managedAppPolicyDeploymentSummary
description: ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 84ca52db1321bc3a2fa356de50e1446f662e725b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465225"
---
# <a name="managedapppolicydeploymentsummary-resource-type"></a><span data-ttu-id="760aa-103">Тип ресурса managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="760aa-103">managedAppPolicyDeploymentSummary resource type</span></span>

> <span data-ttu-id="760aa-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="760aa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="760aa-105">ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="760aa-105">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>

## <a name="methods"></a><span data-ttu-id="760aa-106">Методы</span><span class="sxs-lookup"><span data-stu-id="760aa-106">Methods</span></span>
|<span data-ttu-id="760aa-107">Метод</span><span class="sxs-lookup"><span data-stu-id="760aa-107">Method</span></span>|<span data-ttu-id="760aa-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="760aa-108">Return Type</span></span>|<span data-ttu-id="760aa-109">Описание</span><span class="sxs-lookup"><span data-stu-id="760aa-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="760aa-110">Получение объекта managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="760aa-110">Get managedAppPolicyDeploymentSummary</span></span>](../api/intune-mam-managedapppolicydeploymentsummary-get.md)|<span data-ttu-id="760aa-111">[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md);</span><span class="sxs-lookup"><span data-stu-id="760aa-111">[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md)</span></span>|<span data-ttu-id="760aa-112">Чтение свойств и связей объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="760aa-112">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>|
|[<span data-ttu-id="760aa-113">Обновление объекта managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="760aa-113">Update managedAppPolicyDeploymentSummary</span></span>](../api/intune-mam-managedapppolicydeploymentsummary-update.md)|[<span data-ttu-id="760aa-114">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="760aa-114">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="760aa-115">Обновление свойств объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="760aa-115">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="760aa-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="760aa-116">Properties</span></span>
|<span data-ttu-id="760aa-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="760aa-117">Property</span></span>|<span data-ttu-id="760aa-118">Тип</span><span class="sxs-lookup"><span data-stu-id="760aa-118">Type</span></span>|<span data-ttu-id="760aa-119">Описание</span><span class="sxs-lookup"><span data-stu-id="760aa-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="760aa-120">displayName</span><span class="sxs-lookup"><span data-stu-id="760aa-120">displayName</span></span>|<span data-ttu-id="760aa-121">String</span><span class="sxs-lookup"><span data-stu-id="760aa-121">String</span></span>|<span data-ttu-id="760aa-122">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="760aa-122">Not yet documented</span></span>|
|<span data-ttu-id="760aa-123">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="760aa-123">configurationDeployedUserCount</span></span>|<span data-ttu-id="760aa-124">Int32</span><span class="sxs-lookup"><span data-stu-id="760aa-124">Int32</span></span>|<span data-ttu-id="760aa-125">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="760aa-125">Not yet documented</span></span>|
|<span data-ttu-id="760aa-126">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="760aa-126">lastRefreshTime</span></span>|<span data-ttu-id="760aa-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="760aa-127">DateTimeOffset</span></span>|<span data-ttu-id="760aa-128">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="760aa-128">Not yet documented</span></span>|
|<span data-ttu-id="760aa-129">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="760aa-129">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="760aa-130">Коллекция [managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md)</span><span class="sxs-lookup"><span data-stu-id="760aa-130">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="760aa-131">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="760aa-131">Not yet documented</span></span>|
|<span data-ttu-id="760aa-132">id</span><span class="sxs-lookup"><span data-stu-id="760aa-132">id</span></span>|<span data-ttu-id="760aa-133">String</span><span class="sxs-lookup"><span data-stu-id="760aa-133">String</span></span>|<span data-ttu-id="760aa-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="760aa-134">Key of the entity.</span></span>|
|<span data-ttu-id="760aa-135">version</span><span class="sxs-lookup"><span data-stu-id="760aa-135">version</span></span>|<span data-ttu-id="760aa-136">String</span><span class="sxs-lookup"><span data-stu-id="760aa-136">String</span></span>|<span data-ttu-id="760aa-137">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="760aa-137">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="760aa-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="760aa-138">Relationships</span></span>
<span data-ttu-id="760aa-139">Нет</span><span class="sxs-lookup"><span data-stu-id="760aa-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="760aa-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="760aa-140">JSON Representation</span></span>
<span data-ttu-id="760aa-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="760aa-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummary"
}
-->
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



