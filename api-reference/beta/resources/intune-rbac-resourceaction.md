---
title: Тип ресурса resourceAction
description: Набор разрешенных и запрещенных действий для ресурса.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 48d687fd6878256c43e9c95e167432d3e7454695
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42773737"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="f4338-103">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="f4338-103">resourceAction resource type</span></span>

> <span data-ttu-id="f4338-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4338-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4338-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f4338-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4338-106">Набор разрешенных и запрещенных действий для ресурса.</span><span class="sxs-lookup"><span data-stu-id="f4338-106">Set of allowed and not allowed actions for a resource.</span></span>

## <a name="properties"></a><span data-ttu-id="f4338-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f4338-107">Properties</span></span>
|<span data-ttu-id="f4338-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4338-108">Property</span></span>|<span data-ttu-id="f4338-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f4338-109">Type</span></span>|<span data-ttu-id="f4338-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f4338-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4338-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="f4338-111">allowedResourceActions</span></span>|<span data-ttu-id="f4338-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f4338-112">String collection</span></span>|<span data-ttu-id="f4338-113">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="f4338-113">Allowed Actions</span></span>|
|<span data-ttu-id="f4338-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="f4338-114">notAllowedResourceActions</span></span>|<span data-ttu-id="f4338-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f4338-115">String collection</span></span>|<span data-ttu-id="f4338-116">Действия не разрешены.</span><span class="sxs-lookup"><span data-stu-id="f4338-116">Not Allowed Actions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4338-117">Связи</span><span class="sxs-lookup"><span data-stu-id="f4338-117">Relationships</span></span>
<span data-ttu-id="f4338-118">Нет</span><span class="sxs-lookup"><span data-stu-id="f4338-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4338-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f4338-119">JSON Representation</span></span>
<span data-ttu-id="f4338-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4338-120">Here is a JSON representation of the resource.</span></span>
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



