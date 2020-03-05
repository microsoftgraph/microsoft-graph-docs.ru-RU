---
title: Тип ресурса rolePermission
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f3a01bf7c6f607c7340cff8ea5075a24fb879ddb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447929"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="2371f-103">Тип ресурса rolePermission</span><span class="sxs-lookup"><span data-stu-id="2371f-103">rolePermission resource type</span></span>

<span data-ttu-id="2371f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2371f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2371f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2371f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2371f-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2371f-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="2371f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2371f-107">Properties</span></span>
|<span data-ttu-id="2371f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2371f-108">Property</span></span>|<span data-ttu-id="2371f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2371f-109">Type</span></span>|<span data-ttu-id="2371f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2371f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2371f-111">resourceActions</span><span class="sxs-lookup"><span data-stu-id="2371f-111">resourceActions</span></span>|<span data-ttu-id="2371f-112">Коллекция объектов [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="2371f-112">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="2371f-113">Действия</span><span class="sxs-lookup"><span data-stu-id="2371f-113">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="2371f-114">Связи</span><span class="sxs-lookup"><span data-stu-id="2371f-114">Relationships</span></span>
<span data-ttu-id="2371f-115">Нет</span><span class="sxs-lookup"><span data-stu-id="2371f-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2371f-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2371f-116">JSON Representation</span></span>
<span data-ttu-id="2371f-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2371f-117">Here is a JSON representation of the resource.</span></span>
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




