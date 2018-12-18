---
title: Тип ресурса exclusionGroupAssignmentTarget
description: Представляет группу, которую следует исключить из назначения.
author: tfitzmac
ms.openlocfilehash: 783231c451668169ba85e8ce1cfecd669b5c0b7d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343185"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="313b4-103">Тип ресурса exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="313b4-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="313b4-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="313b4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="313b4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="313b4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="313b4-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="313b4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="313b4-107">Представляет группу, которую следует исключить из назначения.</span><span class="sxs-lookup"><span data-stu-id="313b4-107">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="313b4-108">Наследуется от [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="313b4-108">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="313b4-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="313b4-109">Properties</span></span>
|<span data-ttu-id="313b4-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="313b4-110">Property</span></span>|<span data-ttu-id="313b4-111">Тип</span><span class="sxs-lookup"><span data-stu-id="313b4-111">Type</span></span>|<span data-ttu-id="313b4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="313b4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="313b4-113">groupId</span><span class="sxs-lookup"><span data-stu-id="313b4-113">groupId</span></span>|<span data-ttu-id="313b4-114">Строка</span><span class="sxs-lookup"><span data-stu-id="313b4-114">String</span></span>|<span data-ttu-id="313b4-115">ИД группы, являющейся объектом назначения.</span><span class="sxs-lookup"><span data-stu-id="313b4-115">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="313b4-116">Наследуется от [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="313b4-116">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="313b4-117">Связи</span><span class="sxs-lookup"><span data-stu-id="313b4-117">Relationships</span></span>
<span data-ttu-id="313b4-118">Нет</span><span class="sxs-lookup"><span data-stu-id="313b4-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="313b4-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="313b4-119">JSON Representation</span></span>
<span data-ttu-id="313b4-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="313b4-120">Here is a JSON representation of the resource.</span></span>
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





