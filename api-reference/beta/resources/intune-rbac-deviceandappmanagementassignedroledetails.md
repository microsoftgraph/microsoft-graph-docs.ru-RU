---
title: Тип ресурса Девицеандаппманажементассигнедроледетаилс
description: Набор определений ролей и наЗначений ролей, назначенных пользователю.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 93f99cdc91d046b9ebf292bbd34f1bba39b494ac
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771406"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="e4a9f-103">Тип ресурса Девицеандаппманажементассигнедроледетаилс</span><span class="sxs-lookup"><span data-stu-id="e4a9f-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

> <span data-ttu-id="e4a9f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4a9f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4a9f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e4a9f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4a9f-106">Набор определений ролей и наЗначений ролей, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="e4a9f-106">The set of Role Definitions and Role Assignments assigned to a user.</span></span>

## <a name="properties"></a><span data-ttu-id="e4a9f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4a9f-107">Properties</span></span>
|<span data-ttu-id="e4a9f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4a9f-108">Property</span></span>|<span data-ttu-id="e4a9f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e4a9f-109">Type</span></span>|<span data-ttu-id="e4a9f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e4a9f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4a9f-111">Роледефинитионидс</span><span class="sxs-lookup"><span data-stu-id="e4a9f-111">roleDefinitionIds</span></span>|<span data-ttu-id="e4a9f-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e4a9f-112">String collection</span></span>|<span data-ttu-id="e4a9f-113">Идентификаторы определений ролей для определений ролей частности, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="e4a9f-113">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="e4a9f-114">Ролеассигнментидс</span><span class="sxs-lookup"><span data-stu-id="e4a9f-114">roleAssignmentIds</span></span>|<span data-ttu-id="e4a9f-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e4a9f-115">String collection</span></span>|<span data-ttu-id="e4a9f-116">Идентификаторы назначения ролей для наЗначений ролей частности, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="e4a9f-116">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4a9f-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="e4a9f-117">Relationships</span></span>
<span data-ttu-id="e4a9f-118">Нет</span><span class="sxs-lookup"><span data-stu-id="e4a9f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4a9f-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e4a9f-119">JSON Representation</span></span>
<span data-ttu-id="e4a9f-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4a9f-120">Here is a JSON representation of the resource.</span></span>
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





