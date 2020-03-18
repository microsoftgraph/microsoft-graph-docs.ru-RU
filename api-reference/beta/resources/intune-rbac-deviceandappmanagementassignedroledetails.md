---
title: Тип ресурса Девицеандаппманажементассигнедроледетаилс
description: Набор определений ролей и назначений ролей, назначенных пользователю.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f1590470f436dac6572ebf9d0430d144060f9b7f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42773947"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="bc6ee-103">Тип ресурса Девицеандаппманажементассигнедроледетаилс</span><span class="sxs-lookup"><span data-stu-id="bc6ee-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

> <span data-ttu-id="bc6ee-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc6ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc6ee-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bc6ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc6ee-106">Набор определений ролей и назначений ролей, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="bc6ee-106">The set of Role Definitions and Role Assignments assigned to a user.</span></span>

## <a name="properties"></a><span data-ttu-id="bc6ee-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc6ee-107">Properties</span></span>
|<span data-ttu-id="bc6ee-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc6ee-108">Property</span></span>|<span data-ttu-id="bc6ee-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bc6ee-109">Type</span></span>|<span data-ttu-id="bc6ee-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bc6ee-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc6ee-111">роледефинитионидс</span><span class="sxs-lookup"><span data-stu-id="bc6ee-111">roleDefinitionIds</span></span>|<span data-ttu-id="bc6ee-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bc6ee-112">String collection</span></span>|<span data-ttu-id="bc6ee-113">Идентификаторы определений ролей для определений ролей частности, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="bc6ee-113">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="bc6ee-114">ролеассигнментидс</span><span class="sxs-lookup"><span data-stu-id="bc6ee-114">roleAssignmentIds</span></span>|<span data-ttu-id="bc6ee-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bc6ee-115">String collection</span></span>|<span data-ttu-id="bc6ee-116">Идентификаторы назначения ролей для назначений ролей частности, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="bc6ee-116">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc6ee-117">Связи</span><span class="sxs-lookup"><span data-stu-id="bc6ee-117">Relationships</span></span>
<span data-ttu-id="bc6ee-118">Нет</span><span class="sxs-lookup"><span data-stu-id="bc6ee-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc6ee-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc6ee-119">JSON Representation</span></span>
<span data-ttu-id="bc6ee-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc6ee-120">Here is a JSON representation of the resource.</span></span>
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



