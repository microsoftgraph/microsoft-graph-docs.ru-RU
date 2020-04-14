---
title: Тип ресурса groupAssignmentTarget
description: Представляет ресурс, назначенный группе.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3bb1de3dbd95145bc7f1ce631175e9867deb1dde
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43407696"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="34019-103">Тип ресурса groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="34019-103">groupAssignmentTarget resource type</span></span>

<span data-ttu-id="34019-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34019-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34019-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34019-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34019-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="34019-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34019-107">Представляет ресурс, назначенный группе.</span><span class="sxs-lookup"><span data-stu-id="34019-107">Represents an assignment to a group.</span></span>


<span data-ttu-id="34019-108">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="34019-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="34019-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="34019-109">Properties</span></span>
|<span data-ttu-id="34019-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="34019-110">Property</span></span>|<span data-ttu-id="34019-111">Тип</span><span class="sxs-lookup"><span data-stu-id="34019-111">Type</span></span>|<span data-ttu-id="34019-112">Описание</span><span class="sxs-lookup"><span data-stu-id="34019-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34019-113">groupId</span><span class="sxs-lookup"><span data-stu-id="34019-113">groupId</span></span>|<span data-ttu-id="34019-114">String</span><span class="sxs-lookup"><span data-stu-id="34019-114">String</span></span>|<span data-ttu-id="34019-115">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="34019-115">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34019-116">Связи</span><span class="sxs-lookup"><span data-stu-id="34019-116">Relationships</span></span>
<span data-ttu-id="34019-117">Нет</span><span class="sxs-lookup"><span data-stu-id="34019-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34019-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="34019-118">JSON Representation</span></span>
<span data-ttu-id="34019-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34019-119">Here is a JSON representation of the resource.</span></span>
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



