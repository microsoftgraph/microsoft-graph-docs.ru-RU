---
title: Тип ресурса Девицеандаппманажементассигнедроледетаилс
description: Набор определений ролей и назначений ролей, назначенных пользователю.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 216f8d8d36eca7402667d713b44a9d10f14d0999
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49266244"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="ea847-103">Тип ресурса Девицеандаппманажементассигнедроледетаилс</span><span class="sxs-lookup"><span data-stu-id="ea847-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

<span data-ttu-id="ea847-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea847-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea847-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea847-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea847-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea847-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea847-107">Набор определений ролей и назначений ролей, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="ea847-107">The set of Role Definitions and Role Assignments assigned to a user.</span></span>

## <a name="properties"></a><span data-ttu-id="ea847-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ea847-108">Properties</span></span>
|<span data-ttu-id="ea847-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea847-109">Property</span></span>|<span data-ttu-id="ea847-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ea847-110">Type</span></span>|<span data-ttu-id="ea847-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ea847-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea847-112">роледефинитионидс</span><span class="sxs-lookup"><span data-stu-id="ea847-112">roleDefinitionIds</span></span>|<span data-ttu-id="ea847-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ea847-113">String collection</span></span>|<span data-ttu-id="ea847-114">Идентификаторы определений ролей для определений ролей частности, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="ea847-114">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="ea847-115">ролеассигнментидс</span><span class="sxs-lookup"><span data-stu-id="ea847-115">roleAssignmentIds</span></span>|<span data-ttu-id="ea847-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ea847-116">String collection</span></span>|<span data-ttu-id="ea847-117">Идентификаторы назначения ролей для назначений ролей частности, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="ea847-117">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea847-118">Связи</span><span class="sxs-lookup"><span data-stu-id="ea847-118">Relationships</span></span>
<span data-ttu-id="ea847-119">Нет</span><span class="sxs-lookup"><span data-stu-id="ea847-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea847-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ea847-120">JSON Representation</span></span>
<span data-ttu-id="ea847-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea847-121">Here is a JSON representation of the resource.</span></span>
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




