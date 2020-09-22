---
title: Тип ресурса rolePermission
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1def1929449f5c737bc37b30aa41a1131e1b2944
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037782"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="8d6c0-103">Тип ресурса rolePermission</span><span class="sxs-lookup"><span data-stu-id="8d6c0-103">rolePermission resource type</span></span>

<span data-ttu-id="8d6c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d6c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d6c0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d6c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d6c0-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8d6c0-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8d6c0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d6c0-107">Properties</span></span>
|<span data-ttu-id="8d6c0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d6c0-108">Property</span></span>|<span data-ttu-id="8d6c0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8d6c0-109">Type</span></span>|<span data-ttu-id="8d6c0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8d6c0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d6c0-111">resourceActions</span><span class="sxs-lookup"><span data-stu-id="8d6c0-111">resourceActions</span></span>|<span data-ttu-id="8d6c0-112">Коллекция объектов [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="8d6c0-112">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="8d6c0-113">Действия</span><span class="sxs-lookup"><span data-stu-id="8d6c0-113">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d6c0-114">Связи</span><span class="sxs-lookup"><span data-stu-id="8d6c0-114">Relationships</span></span>
<span data-ttu-id="8d6c0-115">Нет</span><span class="sxs-lookup"><span data-stu-id="8d6c0-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d6c0-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8d6c0-116">JSON Representation</span></span>
<span data-ttu-id="8d6c0-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d6c0-117">Here is a JSON representation of the resource.</span></span>
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









