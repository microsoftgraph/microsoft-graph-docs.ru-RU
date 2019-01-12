---
title: Тип ресурса rolePermission
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c9a1ccacc4de13574ea984977dbfb05c09a2cea5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912332"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="b597a-103">Тип ресурса rolePermission</span><span class="sxs-lookup"><span data-stu-id="b597a-103">rolePermission resource type</span></span>

> <span data-ttu-id="b597a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b597a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b597a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b597a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b597a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b597a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b597a-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b597a-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="b597a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b597a-108">Properties</span></span>
|<span data-ttu-id="b597a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b597a-109">Property</span></span>|<span data-ttu-id="b597a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b597a-110">Type</span></span>|<span data-ttu-id="b597a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b597a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b597a-112">actions</span><span class="sxs-lookup"><span data-stu-id="b597a-112">actions</span></span>|<span data-ttu-id="b597a-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b597a-113">String collection</span></span>|<span data-ttu-id="b597a-114">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="b597a-114">Allowed Actions</span></span>|
|<span data-ttu-id="b597a-115">resourceActions</span><span class="sxs-lookup"><span data-stu-id="b597a-115">resourceActions</span></span>|<span data-ttu-id="b597a-116">Коллекция объектов [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="b597a-116">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="b597a-117">Действия</span><span class="sxs-lookup"><span data-stu-id="b597a-117">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="b597a-118">Связи</span><span class="sxs-lookup"><span data-stu-id="b597a-118">Relationships</span></span>
<span data-ttu-id="b597a-119">Нет</span><span class="sxs-lookup"><span data-stu-id="b597a-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b597a-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b597a-120">JSON Representation</span></span>
<span data-ttu-id="b597a-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b597a-121">Here is a JSON representation of the resource.</span></span>
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





