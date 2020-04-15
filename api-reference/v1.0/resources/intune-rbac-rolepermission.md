---
title: Тип ресурса rolePermission
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7a8e607e01ab0b2955e8a016c0b9d73ee4748cbf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441589"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="8a6d5-103">Тип ресурса rolePermission</span><span class="sxs-lookup"><span data-stu-id="8a6d5-103">rolePermission resource type</span></span>

<span data-ttu-id="8a6d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a6d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8a6d5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8a6d5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a6d5-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8a6d5-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8a6d5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a6d5-107">Properties</span></span>
|<span data-ttu-id="8a6d5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a6d5-108">Property</span></span>|<span data-ttu-id="8a6d5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8a6d5-109">Type</span></span>|<span data-ttu-id="8a6d5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8a6d5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a6d5-111">resourceActions</span><span class="sxs-lookup"><span data-stu-id="8a6d5-111">resourceActions</span></span>|<span data-ttu-id="8a6d5-112">Коллекция объектов [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="8a6d5-112">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="8a6d5-113">Действия</span><span class="sxs-lookup"><span data-stu-id="8a6d5-113">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a6d5-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="8a6d5-114">Relationships</span></span>
<span data-ttu-id="8a6d5-115">Нет</span><span class="sxs-lookup"><span data-stu-id="8a6d5-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a6d5-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8a6d5-116">JSON Representation</span></span>
<span data-ttu-id="8a6d5-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a6d5-117">Here is a JSON representation of the resource.</span></span>
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







