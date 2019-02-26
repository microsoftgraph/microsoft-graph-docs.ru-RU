---
title: Тип ресурса resourceAction
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a48d09d8aeadc9a5d60559d25a4bdcc322d10f21
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262183"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="d05a3-103">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="d05a3-103">resourceAction resource type</span></span>

> <span data-ttu-id="d05a3-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d05a3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d05a3-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d05a3-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d05a3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d05a3-106">Properties</span></span>
|<span data-ttu-id="d05a3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d05a3-107">Property</span></span>|<span data-ttu-id="d05a3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d05a3-108">Type</span></span>|<span data-ttu-id="d05a3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d05a3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d05a3-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="d05a3-110">allowedResourceActions</span></span>|<span data-ttu-id="d05a3-111">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d05a3-111">String collection</span></span>|<span data-ttu-id="d05a3-112">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="d05a3-112">Allowed Actions</span></span>|
|<span data-ttu-id="d05a3-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="d05a3-113">notAllowedResourceActions</span></span>|<span data-ttu-id="d05a3-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d05a3-114">String collection</span></span>|<span data-ttu-id="d05a3-115">Запрещенные действия</span><span class="sxs-lookup"><span data-stu-id="d05a3-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="d05a3-116">Связи</span><span class="sxs-lookup"><span data-stu-id="d05a3-116">Relationships</span></span>
<span data-ttu-id="d05a3-117">Нет</span><span class="sxs-lookup"><span data-stu-id="d05a3-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d05a3-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d05a3-118">JSON Representation</span></span>
<span data-ttu-id="d05a3-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d05a3-119">Here is a JSON representation of the resource.</span></span>
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



