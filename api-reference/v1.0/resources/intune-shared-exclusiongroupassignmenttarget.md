---
title: Тип ресурса exclusionGroupAssignmentTarget
description: Представляет группу, которую следует исключить из назначения.
author: tfitzmac
ms.openlocfilehash: 8193ac714f7f68dc371454c809c3eaa3176f8453
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304517"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="670e6-103">Тип ресурса exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="670e6-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="670e6-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="670e6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="670e6-105">Представляет группу, которую следует исключить из назначения.</span><span class="sxs-lookup"><span data-stu-id="670e6-105">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="670e6-106">Наследуется от [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="670e6-106">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="670e6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="670e6-107">Properties</span></span>
|<span data-ttu-id="670e6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="670e6-108">Property</span></span>|<span data-ttu-id="670e6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="670e6-109">Type</span></span>|<span data-ttu-id="670e6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="670e6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="670e6-111">groupId</span><span class="sxs-lookup"><span data-stu-id="670e6-111">groupId</span></span>|<span data-ttu-id="670e6-112">Строка</span><span class="sxs-lookup"><span data-stu-id="670e6-112">String</span></span>|<span data-ttu-id="670e6-113">ИД группы, являющейся объектом назначения.</span><span class="sxs-lookup"><span data-stu-id="670e6-113">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="670e6-114">Наследуется от [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="670e6-114">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="670e6-115">Связи</span><span class="sxs-lookup"><span data-stu-id="670e6-115">Relationships</span></span>
<span data-ttu-id="670e6-116">Нет</span><span class="sxs-lookup"><span data-stu-id="670e6-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="670e6-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="670e6-117">JSON Representation</span></span>
<span data-ttu-id="670e6-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="670e6-118">Here is a JSON representation of the resource.</span></span>
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



