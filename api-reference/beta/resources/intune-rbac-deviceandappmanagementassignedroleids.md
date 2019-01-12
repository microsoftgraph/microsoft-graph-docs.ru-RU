---
title: Тип ресурса deviceAndAppManagementAssignedRoleIds
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2dbabca28f9ed8aa491d01f6eada5dc11b76867b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923378"
---
# <a name="deviceandappmanagementassignedroleids-resource-type"></a><span data-ttu-id="ed067-103">Тип ресурса deviceAndAppManagementAssignedRoleIds</span><span class="sxs-lookup"><span data-stu-id="ed067-103">deviceAndAppManagementAssignedRoleIds resource type</span></span>

> <span data-ttu-id="ed067-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ed067-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed067-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed067-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed067-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ed067-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed067-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ed067-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="ed067-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ed067-108">Properties</span></span>
|<span data-ttu-id="ed067-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed067-109">Property</span></span>|<span data-ttu-id="ed067-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ed067-110">Type</span></span>|<span data-ttu-id="ed067-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ed067-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed067-112">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="ed067-112">roleDefinitionIds</span></span>|<span data-ttu-id="ed067-113">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="ed067-113">Guid collection</span></span>|<span data-ttu-id="ed067-114">Идентификаторы определения ролей особую определения ролей, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="ed067-114">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="ed067-115">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="ed067-115">roleAssignmentIds</span></span>|<span data-ttu-id="ed067-116">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="ed067-116">Guid collection</span></span>|<span data-ttu-id="ed067-117">Идентификаторы назначения ролей для назначения ролей, назначенных пользователю особую.</span><span class="sxs-lookup"><span data-stu-id="ed067-117">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed067-118">Связи</span><span class="sxs-lookup"><span data-stu-id="ed067-118">Relationships</span></span>
<span data-ttu-id="ed067-119">Нет</span><span class="sxs-lookup"><span data-stu-id="ed067-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ed067-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ed067-120">JSON Representation</span></span>
<span data-ttu-id="ed067-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed067-121">Here is a JSON representation of the resource.</span></span>
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





