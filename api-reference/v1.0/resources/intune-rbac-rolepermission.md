---
title: Тип ресурса rolePermission
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2573b2319d06d6d10d952d94c8fc0a17ab8a36dd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037102"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="e09e5-103">Тип ресурса rolePermission</span><span class="sxs-lookup"><span data-stu-id="e09e5-103">rolePermission resource type</span></span>

> <span data-ttu-id="e09e5-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e09e5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e09e5-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e09e5-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e09e5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e09e5-106">Properties</span></span>
|<span data-ttu-id="e09e5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e09e5-107">Property</span></span>|<span data-ttu-id="e09e5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e09e5-108">Type</span></span>|<span data-ttu-id="e09e5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e09e5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e09e5-110">resourceActions</span><span class="sxs-lookup"><span data-stu-id="e09e5-110">resourceActions</span></span>|<span data-ttu-id="e09e5-111">Коллекция объектов [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="e09e5-111">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="e09e5-112">Действия</span><span class="sxs-lookup"><span data-stu-id="e09e5-112">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="e09e5-113">Отношения</span><span class="sxs-lookup"><span data-stu-id="e09e5-113">Relationships</span></span>
<span data-ttu-id="e09e5-114">Нет</span><span class="sxs-lookup"><span data-stu-id="e09e5-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e09e5-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e09e5-115">JSON Representation</span></span>
<span data-ttu-id="e09e5-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e09e5-116">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rolePermission"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rolePermission",
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



