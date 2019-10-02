---
title: Тип ресурса resourceAction
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c30c9a272029fc681a383772b2467dc6fb67af88
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359028"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="4a517-103">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="4a517-103">resourceAction resource type</span></span>

> <span data-ttu-id="4a517-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a517-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a517-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4a517-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="4a517-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4a517-106">Properties</span></span>
|<span data-ttu-id="4a517-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a517-107">Property</span></span>|<span data-ttu-id="4a517-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4a517-108">Type</span></span>|<span data-ttu-id="4a517-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4a517-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a517-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="4a517-110">allowedResourceActions</span></span>|<span data-ttu-id="4a517-111">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4a517-111">String collection</span></span>|<span data-ttu-id="4a517-112">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="4a517-112">Allowed Actions</span></span>|
|<span data-ttu-id="4a517-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="4a517-113">notAllowedResourceActions</span></span>|<span data-ttu-id="4a517-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4a517-114">String collection</span></span>|<span data-ttu-id="4a517-115">Запрещенные действия</span><span class="sxs-lookup"><span data-stu-id="4a517-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a517-116">Связи</span><span class="sxs-lookup"><span data-stu-id="4a517-116">Relationships</span></span>
<span data-ttu-id="4a517-117">Нет</span><span class="sxs-lookup"><span data-stu-id="4a517-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a517-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4a517-118">JSON Representation</span></span>
<span data-ttu-id="4a517-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a517-119">Here is a JSON representation of the resource.</span></span>
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




