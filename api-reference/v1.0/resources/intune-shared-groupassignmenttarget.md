---
title: Тип ресурса groupAssignmentTarget
description: Представляет назначение группе.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e2928817a4d8bf287c3a941ddea80e7a3c4e19fd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951721"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="c8f57-103">Тип ресурса groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c8f57-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="c8f57-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c8f57-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8f57-105">Представляет назначение группе.</span><span class="sxs-lookup"><span data-stu-id="c8f57-105">Represents an assignment to a group.</span></span>

<span data-ttu-id="c8f57-106">Наследуется от типа [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="c8f57-106">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c8f57-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c8f57-107">Properties</span></span>
|<span data-ttu-id="c8f57-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8f57-108">Property</span></span>|<span data-ttu-id="c8f57-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c8f57-109">Type</span></span>|<span data-ttu-id="c8f57-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c8f57-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8f57-111">groupId</span><span class="sxs-lookup"><span data-stu-id="c8f57-111">groupId</span></span>|<span data-ttu-id="c8f57-112">Строка</span><span class="sxs-lookup"><span data-stu-id="c8f57-112">String</span></span>|<span data-ttu-id="c8f57-113">ИД группы, являющейся объектом назначения.</span><span class="sxs-lookup"><span data-stu-id="c8f57-113">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8f57-114">Связи</span><span class="sxs-lookup"><span data-stu-id="c8f57-114">Relationships</span></span>
<span data-ttu-id="c8f57-115">Нет</span><span class="sxs-lookup"><span data-stu-id="c8f57-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c8f57-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c8f57-116">JSON Representation</span></span>
<span data-ttu-id="c8f57-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8f57-117">Here is a JSON representation of the resource.</span></span>
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



