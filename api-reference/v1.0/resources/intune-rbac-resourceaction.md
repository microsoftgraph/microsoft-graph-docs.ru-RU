---
title: Тип ресурса resourceAction
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 88ea0c947a87135f874755f49d0847a3c2a08fae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037158"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="fd439-103">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="fd439-103">resourceAction resource type</span></span>

> <span data-ttu-id="fd439-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fd439-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd439-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fd439-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="fd439-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="fd439-106">Properties</span></span>
|<span data-ttu-id="fd439-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd439-107">Property</span></span>|<span data-ttu-id="fd439-108">Тип</span><span class="sxs-lookup"><span data-stu-id="fd439-108">Type</span></span>|<span data-ttu-id="fd439-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fd439-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd439-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="fd439-110">allowedResourceActions</span></span>|<span data-ttu-id="fd439-111">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fd439-111">String collection</span></span>|<span data-ttu-id="fd439-112">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="fd439-112">Allowed Actions</span></span>|
|<span data-ttu-id="fd439-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="fd439-113">notAllowedResourceActions</span></span>|<span data-ttu-id="fd439-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fd439-114">String collection</span></span>|<span data-ttu-id="fd439-115">Запрещенные действия</span><span class="sxs-lookup"><span data-stu-id="fd439-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd439-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="fd439-116">Relationships</span></span>
<span data-ttu-id="fd439-117">Нет</span><span class="sxs-lookup"><span data-stu-id="fd439-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd439-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fd439-118">JSON Representation</span></span>
<span data-ttu-id="fd439-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd439-119">Here is a JSON representation of the resource.</span></span>
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



