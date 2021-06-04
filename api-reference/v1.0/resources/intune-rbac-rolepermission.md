---
title: Тип ресурса rolePermission
description: Содержит набор ResourceActions, определяющий разрешенные и не разрешенные разрешения для каждой роли.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7598e7f7a54910d706ec95741234a38a9a9ba422
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752751"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="07c7e-103">Тип ресурса rolePermission</span><span class="sxs-lookup"><span data-stu-id="07c7e-103">rolePermission resource type</span></span>

<span data-ttu-id="07c7e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07c7e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07c7e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="07c7e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07c7e-106">Содержит набор ResourceActions, определяющий разрешенные и не разрешенные разрешения для каждой роли.</span><span class="sxs-lookup"><span data-stu-id="07c7e-106">Contains the set of ResourceActions determining the allowed and not allowed permissions for each role.</span></span>

## <a name="properties"></a><span data-ttu-id="07c7e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="07c7e-107">Properties</span></span>
|<span data-ttu-id="07c7e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="07c7e-108">Property</span></span>|<span data-ttu-id="07c7e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="07c7e-109">Type</span></span>|<span data-ttu-id="07c7e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="07c7e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07c7e-111">resourceActions</span><span class="sxs-lookup"><span data-stu-id="07c7e-111">resourceActions</span></span>|<span data-ttu-id="07c7e-112">Коллекция объектов [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="07c7e-112">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="07c7e-113">Действия ресурса, каждый из которых содержит набор разрешенных и не разрешенных разрешений.</span><span class="sxs-lookup"><span data-stu-id="07c7e-113">Resource Actions each containing a set of allowed and not allowed permissions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07c7e-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="07c7e-114">Relationships</span></span>
<span data-ttu-id="07c7e-115">Нет</span><span class="sxs-lookup"><span data-stu-id="07c7e-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07c7e-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="07c7e-116">JSON Representation</span></span>
<span data-ttu-id="07c7e-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07c7e-117">Here is a JSON representation of the resource.</span></span>
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




