---
title: Тип ресурса rolePermission
description: Содержит набор Ресаурцеактионс, определяющих разрешения "разрешено" и "не разрешено" для каждой роли.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 06790fb7fae9fd072280fd2bfe752285b290918e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523888"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="116e8-103">Тип ресурса rolePermission</span><span class="sxs-lookup"><span data-stu-id="116e8-103">rolePermission resource type</span></span>

<span data-ttu-id="116e8-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="116e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="116e8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="116e8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="116e8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="116e8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="116e8-107">Содержит набор Ресаурцеактионс, определяющих разрешения "разрешено" и "не разрешено" для каждой роли.</span><span class="sxs-lookup"><span data-stu-id="116e8-107">Contains the set of ResourceActions determining the allowed and not allowed permissions for each role.</span></span>

## <a name="properties"></a><span data-ttu-id="116e8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="116e8-108">Properties</span></span>
|<span data-ttu-id="116e8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="116e8-109">Property</span></span>|<span data-ttu-id="116e8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="116e8-110">Type</span></span>|<span data-ttu-id="116e8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="116e8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="116e8-112">actions</span><span class="sxs-lookup"><span data-stu-id="116e8-112">actions</span></span>|<span data-ttu-id="116e8-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="116e8-113">String collection</span></span>|<span data-ttu-id="116e8-114">Разрешенные действия — устарело</span><span class="sxs-lookup"><span data-stu-id="116e8-114">Allowed Actions - Deprecated</span></span>|
|<span data-ttu-id="116e8-115">resourceActions</span><span class="sxs-lookup"><span data-stu-id="116e8-115">resourceActions</span></span>|<span data-ttu-id="116e8-116">Коллекция объектов [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="116e8-116">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="116e8-117">Действия с ресурсами, содержащие набор разрешенных и запрещенных разрешений.</span><span class="sxs-lookup"><span data-stu-id="116e8-117">Resource Actions each containing a set of allowed and not allowed permissions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="116e8-118">Связи</span><span class="sxs-lookup"><span data-stu-id="116e8-118">Relationships</span></span>
<span data-ttu-id="116e8-119">Нет</span><span class="sxs-lookup"><span data-stu-id="116e8-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="116e8-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="116e8-120">JSON Representation</span></span>
<span data-ttu-id="116e8-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="116e8-121">Here is a JSON representation of the resource.</span></span>
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



