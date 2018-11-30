---
title: Тип ресурса groupAssignmentTarget
description: Представляет назначение группе.
ms.openlocfilehash: 76ea8c56b8022dc832335c575ad52632894f1d60
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075512"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="66b30-103">Тип ресурса groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="66b30-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="66b30-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="66b30-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66b30-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66b30-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="66b30-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="66b30-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66b30-107">Представляет назначение группе.</span><span class="sxs-lookup"><span data-stu-id="66b30-107">Represents an assignment to a group.</span></span>

<span data-ttu-id="66b30-108">Наследуется от типа [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="66b30-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="66b30-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="66b30-109">Properties</span></span>
|<span data-ttu-id="66b30-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="66b30-110">Property</span></span>|<span data-ttu-id="66b30-111">Тип</span><span class="sxs-lookup"><span data-stu-id="66b30-111">Type</span></span>|<span data-ttu-id="66b30-112">Описание</span><span class="sxs-lookup"><span data-stu-id="66b30-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66b30-113">groupId</span><span class="sxs-lookup"><span data-stu-id="66b30-113">groupId</span></span>|<span data-ttu-id="66b30-114">String</span><span class="sxs-lookup"><span data-stu-id="66b30-114">String</span></span>|<span data-ttu-id="66b30-115">ИД группы, являющейся объектом назначения.</span><span class="sxs-lookup"><span data-stu-id="66b30-115">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66b30-116">Связи</span><span class="sxs-lookup"><span data-stu-id="66b30-116">Relationships</span></span>
<span data-ttu-id="66b30-117">Нет</span><span class="sxs-lookup"><span data-stu-id="66b30-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="66b30-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="66b30-118">JSON Representation</span></span>
<span data-ttu-id="66b30-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66b30-119">Here is a JSON representation of the resource.</span></span>
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





