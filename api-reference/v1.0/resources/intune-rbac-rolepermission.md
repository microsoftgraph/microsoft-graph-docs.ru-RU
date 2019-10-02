---
title: Тип ресурса rolePermission
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2f53a6250500137b368f17ae71524f4e1121d1aa
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355878"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="b570c-103">Тип ресурса rolePermission</span><span class="sxs-lookup"><span data-stu-id="b570c-103">rolePermission resource type</span></span>

> <span data-ttu-id="b570c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b570c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b570c-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b570c-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b570c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b570c-106">Properties</span></span>
|<span data-ttu-id="b570c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b570c-107">Property</span></span>|<span data-ttu-id="b570c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b570c-108">Type</span></span>|<span data-ttu-id="b570c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b570c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b570c-110">resourceActions</span><span class="sxs-lookup"><span data-stu-id="b570c-110">resourceActions</span></span>|<span data-ttu-id="b570c-111">Коллекция объектов [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="b570c-111">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="b570c-112">Действия</span><span class="sxs-lookup"><span data-stu-id="b570c-112">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="b570c-113">Связи</span><span class="sxs-lookup"><span data-stu-id="b570c-113">Relationships</span></span>
<span data-ttu-id="b570c-114">Нет</span><span class="sxs-lookup"><span data-stu-id="b570c-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b570c-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b570c-115">JSON Representation</span></span>
<span data-ttu-id="b570c-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b570c-116">Here is a JSON representation of the resource.</span></span>
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




