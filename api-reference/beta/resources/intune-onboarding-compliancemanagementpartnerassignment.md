---
title: Тип ресурса Комплианцеманажементпартнерассигнмент
description: Нацеленность для группы пользователей для партнера по управлению соответствием требованиям
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4bf6a767c71c7212e0499bb6281e3a0d9477b3cd
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44175261"
---
# <a name="compliancemanagementpartnerassignment-resource-type"></a><span data-ttu-id="1a5f8-103">Тип ресурса Комплианцеманажементпартнерассигнмент</span><span class="sxs-lookup"><span data-stu-id="1a5f8-103">complianceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="1a5f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a5f8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a5f8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a5f8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a5f8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a5f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a5f8-107">Нацеленность для группы пользователей для партнера по управлению соответствием требованиям</span><span class="sxs-lookup"><span data-stu-id="1a5f8-107">User group targeting for Compliance Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="1a5f8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1a5f8-108">Properties</span></span>
|<span data-ttu-id="1a5f8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a5f8-109">Property</span></span>|<span data-ttu-id="1a5f8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1a5f8-110">Type</span></span>|<span data-ttu-id="1a5f8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1a5f8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a5f8-112">target</span><span class="sxs-lookup"><span data-stu-id="1a5f8-112">target</span></span>|[<span data-ttu-id="1a5f8-113">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1a5f8-113">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1a5f8-114">Целевой объект назначения группы.</span><span class="sxs-lookup"><span data-stu-id="1a5f8-114">Group assignment target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a5f8-115">Связи</span><span class="sxs-lookup"><span data-stu-id="1a5f8-115">Relationships</span></span>
<span data-ttu-id="1a5f8-116">Нет</span><span class="sxs-lookup"><span data-stu-id="1a5f8-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a5f8-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1a5f8-117">JSON Representation</span></span>
<span data-ttu-id="1a5f8-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a5f8-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.complianceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  }
}
```



