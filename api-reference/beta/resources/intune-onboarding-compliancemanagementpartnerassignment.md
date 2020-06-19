---
title: Тип ресурса Комплианцеманажементпартнерассигнмент
description: Нацеленность для группы пользователей для партнера по управлению соответствием требованиям
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 04157461b1990403be4a60992876bb9a46317f1b
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793817"
---
# <a name="compliancemanagementpartnerassignment-resource-type"></a><span data-ttu-id="1af94-103">Тип ресурса Комплианцеманажементпартнерассигнмент</span><span class="sxs-lookup"><span data-stu-id="1af94-103">complianceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="1af94-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1af94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1af94-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1af94-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1af94-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1af94-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1af94-107">Нацеленность для группы пользователей для партнера по управлению соответствием требованиям</span><span class="sxs-lookup"><span data-stu-id="1af94-107">User group targeting for Compliance Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="1af94-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1af94-108">Properties</span></span>
|<span data-ttu-id="1af94-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1af94-109">Property</span></span>|<span data-ttu-id="1af94-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1af94-110">Type</span></span>|<span data-ttu-id="1af94-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1af94-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1af94-112">target</span><span class="sxs-lookup"><span data-stu-id="1af94-112">target</span></span>|[<span data-ttu-id="1af94-113">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1af94-113">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1af94-114">Целевой объект назначения группы.</span><span class="sxs-lookup"><span data-stu-id="1af94-114">Group assignment target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1af94-115">Связи</span><span class="sxs-lookup"><span data-stu-id="1af94-115">Relationships</span></span>
<span data-ttu-id="1af94-116">Нет</span><span class="sxs-lookup"><span data-stu-id="1af94-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1af94-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1af94-117">JSON Representation</span></span>
<span data-ttu-id="1af94-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1af94-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.complianceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```



