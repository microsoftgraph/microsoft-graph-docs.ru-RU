---
title: Тип ресурса Девицеандаппманажементассигнедроледетаилс
description: Набор определений ролей и назначений ролей, назначенных пользователю.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f9dff637f950d980b3fc0de89ecfde26da6b40de
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070802"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="44a6a-103">Тип ресурса Девицеандаппманажементассигнедроледетаилс</span><span class="sxs-lookup"><span data-stu-id="44a6a-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

<span data-ttu-id="44a6a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44a6a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44a6a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44a6a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44a6a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44a6a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44a6a-107">Набор определений ролей и назначений ролей, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="44a6a-107">The set of Role Definitions and Role Assignments assigned to a user.</span></span>

## <a name="properties"></a><span data-ttu-id="44a6a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="44a6a-108">Properties</span></span>
|<span data-ttu-id="44a6a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="44a6a-109">Property</span></span>|<span data-ttu-id="44a6a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="44a6a-110">Type</span></span>|<span data-ttu-id="44a6a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="44a6a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44a6a-112">роледефинитионидс</span><span class="sxs-lookup"><span data-stu-id="44a6a-112">roleDefinitionIds</span></span>|<span data-ttu-id="44a6a-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="44a6a-113">String collection</span></span>|<span data-ttu-id="44a6a-114">Идентификаторы определений ролей для определений ролей частности, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="44a6a-114">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="44a6a-115">ролеассигнментидс</span><span class="sxs-lookup"><span data-stu-id="44a6a-115">roleAssignmentIds</span></span>|<span data-ttu-id="44a6a-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="44a6a-116">String collection</span></span>|<span data-ttu-id="44a6a-117">Идентификаторы назначения ролей для назначений ролей частности, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="44a6a-117">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="44a6a-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="44a6a-118">Relationships</span></span>
<span data-ttu-id="44a6a-119">Нет</span><span class="sxs-lookup"><span data-stu-id="44a6a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="44a6a-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="44a6a-120">JSON Representation</span></span>
<span data-ttu-id="44a6a-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44a6a-121">Here is a JSON representation of the resource.</span></span>
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






