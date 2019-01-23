---
title: Тип ресурса groupAssignmentTarget
description: Представляет назначение группе.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2039f5917aa5d69b74ccb6c1732496dc567ab673
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399425"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="4960d-103">Тип ресурса groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4960d-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="4960d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4960d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4960d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4960d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4960d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4960d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4960d-107">Представляет назначение группе.</span><span class="sxs-lookup"><span data-stu-id="4960d-107">Represents an assignment to a group.</span></span>


<span data-ttu-id="4960d-108">Наследуется от типа [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="4960d-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4960d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4960d-109">Properties</span></span>
|<span data-ttu-id="4960d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4960d-110">Property</span></span>|<span data-ttu-id="4960d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4960d-111">Type</span></span>|<span data-ttu-id="4960d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4960d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4960d-113">groupId</span><span class="sxs-lookup"><span data-stu-id="4960d-113">groupId</span></span>|<span data-ttu-id="4960d-114">String</span><span class="sxs-lookup"><span data-stu-id="4960d-114">String</span></span>|<span data-ttu-id="4960d-115">ИД группы, являющейся объектом назначения.</span><span class="sxs-lookup"><span data-stu-id="4960d-115">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4960d-116">Связи</span><span class="sxs-lookup"><span data-stu-id="4960d-116">Relationships</span></span>
<span data-ttu-id="4960d-117">Нет</span><span class="sxs-lookup"><span data-stu-id="4960d-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4960d-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4960d-118">JSON Representation</span></span>
<span data-ttu-id="4960d-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4960d-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupAssignmentTarget",
  "groupId": "String"
}
```




