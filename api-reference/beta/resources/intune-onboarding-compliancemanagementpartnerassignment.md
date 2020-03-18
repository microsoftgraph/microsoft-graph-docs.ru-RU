---
title: Тип ресурса Комплианцеманажементпартнерассигнмент
description: Нацеленность для группы пользователей для партнера по управлению соответствием требованиям
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 83652eb419566836c349fd2f12160516710c710b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42779802"
---
# <a name="compliancemanagementpartnerassignment-resource-type"></a><span data-ttu-id="6980c-103">Тип ресурса Комплианцеманажементпартнерассигнмент</span><span class="sxs-lookup"><span data-stu-id="6980c-103">complianceManagementPartnerAssignment resource type</span></span>

> <span data-ttu-id="6980c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6980c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6980c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6980c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6980c-106">Нацеленность для группы пользователей для партнера по управлению соответствием требованиям</span><span class="sxs-lookup"><span data-stu-id="6980c-106">User group targeting for Compliance Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="6980c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6980c-107">Properties</span></span>
|<span data-ttu-id="6980c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6980c-108">Property</span></span>|<span data-ttu-id="6980c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6980c-109">Type</span></span>|<span data-ttu-id="6980c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6980c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6980c-111">target</span><span class="sxs-lookup"><span data-stu-id="6980c-111">target</span></span>|[<span data-ttu-id="6980c-112">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6980c-112">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6980c-113">Целевой объект назначения группы.</span><span class="sxs-lookup"><span data-stu-id="6980c-113">Group assignment target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6980c-114">Связи</span><span class="sxs-lookup"><span data-stu-id="6980c-114">Relationships</span></span>
<span data-ttu-id="6980c-115">Нет</span><span class="sxs-lookup"><span data-stu-id="6980c-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6980c-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6980c-116">JSON Representation</span></span>
<span data-ttu-id="6980c-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6980c-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.complianceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



