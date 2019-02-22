---
title: Тип ресурса Девицеандаппманажементассигнедроледетаилс
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eafacd349b5d315cb7a1149d7bcc7070700b7130
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160076"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="52b1d-103">Тип ресурса Девицеандаппманажементассигнедроледетаилс</span><span class="sxs-lookup"><span data-stu-id="52b1d-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

> <span data-ttu-id="52b1d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52b1d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52b1d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="52b1d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52b1d-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="52b1d-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="52b1d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="52b1d-107">Properties</span></span>
|<span data-ttu-id="52b1d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="52b1d-108">Property</span></span>|<span data-ttu-id="52b1d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="52b1d-109">Type</span></span>|<span data-ttu-id="52b1d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="52b1d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52b1d-111">Роледефинитионидс</span><span class="sxs-lookup"><span data-stu-id="52b1d-111">roleDefinitionIds</span></span>|<span data-ttu-id="52b1d-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="52b1d-112">String collection</span></span>|<span data-ttu-id="52b1d-113">Идентификаторы определений ролей для определений ролей частности, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="52b1d-113">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="52b1d-114">Ролеассигнментидс</span><span class="sxs-lookup"><span data-stu-id="52b1d-114">roleAssignmentIds</span></span>|<span data-ttu-id="52b1d-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="52b1d-115">String collection</span></span>|<span data-ttu-id="52b1d-116">Идентификаторы назначения ролей для наЗначений ролей частности, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="52b1d-116">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52b1d-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="52b1d-117">Relationships</span></span>
<span data-ttu-id="52b1d-118">Нет</span><span class="sxs-lookup"><span data-stu-id="52b1d-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="52b1d-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="52b1d-119">JSON Representation</span></span>
<span data-ttu-id="52b1d-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52b1d-120">Here is a JSON representation of the resource.</span></span>
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




