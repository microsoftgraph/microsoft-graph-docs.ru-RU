---
title: Тип ресурса rolePermission
description: Содержит набор Ресаурцеактионс, определяющих разрешения "разрешено" и "не разрешено" для каждой роли.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e9bbd4782022faebcf56b8bf582e233fd5ba54f6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771266"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="6e7b5-103">Тип ресурса rolePermission</span><span class="sxs-lookup"><span data-stu-id="6e7b5-103">rolePermission resource type</span></span>

> <span data-ttu-id="6e7b5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e7b5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e7b5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6e7b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e7b5-106">Содержит набор Ресаурцеактионс, определяющих разрешения "разрешено" и "не разрешено" для каждой роли.</span><span class="sxs-lookup"><span data-stu-id="6e7b5-106">Contains the set of ResourceActions determining the allowed and not allowed permissions for each role.</span></span>

## <a name="properties"></a><span data-ttu-id="6e7b5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e7b5-107">Properties</span></span>
|<span data-ttu-id="6e7b5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e7b5-108">Property</span></span>|<span data-ttu-id="6e7b5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6e7b5-109">Type</span></span>|<span data-ttu-id="6e7b5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6e7b5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e7b5-111">actions</span><span class="sxs-lookup"><span data-stu-id="6e7b5-111">actions</span></span>|<span data-ttu-id="6e7b5-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6e7b5-112">String collection</span></span>|<span data-ttu-id="6e7b5-113">Разрешенные действия — устарело</span><span class="sxs-lookup"><span data-stu-id="6e7b5-113">Allowed Actions - Deprecated</span></span>|
|<span data-ttu-id="6e7b5-114">resourceActions</span><span class="sxs-lookup"><span data-stu-id="6e7b5-114">resourceActions</span></span>|<span data-ttu-id="6e7b5-115">Коллекция объектов [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="6e7b5-115">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="6e7b5-116">Действия с ресурсами, содержащие набор разрешенных и запрещенных разрешений.</span><span class="sxs-lookup"><span data-stu-id="6e7b5-116">Resource Actions each containing a set of allowed and not allowed permissions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e7b5-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="6e7b5-117">Relationships</span></span>
<span data-ttu-id="6e7b5-118">Нет</span><span class="sxs-lookup"><span data-stu-id="6e7b5-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e7b5-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e7b5-119">JSON Representation</span></span>
<span data-ttu-id="6e7b5-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e7b5-120">Here is a JSON representation of the resource.</span></span>
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





