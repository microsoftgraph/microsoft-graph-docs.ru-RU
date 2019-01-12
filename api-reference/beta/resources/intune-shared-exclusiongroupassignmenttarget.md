---
title: Тип ресурса exclusionGroupAssignmentTarget
description: Представляет группу, которую следует исключить из назначения.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 24e732bc0c48c9c25f35da1afbccef04d17fe0cb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919865"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="a6388-103">Тип ресурса exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a6388-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="a6388-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a6388-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6388-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6388-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a6388-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a6388-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6388-107">Представляет группу, которую следует исключить из назначения.</span><span class="sxs-lookup"><span data-stu-id="a6388-107">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="a6388-108">Наследуется от [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="a6388-108">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a6388-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a6388-109">Properties</span></span>
|<span data-ttu-id="a6388-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6388-110">Property</span></span>|<span data-ttu-id="a6388-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a6388-111">Type</span></span>|<span data-ttu-id="a6388-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a6388-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6388-113">groupId</span><span class="sxs-lookup"><span data-stu-id="a6388-113">groupId</span></span>|<span data-ttu-id="a6388-114">Строка</span><span class="sxs-lookup"><span data-stu-id="a6388-114">String</span></span>|<span data-ttu-id="a6388-115">ИД группы, являющейся объектом назначения.</span><span class="sxs-lookup"><span data-stu-id="a6388-115">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="a6388-116">Наследуется от [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="a6388-116">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6388-117">Связи</span><span class="sxs-lookup"><span data-stu-id="a6388-117">Relationships</span></span>
<span data-ttu-id="a6388-118">Нет</span><span class="sxs-lookup"><span data-stu-id="a6388-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a6388-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a6388-119">JSON Representation</span></span>
<span data-ttu-id="a6388-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6388-120">Here is a JSON representation of the resource.</span></span>
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





