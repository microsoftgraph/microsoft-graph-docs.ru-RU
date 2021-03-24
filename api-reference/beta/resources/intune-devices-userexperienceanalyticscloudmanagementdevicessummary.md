---
title: тип ресурса userExperienceAnalyticsCloudManagementDevicesSummary
description: Пользовательский интерфейс работает в любом месте сводки устройств облачного управления.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f0fb4e7d9a8ac5b2ab9c134d45c2e625a935b491
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146833"
---
# <a name="userexperienceanalyticscloudmanagementdevicessummary-resource-type"></a><span data-ttu-id="5ff66-103">тип ресурса userExperienceAnalyticsCloudManagementDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="5ff66-103">userExperienceAnalyticsCloudManagementDevicesSummary resource type</span></span>

<span data-ttu-id="5ff66-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ff66-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ff66-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ff66-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ff66-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5ff66-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ff66-107">Пользовательский интерфейс работает в любом месте сводки устройств облачного управления.</span><span class="sxs-lookup"><span data-stu-id="5ff66-107">The user experience work from anywhere Cloud management devices summary.</span></span>

## <a name="properties"></a><span data-ttu-id="5ff66-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5ff66-108">Properties</span></span>
|<span data-ttu-id="5ff66-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ff66-109">Property</span></span>|<span data-ttu-id="5ff66-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5ff66-110">Type</span></span>|<span data-ttu-id="5ff66-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5ff66-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ff66-112">coManagedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ff66-112">coManagedDeviceCount</span></span>|<span data-ttu-id="5ff66-113">Int32</span><span class="sxs-lookup"><span data-stu-id="5ff66-113">Int32</span></span>|<span data-ttu-id="5ff66-114">Общее количество совместно управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="5ff66-114">Total number of  co-managed devices.</span></span>|
|<span data-ttu-id="5ff66-115">intuneDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ff66-115">intuneDeviceCount</span></span>|<span data-ttu-id="5ff66-116">Int32</span><span class="sxs-lookup"><span data-stu-id="5ff66-116">Int32</span></span>|<span data-ttu-id="5ff66-117">Количество устройств intune, которые не зарегистрированы автопилотом.</span><span class="sxs-lookup"><span data-stu-id="5ff66-117">The count of intune devices that are not autopilot registerd.</span></span>|
|<span data-ttu-id="5ff66-118">tenantAttachDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ff66-118">tenantAttachDeviceCount</span></span>|<span data-ttu-id="5ff66-119">Int32</span><span class="sxs-lookup"><span data-stu-id="5ff66-119">Int32</span></span>|<span data-ttu-id="5ff66-120">Общее количество устройств присоединений клиента.</span><span class="sxs-lookup"><span data-stu-id="5ff66-120">Total count of tenant attach devices.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ff66-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="5ff66-121">Relationships</span></span>
<span data-ttu-id="5ff66-122">Нет</span><span class="sxs-lookup"><span data-stu-id="5ff66-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ff66-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5ff66-123">JSON Representation</span></span>
<span data-ttu-id="5ff66-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ff66-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsCloudManagementDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCloudManagementDevicesSummary",
  "coManagedDeviceCount": 1024,
  "intuneDeviceCount": 1024,
  "tenantAttachDeviceCount": 1024
}
```




