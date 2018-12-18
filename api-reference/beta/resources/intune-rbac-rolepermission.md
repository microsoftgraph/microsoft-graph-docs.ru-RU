---
title: Тип ресурса rolePermission
description: Н/Д
author: tfitzmac
ms.openlocfilehash: c33af6af3bc06a53bd24ddf97576551a5eea6e9c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349107"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="9aa02-103">Тип ресурса rolePermission</span><span class="sxs-lookup"><span data-stu-id="9aa02-103">rolePermission resource type</span></span>

> <span data-ttu-id="9aa02-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9aa02-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9aa02-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9aa02-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9aa02-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9aa02-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9aa02-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9aa02-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="9aa02-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9aa02-108">Properties</span></span>
|<span data-ttu-id="9aa02-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9aa02-109">Property</span></span>|<span data-ttu-id="9aa02-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9aa02-110">Type</span></span>|<span data-ttu-id="9aa02-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9aa02-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9aa02-112">actions</span><span class="sxs-lookup"><span data-stu-id="9aa02-112">actions</span></span>|<span data-ttu-id="9aa02-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9aa02-113">String collection</span></span>|<span data-ttu-id="9aa02-114">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="9aa02-114">Allowed Actions</span></span>|
|<span data-ttu-id="9aa02-115">resourceActions</span><span class="sxs-lookup"><span data-stu-id="9aa02-115">resourceActions</span></span>|<span data-ttu-id="9aa02-116">Коллекция объектов [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="9aa02-116">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="9aa02-117">Действия</span><span class="sxs-lookup"><span data-stu-id="9aa02-117">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="9aa02-118">Связи</span><span class="sxs-lookup"><span data-stu-id="9aa02-118">Relationships</span></span>
<span data-ttu-id="9aa02-119">Нет</span><span class="sxs-lookup"><span data-stu-id="9aa02-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9aa02-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9aa02-120">JSON Representation</span></span>
<span data-ttu-id="9aa02-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9aa02-121">Here is a JSON representation of the resource.</span></span>
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





