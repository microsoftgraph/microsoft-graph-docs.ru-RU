---
title: Тип ресурса resourceAction
description: Набор разрешенных и запрещенных действий для ресурса.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 597a9c7cdc2f04247e799772f100d1a0b778453e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939989"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="86ceb-103">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="86ceb-103">resourceAction resource type</span></span>

> <span data-ttu-id="86ceb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86ceb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86ceb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="86ceb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86ceb-106">Набор разрешенных и запрещенных действий для ресурса.</span><span class="sxs-lookup"><span data-stu-id="86ceb-106">Set of allowed and not allowed actions for a resource.</span></span>

## <a name="properties"></a><span data-ttu-id="86ceb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="86ceb-107">Properties</span></span>
|<span data-ttu-id="86ceb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="86ceb-108">Property</span></span>|<span data-ttu-id="86ceb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="86ceb-109">Type</span></span>|<span data-ttu-id="86ceb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="86ceb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86ceb-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="86ceb-111">allowedResourceActions</span></span>|<span data-ttu-id="86ceb-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="86ceb-112">String collection</span></span>|<span data-ttu-id="86ceb-113">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="86ceb-113">Allowed Actions</span></span>|
|<span data-ttu-id="86ceb-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="86ceb-114">notAllowedResourceActions</span></span>|<span data-ttu-id="86ceb-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="86ceb-115">String collection</span></span>|<span data-ttu-id="86ceb-116">Действия не разрешены.</span><span class="sxs-lookup"><span data-stu-id="86ceb-116">Not Allowed Actions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86ceb-117">Связи</span><span class="sxs-lookup"><span data-stu-id="86ceb-117">Relationships</span></span>
<span data-ttu-id="86ceb-118">Нет</span><span class="sxs-lookup"><span data-stu-id="86ceb-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="86ceb-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="86ceb-119">JSON Representation</span></span>
<span data-ttu-id="86ceb-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86ceb-120">Here is a JSON representation of the resource.</span></span>
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




