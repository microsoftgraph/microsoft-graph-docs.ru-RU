---
title: Тип ресурса Девицеандаппманажементассигнедроледетаилс
description: Набор определений ролей и наЗначений ролей, назначенных пользователю.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 93f99cdc91d046b9ebf292bbd34f1bba39b494ac
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573076"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="d2df0-103">Тип ресурса Девицеандаппманажементассигнедроледетаилс</span><span class="sxs-lookup"><span data-stu-id="d2df0-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

> <span data-ttu-id="d2df0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2df0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2df0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d2df0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2df0-106">Набор определений ролей и наЗначений ролей, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="d2df0-106">The set of Role Definitions and Role Assignments assigned to a user.</span></span>

## <a name="properties"></a><span data-ttu-id="d2df0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2df0-107">Properties</span></span>
|<span data-ttu-id="d2df0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2df0-108">Property</span></span>|<span data-ttu-id="d2df0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d2df0-109">Type</span></span>|<span data-ttu-id="d2df0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d2df0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2df0-111">Роледефинитионидс</span><span class="sxs-lookup"><span data-stu-id="d2df0-111">roleDefinitionIds</span></span>|<span data-ttu-id="d2df0-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d2df0-112">String collection</span></span>|<span data-ttu-id="d2df0-113">Идентификаторы определений ролей для определений ролей частности, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="d2df0-113">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="d2df0-114">Ролеассигнментидс</span><span class="sxs-lookup"><span data-stu-id="d2df0-114">roleAssignmentIds</span></span>|<span data-ttu-id="d2df0-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d2df0-115">String collection</span></span>|<span data-ttu-id="d2df0-116">Идентификаторы назначения ролей для наЗначений ролей частности, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="d2df0-116">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2df0-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="d2df0-117">Relationships</span></span>
<span data-ttu-id="d2df0-118">Нет</span><span class="sxs-lookup"><span data-stu-id="d2df0-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2df0-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d2df0-119">JSON Representation</span></span>
<span data-ttu-id="d2df0-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2df0-120">Here is a JSON representation of the resource.</span></span>
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





