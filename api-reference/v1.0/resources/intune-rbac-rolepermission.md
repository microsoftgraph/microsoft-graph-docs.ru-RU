---
title: Тип ресурса rolePermission
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b8b9ba237052fef2b4caa8123d147ea1782fa9b9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932807"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="6cf7e-103">Тип ресурса rolePermission</span><span class="sxs-lookup"><span data-stu-id="6cf7e-103">rolePermission resource type</span></span>

> <span data-ttu-id="6cf7e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6cf7e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6cf7e-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6cf7e-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="6cf7e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6cf7e-106">Properties</span></span>
|<span data-ttu-id="6cf7e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6cf7e-107">Property</span></span>|<span data-ttu-id="6cf7e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6cf7e-108">Type</span></span>|<span data-ttu-id="6cf7e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6cf7e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cf7e-110">resourceActions</span><span class="sxs-lookup"><span data-stu-id="6cf7e-110">resourceActions</span></span>|<span data-ttu-id="6cf7e-111">Коллекция объектов [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="6cf7e-111">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="6cf7e-112">Действия</span><span class="sxs-lookup"><span data-stu-id="6cf7e-112">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="6cf7e-113">Связи</span><span class="sxs-lookup"><span data-stu-id="6cf7e-113">Relationships</span></span>
<span data-ttu-id="6cf7e-114">Нет</span><span class="sxs-lookup"><span data-stu-id="6cf7e-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6cf7e-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6cf7e-115">JSON Representation</span></span>
<span data-ttu-id="6cf7e-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6cf7e-116">Here is a JSON representation of the resource.</span></span>
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



