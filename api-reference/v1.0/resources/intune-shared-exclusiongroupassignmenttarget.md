---
title: Тип ресурса exclusionGroupAssignmentTarget
description: Представляет группу, которую следует исключить из назначения.
ms.openlocfilehash: fdbb463687d75791965db2ef05abfea1a269d1a1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027033"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="edcab-103">Тип ресурса exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="edcab-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="edcab-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="edcab-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="edcab-105">Представляет группу, которую следует исключить из назначения.</span><span class="sxs-lookup"><span data-stu-id="edcab-105">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="edcab-106">Наследуется от [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="edcab-106">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="edcab-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="edcab-107">Properties</span></span>
|<span data-ttu-id="edcab-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="edcab-108">Property</span></span>|<span data-ttu-id="edcab-109">Тип</span><span class="sxs-lookup"><span data-stu-id="edcab-109">Type</span></span>|<span data-ttu-id="edcab-110">Описание</span><span class="sxs-lookup"><span data-stu-id="edcab-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edcab-111">groupId</span><span class="sxs-lookup"><span data-stu-id="edcab-111">groupId</span></span>|<span data-ttu-id="edcab-112">String</span><span class="sxs-lookup"><span data-stu-id="edcab-112">String</span></span>|<span data-ttu-id="edcab-113">ИД группы, являющейся объектом назначения.</span><span class="sxs-lookup"><span data-stu-id="edcab-113">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="edcab-114">Наследуется от [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="edcab-114">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="edcab-115">Связи</span><span class="sxs-lookup"><span data-stu-id="edcab-115">Relationships</span></span>
<span data-ttu-id="edcab-116">Нет</span><span class="sxs-lookup"><span data-stu-id="edcab-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="edcab-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="edcab-117">JSON Representation</span></span>
<span data-ttu-id="edcab-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="edcab-118">Here is a JSON representation of the resource.</span></span>
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



