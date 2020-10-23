---
title: Тип ресурса Девицеманажементпартнерассигнмент
description: Целевая группа пользователей для партнера по управлению устройствами
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e6f329f8f80aab84f069b4b65f8865bfc4220b0d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48718520"
---
# <a name="devicemanagementpartnerassignment-resource-type"></a><span data-ttu-id="30fb9-103">Тип ресурса Девицеманажементпартнерассигнмент</span><span class="sxs-lookup"><span data-stu-id="30fb9-103">deviceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="30fb9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30fb9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="30fb9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30fb9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30fb9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="30fb9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30fb9-107">Целевая группа пользователей для партнера по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="30fb9-107">User group targeting for Device Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="30fb9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="30fb9-108">Properties</span></span>
|<span data-ttu-id="30fb9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="30fb9-109">Property</span></span>|<span data-ttu-id="30fb9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="30fb9-110">Type</span></span>|<span data-ttu-id="30fb9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="30fb9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30fb9-112">target</span><span class="sxs-lookup"><span data-stu-id="30fb9-112">target</span></span>|[<span data-ttu-id="30fb9-113">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="30fb9-113">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="30fb9-114">Группы пользователей, предназначенные для регистрации устройств с помощью партнера.</span><span class="sxs-lookup"><span data-stu-id="30fb9-114">User groups targeting for devices to be enrolled through partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="30fb9-115">Связи</span><span class="sxs-lookup"><span data-stu-id="30fb9-115">Relationships</span></span>
<span data-ttu-id="30fb9-116">Нет</span><span class="sxs-lookup"><span data-stu-id="30fb9-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="30fb9-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="30fb9-117">JSON Representation</span></span>
<span data-ttu-id="30fb9-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30fb9-118">Here is a JSON representation of the resource.</span></span>
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





