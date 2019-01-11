---
title: Тип ресурса rolePermission
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3e284198b7b2e6ad3fe120bd1c17c96a1872b793
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816606"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="2421f-103">Тип ресурса rolePermission</span><span class="sxs-lookup"><span data-stu-id="2421f-103">rolePermission resource type</span></span>

> <span data-ttu-id="2421f-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2421f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2421f-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2421f-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="2421f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2421f-106">Properties</span></span>
|<span data-ttu-id="2421f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2421f-107">Property</span></span>|<span data-ttu-id="2421f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2421f-108">Type</span></span>|<span data-ttu-id="2421f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2421f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2421f-110">resourceActions</span><span class="sxs-lookup"><span data-stu-id="2421f-110">resourceActions</span></span>|<span data-ttu-id="2421f-111">Коллекция объектов [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="2421f-111">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="2421f-112">Действия</span><span class="sxs-lookup"><span data-stu-id="2421f-112">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="2421f-113">Связи</span><span class="sxs-lookup"><span data-stu-id="2421f-113">Relationships</span></span>
<span data-ttu-id="2421f-114">Нет</span><span class="sxs-lookup"><span data-stu-id="2421f-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2421f-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2421f-115">JSON Representation</span></span>
<span data-ttu-id="2421f-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2421f-116">Here is a JSON representation of the resource.</span></span>
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



