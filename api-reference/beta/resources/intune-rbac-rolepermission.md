---
title: Тип ресурса rolePermission
description: Н/Д
ms.openlocfilehash: 350cfe6c220d73b14464a761c3b8a469f57ab352
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080033"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="0c239-103">Тип ресурса rolePermission</span><span class="sxs-lookup"><span data-stu-id="0c239-103">rolePermission resource type</span></span>

> <span data-ttu-id="0c239-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0c239-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c239-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c239-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c239-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0c239-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c239-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0c239-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="0c239-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c239-108">Properties</span></span>
|<span data-ttu-id="0c239-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c239-109">Property</span></span>|<span data-ttu-id="0c239-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0c239-110">Type</span></span>|<span data-ttu-id="0c239-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0c239-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c239-112">actions</span><span class="sxs-lookup"><span data-stu-id="0c239-112">actions</span></span>|<span data-ttu-id="0c239-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0c239-113">String collection</span></span>|<span data-ttu-id="0c239-114">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="0c239-114">Allowed Actions</span></span>|
|<span data-ttu-id="0c239-115">resourceActions</span><span class="sxs-lookup"><span data-stu-id="0c239-115">resourceActions</span></span>|<span data-ttu-id="0c239-116">Коллекция объектов [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="0c239-116">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="0c239-117">Действия</span><span class="sxs-lookup"><span data-stu-id="0c239-117">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c239-118">Связи</span><span class="sxs-lookup"><span data-stu-id="0c239-118">Relationships</span></span>
<span data-ttu-id="0c239-119">Нет</span><span class="sxs-lookup"><span data-stu-id="0c239-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0c239-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0c239-120">JSON Representation</span></span>
<span data-ttu-id="0c239-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c239-121">Here is a JSON representation of the resource.</span></span>
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





