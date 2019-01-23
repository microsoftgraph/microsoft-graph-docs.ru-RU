---
title: Тип ресурса exclusionGroupAssignmentTarget
description: Представляет группу, которую следует исключить из назначения.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a42cab192a9cd643c6c11de596ca0790fa8b4a5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421888"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="15c42-103">Тип ресурса exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="15c42-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="15c42-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="15c42-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="15c42-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15c42-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15c42-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15c42-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15c42-107">Представляет группу, которую следует исключить из назначения.</span><span class="sxs-lookup"><span data-stu-id="15c42-107">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="15c42-108">Наследуется от [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="15c42-108">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="15c42-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="15c42-109">Properties</span></span>
|<span data-ttu-id="15c42-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="15c42-110">Property</span></span>|<span data-ttu-id="15c42-111">Тип</span><span class="sxs-lookup"><span data-stu-id="15c42-111">Type</span></span>|<span data-ttu-id="15c42-112">Описание</span><span class="sxs-lookup"><span data-stu-id="15c42-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15c42-113">groupId</span><span class="sxs-lookup"><span data-stu-id="15c42-113">groupId</span></span>|<span data-ttu-id="15c42-114">String</span><span class="sxs-lookup"><span data-stu-id="15c42-114">String</span></span>|<span data-ttu-id="15c42-115">ИД группы, являющейся объектом назначения.</span><span class="sxs-lookup"><span data-stu-id="15c42-115">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="15c42-116">Наследуется от [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="15c42-116">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="15c42-117">Связи</span><span class="sxs-lookup"><span data-stu-id="15c42-117">Relationships</span></span>
<span data-ttu-id="15c42-118">Нет</span><span class="sxs-lookup"><span data-stu-id="15c42-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="15c42-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="15c42-119">JSON Representation</span></span>
<span data-ttu-id="15c42-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15c42-120">Here is a JSON representation of the resource.</span></span>
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




