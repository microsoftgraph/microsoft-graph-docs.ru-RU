---
title: Тип ресурса rolePermission
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a90de4e78bbc831ebb9eb7bf5ee65c26434fc06
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257787"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="6b9d2-103">Тип ресурса rolePermission</span><span class="sxs-lookup"><span data-stu-id="6b9d2-103">rolePermission resource type</span></span>

> <span data-ttu-id="6b9d2-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6b9d2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b9d2-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6b9d2-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6b9d2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b9d2-106">Properties</span></span>
|<span data-ttu-id="6b9d2-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b9d2-107">Property</span></span>|<span data-ttu-id="6b9d2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6b9d2-108">Type</span></span>|<span data-ttu-id="6b9d2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6b9d2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b9d2-110">resourceActions</span><span class="sxs-lookup"><span data-stu-id="6b9d2-110">resourceActions</span></span>|<span data-ttu-id="6b9d2-111">Коллекция объектов [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="6b9d2-111">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="6b9d2-112">Действия</span><span class="sxs-lookup"><span data-stu-id="6b9d2-112">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b9d2-113">Связи</span><span class="sxs-lookup"><span data-stu-id="6b9d2-113">Relationships</span></span>
<span data-ttu-id="6b9d2-114">Нет</span><span class="sxs-lookup"><span data-stu-id="6b9d2-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b9d2-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6b9d2-115">JSON Representation</span></span>
<span data-ttu-id="6b9d2-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b9d2-116">Here is a JSON representation of the resource.</span></span>
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



