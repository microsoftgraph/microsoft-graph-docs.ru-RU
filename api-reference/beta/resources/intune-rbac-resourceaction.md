---
title: Тип ресурса resourceAction
description: Набор разрешенных и запрещенных действий для ресурса.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 256db900b85142ebe10cfcacf571bc3c29526359
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43357555"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="79a04-103">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="79a04-103">resourceAction resource type</span></span>

<span data-ttu-id="79a04-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79a04-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79a04-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79a04-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79a04-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="79a04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79a04-107">Набор разрешенных и запрещенных действий для ресурса.</span><span class="sxs-lookup"><span data-stu-id="79a04-107">Set of allowed and not allowed actions for a resource.</span></span>

## <a name="properties"></a><span data-ttu-id="79a04-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="79a04-108">Properties</span></span>
|<span data-ttu-id="79a04-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="79a04-109">Property</span></span>|<span data-ttu-id="79a04-110">Тип</span><span class="sxs-lookup"><span data-stu-id="79a04-110">Type</span></span>|<span data-ttu-id="79a04-111">Описание</span><span class="sxs-lookup"><span data-stu-id="79a04-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79a04-112">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="79a04-112">allowedResourceActions</span></span>|<span data-ttu-id="79a04-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="79a04-113">String collection</span></span>|<span data-ttu-id="79a04-114">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="79a04-114">Allowed Actions</span></span>|
|<span data-ttu-id="79a04-115">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="79a04-115">notAllowedResourceActions</span></span>|<span data-ttu-id="79a04-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="79a04-116">String collection</span></span>|<span data-ttu-id="79a04-117">Действия не разрешены.</span><span class="sxs-lookup"><span data-stu-id="79a04-117">Not Allowed Actions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79a04-118">Связи</span><span class="sxs-lookup"><span data-stu-id="79a04-118">Relationships</span></span>
<span data-ttu-id="79a04-119">Нет</span><span class="sxs-lookup"><span data-stu-id="79a04-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="79a04-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="79a04-120">JSON Representation</span></span>
<span data-ttu-id="79a04-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79a04-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```



