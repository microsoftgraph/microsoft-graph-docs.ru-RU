---
title: Тип ресурса Девицеманажементпартнерассигнмент
description: Целевая группа пользователей для партнера по управлению устройствами
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3be5d3326ac5ee1c9446590ac79a9572c04819a6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49307418"
---
# <a name="devicemanagementpartnerassignment-resource-type"></a><span data-ttu-id="186a5-103">Тип ресурса Девицеманажементпартнерассигнмент</span><span class="sxs-lookup"><span data-stu-id="186a5-103">deviceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="186a5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="186a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="186a5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="186a5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="186a5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="186a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="186a5-107">Целевая группа пользователей для партнера по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="186a5-107">User group targeting for Device Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="186a5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="186a5-108">Properties</span></span>
|<span data-ttu-id="186a5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="186a5-109">Property</span></span>|<span data-ttu-id="186a5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="186a5-110">Type</span></span>|<span data-ttu-id="186a5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="186a5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="186a5-112">target</span><span class="sxs-lookup"><span data-stu-id="186a5-112">target</span></span>|[<span data-ttu-id="186a5-113">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="186a5-113">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="186a5-114">Группы пользователей, предназначенные для регистрации устройств с помощью партнера.</span><span class="sxs-lookup"><span data-stu-id="186a5-114">User groups targeting for devices to be enrolled through partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="186a5-115">Связи</span><span class="sxs-lookup"><span data-stu-id="186a5-115">Relationships</span></span>
<span data-ttu-id="186a5-116">Нет</span><span class="sxs-lookup"><span data-stu-id="186a5-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="186a5-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="186a5-117">JSON Representation</span></span>
<span data-ttu-id="186a5-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="186a5-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```




