---
title: Тип ресурса exclusionGroupAssignmentTarget
description: Представляет группу, которую следует исключить из назначения.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2d2d6b004b6dbd78b43d4cab1c06e960d43f30d7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917225"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="d6af4-103">Тип ресурса exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d6af4-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="d6af4-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d6af4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6af4-105">Представляет группу, которую следует исключить из назначения.</span><span class="sxs-lookup"><span data-stu-id="d6af4-105">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="d6af4-106">Наследуется от [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="d6af4-106">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d6af4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d6af4-107">Properties</span></span>
|<span data-ttu-id="d6af4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6af4-108">Property</span></span>|<span data-ttu-id="d6af4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d6af4-109">Type</span></span>|<span data-ttu-id="d6af4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d6af4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6af4-111">groupId</span><span class="sxs-lookup"><span data-stu-id="d6af4-111">groupId</span></span>|<span data-ttu-id="d6af4-112">Строка</span><span class="sxs-lookup"><span data-stu-id="d6af4-112">String</span></span>|<span data-ttu-id="d6af4-113">ИД группы, являющейся объектом назначения.</span><span class="sxs-lookup"><span data-stu-id="d6af4-113">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="d6af4-114">Наследуется от [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="d6af4-114">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6af4-115">Связи</span><span class="sxs-lookup"><span data-stu-id="d6af4-115">Relationships</span></span>
<span data-ttu-id="d6af4-116">Нет</span><span class="sxs-lookup"><span data-stu-id="d6af4-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d6af4-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d6af4-117">JSON Representation</span></span>
<span data-ttu-id="d6af4-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6af4-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "groupId": "String"
}
```



