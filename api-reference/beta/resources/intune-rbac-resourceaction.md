---
title: Тип ресурса resourceAction
description: Набор разрешенных и запрещенных действий для ресурса.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a07701a516c1ebdaf78e98b97be47d37b876c945
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369292"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="e9724-103">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="e9724-103">resourceAction resource type</span></span>

> <span data-ttu-id="e9724-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9724-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9724-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e9724-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9724-106">Набор разрешенных и запрещенных действий для ресурса.</span><span class="sxs-lookup"><span data-stu-id="e9724-106">Set of allowed and not allowed actions for a resource.</span></span>

## <a name="properties"></a><span data-ttu-id="e9724-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9724-107">Properties</span></span>
|<span data-ttu-id="e9724-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9724-108">Property</span></span>|<span data-ttu-id="e9724-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e9724-109">Type</span></span>|<span data-ttu-id="e9724-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e9724-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9724-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="e9724-111">allowedResourceActions</span></span>|<span data-ttu-id="e9724-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e9724-112">String collection</span></span>|<span data-ttu-id="e9724-113">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="e9724-113">Allowed Actions</span></span>|
|<span data-ttu-id="e9724-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="e9724-114">notAllowedResourceActions</span></span>|<span data-ttu-id="e9724-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e9724-115">String collection</span></span>|<span data-ttu-id="e9724-116">Действия не разрешены.</span><span class="sxs-lookup"><span data-stu-id="e9724-116">Not Allowed Actions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9724-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="e9724-117">Relationships</span></span>
<span data-ttu-id="e9724-118">Нет</span><span class="sxs-lookup"><span data-stu-id="e9724-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9724-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e9724-119">JSON Representation</span></span>
<span data-ttu-id="e9724-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9724-120">Here is a JSON representation of the resource.</span></span>
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



