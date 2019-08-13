---
title: Тип ресурса rolePermission
description: Содержит набор Ресаурцеактионс, определяющих разрешения "разрешено" и "не разрешено" для каждой роли.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c612e4c6201a3016b866eddc7e5e52d0b3238306
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369215"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="60651-103">Тип ресурса rolePermission</span><span class="sxs-lookup"><span data-stu-id="60651-103">rolePermission resource type</span></span>

> <span data-ttu-id="60651-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60651-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60651-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="60651-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60651-106">Содержит набор Ресаурцеактионс, определяющих разрешения "разрешено" и "не разрешено" для каждой роли.</span><span class="sxs-lookup"><span data-stu-id="60651-106">Contains the set of ResourceActions determining the allowed and not allowed permissions for each role.</span></span>

## <a name="properties"></a><span data-ttu-id="60651-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="60651-107">Properties</span></span>
|<span data-ttu-id="60651-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="60651-108">Property</span></span>|<span data-ttu-id="60651-109">Тип</span><span class="sxs-lookup"><span data-stu-id="60651-109">Type</span></span>|<span data-ttu-id="60651-110">Описание</span><span class="sxs-lookup"><span data-stu-id="60651-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60651-111">actions</span><span class="sxs-lookup"><span data-stu-id="60651-111">actions</span></span>|<span data-ttu-id="60651-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="60651-112">String collection</span></span>|<span data-ttu-id="60651-113">Разрешенные действия — устарело</span><span class="sxs-lookup"><span data-stu-id="60651-113">Allowed Actions - Deprecated</span></span>|
|<span data-ttu-id="60651-114">resourceActions</span><span class="sxs-lookup"><span data-stu-id="60651-114">resourceActions</span></span>|<span data-ttu-id="60651-115">Коллекция объектов [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="60651-115">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="60651-116">Действия с ресурсами, содержащие набор разрешенных и запрещенных разрешений.</span><span class="sxs-lookup"><span data-stu-id="60651-116">Resource Actions each containing a set of allowed and not allowed permissions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60651-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="60651-117">Relationships</span></span>
<span data-ttu-id="60651-118">Нет</span><span class="sxs-lookup"><span data-stu-id="60651-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="60651-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="60651-119">JSON Representation</span></span>
<span data-ttu-id="60651-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60651-120">Here is a JSON representation of the resource.</span></span>
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



