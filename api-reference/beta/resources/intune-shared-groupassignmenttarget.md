---
title: Тип ресурса groupAssignmentTarget
description: Представляет ресурс, назначенный группе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d67b7789f30dd1226c7918e734d615db4ee83ac
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550653"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="902d9-103">Тип ресурса groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="902d9-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="902d9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="902d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="902d9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="902d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="902d9-106">Представляет ресурс, назначенный группе.</span><span class="sxs-lookup"><span data-stu-id="902d9-106">Represents an assignment to a group.</span></span>


<span data-ttu-id="902d9-107">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="902d9-107">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="902d9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="902d9-108">Properties</span></span>
|<span data-ttu-id="902d9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="902d9-109">Property</span></span>|<span data-ttu-id="902d9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="902d9-110">Type</span></span>|<span data-ttu-id="902d9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="902d9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="902d9-112">groupId</span><span class="sxs-lookup"><span data-stu-id="902d9-112">groupId</span></span>|<span data-ttu-id="902d9-113">String</span><span class="sxs-lookup"><span data-stu-id="902d9-113">String</span></span>|<span data-ttu-id="902d9-114">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="902d9-114">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="902d9-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="902d9-115">Relationships</span></span>
<span data-ttu-id="902d9-116">Нет</span><span class="sxs-lookup"><span data-stu-id="902d9-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="902d9-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="902d9-117">JSON Representation</span></span>
<span data-ttu-id="902d9-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="902d9-118">Here is a JSON representation of the resource.</span></span>
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





