---
title: Тип ресурса rolePermission
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0669a0e169a71ea3806b21a125a4921b5161d516
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855575"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="822e5-103">Тип ресурса rolePermission</span><span class="sxs-lookup"><span data-stu-id="822e5-103">rolePermission resource type</span></span>

> <span data-ttu-id="822e5-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="822e5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="822e5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="822e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="822e5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="822e5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="822e5-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="822e5-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="822e5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="822e5-108">Properties</span></span>
|<span data-ttu-id="822e5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="822e5-109">Property</span></span>|<span data-ttu-id="822e5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="822e5-110">Type</span></span>|<span data-ttu-id="822e5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="822e5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="822e5-112">actions</span><span class="sxs-lookup"><span data-stu-id="822e5-112">actions</span></span>|<span data-ttu-id="822e5-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="822e5-113">String collection</span></span>|<span data-ttu-id="822e5-114">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="822e5-114">Allowed Actions</span></span>|
|<span data-ttu-id="822e5-115">resourceActions</span><span class="sxs-lookup"><span data-stu-id="822e5-115">resourceActions</span></span>|<span data-ttu-id="822e5-116">Коллекция объектов [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="822e5-116">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="822e5-117">Действия</span><span class="sxs-lookup"><span data-stu-id="822e5-117">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="822e5-118">Связи</span><span class="sxs-lookup"><span data-stu-id="822e5-118">Relationships</span></span>
<span data-ttu-id="822e5-119">Нет</span><span class="sxs-lookup"><span data-stu-id="822e5-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="822e5-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="822e5-120">JSON Representation</span></span>
<span data-ttu-id="822e5-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="822e5-121">Here is a JSON representation of the resource.</span></span>
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





