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
# <a name="rolepermission-resource-type"></a><span data-ttu-id="bf997-103">Тип ресурса rolePermission</span><span class="sxs-lookup"><span data-stu-id="bf997-103">rolePermission resource type</span></span>

<span data-ttu-id="bf997-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf997-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bf997-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bf997-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf997-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="bf997-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="bf997-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf997-107">Properties</span></span>
|<span data-ttu-id="bf997-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf997-108">Property</span></span>|<span data-ttu-id="bf997-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bf997-109">Type</span></span>|<span data-ttu-id="bf997-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bf997-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf997-111">resourceActions</span><span class="sxs-lookup"><span data-stu-id="bf997-111">resourceActions</span></span>|<span data-ttu-id="bf997-112">Коллекция объектов [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="bf997-112">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="bf997-113">Действия</span><span class="sxs-lookup"><span data-stu-id="bf997-113">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf997-114">Связи</span><span class="sxs-lookup"><span data-stu-id="bf997-114">Relationships</span></span>
<span data-ttu-id="bf997-115">Нет</span><span class="sxs-lookup"><span data-stu-id="bf997-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf997-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bf997-116">JSON Representation</span></span>
<span data-ttu-id="bf997-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf997-117">Here is a JSON representation of the resource.</span></span>
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







