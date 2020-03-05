---
title: Тип ресурса groupAssignmentTarget
description: Представляет ресурс, назначенный группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4b15df3fab9303f56e697eb09305db50d3ddea8b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523676"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="ef299-103">Тип ресурса groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ef299-103">groupAssignmentTarget resource type</span></span>

<span data-ttu-id="ef299-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ef299-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef299-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef299-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef299-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef299-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef299-107">Представляет ресурс, назначенный группе.</span><span class="sxs-lookup"><span data-stu-id="ef299-107">Represents an assignment to a group.</span></span>


<span data-ttu-id="ef299-108">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="ef299-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ef299-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ef299-109">Properties</span></span>
|<span data-ttu-id="ef299-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef299-110">Property</span></span>|<span data-ttu-id="ef299-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ef299-111">Type</span></span>|<span data-ttu-id="ef299-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ef299-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef299-113">groupId</span><span class="sxs-lookup"><span data-stu-id="ef299-113">groupId</span></span>|<span data-ttu-id="ef299-114">String</span><span class="sxs-lookup"><span data-stu-id="ef299-114">String</span></span>|<span data-ttu-id="ef299-115">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="ef299-115">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef299-116">Связи</span><span class="sxs-lookup"><span data-stu-id="ef299-116">Relationships</span></span>
<span data-ttu-id="ef299-117">Нет</span><span class="sxs-lookup"><span data-stu-id="ef299-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ef299-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ef299-118">JSON Representation</span></span>
<span data-ttu-id="ef299-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef299-119">Here is a JSON representation of the resource.</span></span>
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



