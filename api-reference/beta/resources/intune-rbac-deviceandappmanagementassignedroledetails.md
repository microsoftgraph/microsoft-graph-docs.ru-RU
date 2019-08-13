---
title: Тип ресурса Девицеандаппманажементассигнедроледетаилс
description: Набор определений ролей и назначений ролей, назначенных пользователю.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 89f864da336045622af0e59a94fb14d0132872db
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308192"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="1ce85-103">Тип ресурса Девицеандаппманажементассигнедроледетаилс</span><span class="sxs-lookup"><span data-stu-id="1ce85-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

> <span data-ttu-id="1ce85-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ce85-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ce85-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1ce85-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ce85-106">Набор определений ролей и назначений ролей, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="1ce85-106">The set of Role Definitions and Role Assignments assigned to a user.</span></span>

## <a name="properties"></a><span data-ttu-id="1ce85-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1ce85-107">Properties</span></span>
|<span data-ttu-id="1ce85-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ce85-108">Property</span></span>|<span data-ttu-id="1ce85-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1ce85-109">Type</span></span>|<span data-ttu-id="1ce85-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1ce85-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ce85-111">роледефинитионидс</span><span class="sxs-lookup"><span data-stu-id="1ce85-111">roleDefinitionIds</span></span>|<span data-ttu-id="1ce85-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1ce85-112">String collection</span></span>|<span data-ttu-id="1ce85-113">Идентификаторы определений ролей для определений ролей частности, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="1ce85-113">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="1ce85-114">ролеассигнментидс</span><span class="sxs-lookup"><span data-stu-id="1ce85-114">roleAssignmentIds</span></span>|<span data-ttu-id="1ce85-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1ce85-115">String collection</span></span>|<span data-ttu-id="1ce85-116">Идентификаторы назначения ролей для назначений ролей частности, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="1ce85-116">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ce85-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="1ce85-117">Relationships</span></span>
<span data-ttu-id="1ce85-118">Нет</span><span class="sxs-lookup"><span data-stu-id="1ce85-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ce85-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1ce85-119">JSON Representation</span></span>
<span data-ttu-id="1ce85-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ce85-120">Here is a JSON representation of the resource.</span></span>
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



