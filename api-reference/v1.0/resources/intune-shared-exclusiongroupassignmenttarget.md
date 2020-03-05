---
title: Тип ресурса exclusionGroupAssignmentTarget
description: Представляет группу, которую следует исключить из назначения.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 08bf52ab16a29c869366373c5f205f25b352e1b5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447845"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="502cd-103">Тип ресурса exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="502cd-103">exclusionGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="502cd-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="502cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="502cd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="502cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="502cd-106">Представляет группу, которую следует исключить из назначения.</span><span class="sxs-lookup"><span data-stu-id="502cd-106">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="502cd-107">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="502cd-107">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="502cd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="502cd-108">Properties</span></span>
|<span data-ttu-id="502cd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="502cd-109">Property</span></span>|<span data-ttu-id="502cd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="502cd-110">Type</span></span>|<span data-ttu-id="502cd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="502cd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="502cd-112">groupId</span><span class="sxs-lookup"><span data-stu-id="502cd-112">groupId</span></span>|<span data-ttu-id="502cd-113">String</span><span class="sxs-lookup"><span data-stu-id="502cd-113">String</span></span>|<span data-ttu-id="502cd-114">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="502cd-114">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="502cd-115">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="502cd-115">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="502cd-116">Связи</span><span class="sxs-lookup"><span data-stu-id="502cd-116">Relationships</span></span>
<span data-ttu-id="502cd-117">Нет</span><span class="sxs-lookup"><span data-stu-id="502cd-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="502cd-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="502cd-118">JSON Representation</span></span>
<span data-ttu-id="502cd-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="502cd-119">Here is a JSON representation of the resource.</span></span>
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




