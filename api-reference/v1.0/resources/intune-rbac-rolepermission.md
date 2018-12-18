---
title: Тип ресурса rolePermission
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 0433c3f3a0ab3ef63fcd2a44776c083ddb5b91a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325678"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="8d577-103">Тип ресурса rolePermission</span><span class="sxs-lookup"><span data-stu-id="8d577-103">rolePermission resource type</span></span>

> <span data-ttu-id="8d577-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8d577-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8d577-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8d577-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="8d577-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d577-106">Properties</span></span>
|<span data-ttu-id="8d577-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d577-107">Property</span></span>|<span data-ttu-id="8d577-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8d577-108">Type</span></span>|<span data-ttu-id="8d577-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8d577-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d577-110">resourceActions</span><span class="sxs-lookup"><span data-stu-id="8d577-110">resourceActions</span></span>|<span data-ttu-id="8d577-111">Коллекция объектов [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="8d577-111">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="8d577-112">Действия</span><span class="sxs-lookup"><span data-stu-id="8d577-112">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d577-113">Связи</span><span class="sxs-lookup"><span data-stu-id="8d577-113">Relationships</span></span>
<span data-ttu-id="8d577-114">Нет</span><span class="sxs-lookup"><span data-stu-id="8d577-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8d577-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8d577-115">JSON Representation</span></span>
<span data-ttu-id="8d577-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d577-116">Here is a JSON representation of the resource.</span></span>
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



