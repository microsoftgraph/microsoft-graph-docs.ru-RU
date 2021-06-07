---
title: Тип ресурса groupAssignmentTarget
description: Представляет ресурс, назначенный группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d90440ee70ad701b3bb19f159cda53a1355fc7f0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756766"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="2a0f2-103">Тип ресурса groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2a0f2-103">groupAssignmentTarget resource type</span></span>

<span data-ttu-id="2a0f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a0f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a0f2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2a0f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a0f2-106">Представляет ресурс, назначенный группе.</span><span class="sxs-lookup"><span data-stu-id="2a0f2-106">Represents an assignment to a group.</span></span>


<span data-ttu-id="2a0f2-107">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="2a0f2-107">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2a0f2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2a0f2-108">Properties</span></span>
|<span data-ttu-id="2a0f2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a0f2-109">Property</span></span>|<span data-ttu-id="2a0f2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2a0f2-110">Type</span></span>|<span data-ttu-id="2a0f2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2a0f2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a0f2-112">groupId</span><span class="sxs-lookup"><span data-stu-id="2a0f2-112">groupId</span></span>|<span data-ttu-id="2a0f2-113">String</span><span class="sxs-lookup"><span data-stu-id="2a0f2-113">String</span></span>|<span data-ttu-id="2a0f2-114">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="2a0f2-114">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a0f2-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="2a0f2-115">Relationships</span></span>
<span data-ttu-id="2a0f2-116">Нет</span><span class="sxs-lookup"><span data-stu-id="2a0f2-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a0f2-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2a0f2-117">JSON Representation</span></span>
<span data-ttu-id="2a0f2-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a0f2-118">Here is a JSON representation of the resource.</span></span>
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




