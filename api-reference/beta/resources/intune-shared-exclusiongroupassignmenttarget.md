---
title: Тип ресурса exclusionGroupAssignmentTarget
description: Представляет группу, которую следует исключить из назначения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 390c9de591af10dc19df7bc989b9fa01ef59f86a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527428"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="13b08-103">Тип ресурса exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="13b08-103">exclusionGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="13b08-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="13b08-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13b08-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13b08-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13b08-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13b08-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13b08-107">Представляет группу, которую следует исключить из назначения.</span><span class="sxs-lookup"><span data-stu-id="13b08-107">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="13b08-108">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="13b08-108">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="13b08-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="13b08-109">Properties</span></span>
|<span data-ttu-id="13b08-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="13b08-110">Property</span></span>|<span data-ttu-id="13b08-111">Тип</span><span class="sxs-lookup"><span data-stu-id="13b08-111">Type</span></span>|<span data-ttu-id="13b08-112">Описание</span><span class="sxs-lookup"><span data-stu-id="13b08-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13b08-113">groupId</span><span class="sxs-lookup"><span data-stu-id="13b08-113">groupId</span></span>|<span data-ttu-id="13b08-114">String</span><span class="sxs-lookup"><span data-stu-id="13b08-114">String</span></span>|<span data-ttu-id="13b08-115">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="13b08-115">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="13b08-116">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="13b08-116">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="13b08-117">Связи</span><span class="sxs-lookup"><span data-stu-id="13b08-117">Relationships</span></span>
<span data-ttu-id="13b08-118">Нет</span><span class="sxs-lookup"><span data-stu-id="13b08-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13b08-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="13b08-119">JSON Representation</span></span>
<span data-ttu-id="13b08-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13b08-120">Here is a JSON representation of the resource.</span></span>
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



