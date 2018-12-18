---
title: Тип ресурса deviceAndAppManagementAssignedRoleIds
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 034120b891812a43c6c1683f61e52f071dc89816
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353384"
---
# <a name="deviceandappmanagementassignedroleids-resource-type"></a><span data-ttu-id="58421-103">Тип ресурса deviceAndAppManagementAssignedRoleIds</span><span class="sxs-lookup"><span data-stu-id="58421-103">deviceAndAppManagementAssignedRoleIds resource type</span></span>

> <span data-ttu-id="58421-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="58421-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58421-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58421-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="58421-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="58421-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58421-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="58421-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="58421-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="58421-108">Properties</span></span>
|<span data-ttu-id="58421-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="58421-109">Property</span></span>|<span data-ttu-id="58421-110">Тип</span><span class="sxs-lookup"><span data-stu-id="58421-110">Type</span></span>|<span data-ttu-id="58421-111">Описание</span><span class="sxs-lookup"><span data-stu-id="58421-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58421-112">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="58421-112">roleDefinitionIds</span></span>|<span data-ttu-id="58421-113">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="58421-113">Guid collection</span></span>|<span data-ttu-id="58421-114">Идентификаторы определения ролей особую определения ролей, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="58421-114">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="58421-115">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="58421-115">roleAssignmentIds</span></span>|<span data-ttu-id="58421-116">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="58421-116">Guid collection</span></span>|<span data-ttu-id="58421-117">Идентификаторы назначения ролей для назначения ролей, назначенных пользователю особую.</span><span class="sxs-lookup"><span data-stu-id="58421-117">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="58421-118">Связи</span><span class="sxs-lookup"><span data-stu-id="58421-118">Relationships</span></span>
<span data-ttu-id="58421-119">Нет</span><span class="sxs-lookup"><span data-stu-id="58421-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="58421-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="58421-120">JSON Representation</span></span>
<span data-ttu-id="58421-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58421-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleIds"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignedRoleIds",
  "roleDefinitionIds": [
    "Guid"
  ],
  "roleAssignmentIds": [
    "Guid"
  ]
}
```





