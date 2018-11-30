---
title: Тип ресурса rolePermission
description: Н/Д
ms.openlocfilehash: 16c78e2ee4475a717879d501aabeb5fe2ae0d481
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026007"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="0305d-103">Тип ресурса rolePermission</span><span class="sxs-lookup"><span data-stu-id="0305d-103">rolePermission resource type</span></span>

> <span data-ttu-id="0305d-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0305d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0305d-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0305d-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="0305d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0305d-106">Properties</span></span>
|<span data-ttu-id="0305d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0305d-107">Property</span></span>|<span data-ttu-id="0305d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0305d-108">Type</span></span>|<span data-ttu-id="0305d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0305d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0305d-110">resourceActions</span><span class="sxs-lookup"><span data-stu-id="0305d-110">resourceActions</span></span>|<span data-ttu-id="0305d-111">Коллекция объектов [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="0305d-111">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="0305d-112">Действия</span><span class="sxs-lookup"><span data-stu-id="0305d-112">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="0305d-113">Связи</span><span class="sxs-lookup"><span data-stu-id="0305d-113">Relationships</span></span>
<span data-ttu-id="0305d-114">Нет</span><span class="sxs-lookup"><span data-stu-id="0305d-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0305d-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0305d-115">JSON Representation</span></span>
<span data-ttu-id="0305d-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0305d-116">Here is a JSON representation of the resource.</span></span>
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



