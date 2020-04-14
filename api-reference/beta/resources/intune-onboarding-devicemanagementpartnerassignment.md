---
title: Тип ресурса Девицеманажементпартнерассигнмент
description: Целевая группа пользователей для партнера по управлению устройствами
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4bee2745c7757ed31d18c3a05916b1e9aa0bec41
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455653"
---
# <a name="devicemanagementpartnerassignment-resource-type"></a><span data-ttu-id="5549d-103">Тип ресурса Девицеманажементпартнерассигнмент</span><span class="sxs-lookup"><span data-stu-id="5549d-103">deviceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="5549d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5549d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5549d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5549d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5549d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5549d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5549d-107">Целевая группа пользователей для партнера по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="5549d-107">User group targeting for Device Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="5549d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5549d-108">Properties</span></span>
|<span data-ttu-id="5549d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5549d-109">Property</span></span>|<span data-ttu-id="5549d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5549d-110">Type</span></span>|<span data-ttu-id="5549d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5549d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5549d-112">target</span><span class="sxs-lookup"><span data-stu-id="5549d-112">target</span></span>|[<span data-ttu-id="5549d-113">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5549d-113">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5549d-114">Группы пользователей, предназначенные для регистрации устройств с помощью партнера.</span><span class="sxs-lookup"><span data-stu-id="5549d-114">User groups targeting for devices to be enrolled through partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5549d-115">Связи</span><span class="sxs-lookup"><span data-stu-id="5549d-115">Relationships</span></span>
<span data-ttu-id="5549d-116">Нет</span><span class="sxs-lookup"><span data-stu-id="5549d-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5549d-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5549d-117">JSON Representation</span></span>
<span data-ttu-id="5549d-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5549d-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



