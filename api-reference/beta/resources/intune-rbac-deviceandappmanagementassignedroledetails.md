---
title: Тип ресурса Девицеандаппманажементассигнедроледетаилс
description: Набор определений ролей и назначений ролей, назначенных пользователю.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 17a2313b60d4cf843e5b048821a58748c8eb27ca
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523916"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="e2672-103">Тип ресурса Девицеандаппманажементассигнедроледетаилс</span><span class="sxs-lookup"><span data-stu-id="e2672-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

<span data-ttu-id="e2672-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e2672-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2672-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2672-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2672-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e2672-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2672-107">Набор определений ролей и назначений ролей, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="e2672-107">The set of Role Definitions and Role Assignments assigned to a user.</span></span>

## <a name="properties"></a><span data-ttu-id="e2672-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e2672-108">Properties</span></span>
|<span data-ttu-id="e2672-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2672-109">Property</span></span>|<span data-ttu-id="e2672-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e2672-110">Type</span></span>|<span data-ttu-id="e2672-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e2672-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2672-112">роледефинитионидс</span><span class="sxs-lookup"><span data-stu-id="e2672-112">roleDefinitionIds</span></span>|<span data-ttu-id="e2672-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e2672-113">String collection</span></span>|<span data-ttu-id="e2672-114">Идентификаторы определений ролей для определений ролей частности, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="e2672-114">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="e2672-115">ролеассигнментидс</span><span class="sxs-lookup"><span data-stu-id="e2672-115">roleAssignmentIds</span></span>|<span data-ttu-id="e2672-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e2672-116">String collection</span></span>|<span data-ttu-id="e2672-117">Идентификаторы назначения ролей для назначений ролей частности, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="e2672-117">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2672-118">Связи</span><span class="sxs-lookup"><span data-stu-id="e2672-118">Relationships</span></span>
<span data-ttu-id="e2672-119">Нет</span><span class="sxs-lookup"><span data-stu-id="e2672-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2672-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e2672-120">JSON Representation</span></span>
<span data-ttu-id="e2672-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2672-121">Here is a JSON representation of the resource.</span></span>
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



