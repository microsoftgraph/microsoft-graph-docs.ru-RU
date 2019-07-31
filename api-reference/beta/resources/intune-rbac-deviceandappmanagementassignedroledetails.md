---
title: Тип ресурса Девицеандаппманажементассигнедроледетаилс
description: Набор определений ролей и назначений ролей, назначенных пользователю.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: beadac8ef20d1a716369626c52664af3ef8d9042
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967674"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="e87d6-103">Тип ресурса Девицеандаппманажементассигнедроледетаилс</span><span class="sxs-lookup"><span data-stu-id="e87d6-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

> <span data-ttu-id="e87d6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e87d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e87d6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e87d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e87d6-106">Набор определений ролей и назначений ролей, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="e87d6-106">The set of Role Definitions and Role Assignments assigned to a user.</span></span>

## <a name="properties"></a><span data-ttu-id="e87d6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e87d6-107">Properties</span></span>
|<span data-ttu-id="e87d6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e87d6-108">Property</span></span>|<span data-ttu-id="e87d6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e87d6-109">Type</span></span>|<span data-ttu-id="e87d6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e87d6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e87d6-111">Роледефинитионидс</span><span class="sxs-lookup"><span data-stu-id="e87d6-111">roleDefinitionIds</span></span>|<span data-ttu-id="e87d6-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e87d6-112">String collection</span></span>|<span data-ttu-id="e87d6-113">Идентификаторы определений ролей для определений ролей частности, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="e87d6-113">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="e87d6-114">Ролеассигнментидс</span><span class="sxs-lookup"><span data-stu-id="e87d6-114">roleAssignmentIds</span></span>|<span data-ttu-id="e87d6-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e87d6-115">String collection</span></span>|<span data-ttu-id="e87d6-116">Идентификаторы назначения ролей для назначений ролей частности, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="e87d6-116">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e87d6-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="e87d6-117">Relationships</span></span>
<span data-ttu-id="e87d6-118">Нет</span><span class="sxs-lookup"><span data-stu-id="e87d6-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e87d6-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e87d6-119">JSON Representation</span></span>
<span data-ttu-id="e87d6-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e87d6-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignedRoleDetails",
  "roleDefinitionIds": [
    "String"
  ],
  "roleAssignmentIds": [
    "String"
  ]
}
```





