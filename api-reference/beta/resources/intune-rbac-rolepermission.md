---
title: Тип ресурса rolePermission
description: Содержит набор Ресаурцеактионс, определяющих разрешения "разрешено" и "не разрешено" для каждой роли.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7c5ef360393e99b8c8a152596a2285cddd49d7e0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939030"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="52d49-103">Тип ресурса rolePermission</span><span class="sxs-lookup"><span data-stu-id="52d49-103">rolePermission resource type</span></span>

> <span data-ttu-id="52d49-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52d49-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52d49-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="52d49-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52d49-106">Содержит набор Ресаурцеактионс, определяющих разрешения "разрешено" и "не разрешено" для каждой роли.</span><span class="sxs-lookup"><span data-stu-id="52d49-106">Contains the set of ResourceActions determining the allowed and not allowed permissions for each role.</span></span>

## <a name="properties"></a><span data-ttu-id="52d49-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="52d49-107">Properties</span></span>
|<span data-ttu-id="52d49-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="52d49-108">Property</span></span>|<span data-ttu-id="52d49-109">Тип</span><span class="sxs-lookup"><span data-stu-id="52d49-109">Type</span></span>|<span data-ttu-id="52d49-110">Описание</span><span class="sxs-lookup"><span data-stu-id="52d49-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52d49-111">actions</span><span class="sxs-lookup"><span data-stu-id="52d49-111">actions</span></span>|<span data-ttu-id="52d49-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="52d49-112">String collection</span></span>|<span data-ttu-id="52d49-113">Разрешенные действия — устарело</span><span class="sxs-lookup"><span data-stu-id="52d49-113">Allowed Actions - Deprecated</span></span>|
|<span data-ttu-id="52d49-114">resourceActions</span><span class="sxs-lookup"><span data-stu-id="52d49-114">resourceActions</span></span>|<span data-ttu-id="52d49-115">Коллекция объектов [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="52d49-115">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="52d49-116">Действия с ресурсами, содержащие набор разрешенных и запрещенных разрешений.</span><span class="sxs-lookup"><span data-stu-id="52d49-116">Resource Actions each containing a set of allowed and not allowed permissions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52d49-117">Связи</span><span class="sxs-lookup"><span data-stu-id="52d49-117">Relationships</span></span>
<span data-ttu-id="52d49-118">Нет</span><span class="sxs-lookup"><span data-stu-id="52d49-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="52d49-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="52d49-119">JSON Representation</span></span>
<span data-ttu-id="52d49-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52d49-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rolePermission"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rolePermission",
  "actions": [
    "String"
  ],
  "resourceActions": [
    {
      "@odata.type": "microsoft.graph.resourceAction",
      "allowedResourceActions": [
        "String"
      ],
      "notAllowedResourceActions": [
        "String"
      ]
    }
  ]
}
```




