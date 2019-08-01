---
title: Тип ресурса keyValuePair
description: Пара "ключ-значение" для хранения пользовательских настроек
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fd0f9c6e17d1550e4b2584200239ff303ba91232
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36038117"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="3802a-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="3802a-103">keyValuePair resource type</span></span>

> <span data-ttu-id="3802a-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3802a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3802a-105">Пара "ключ-значение" для хранения пользовательских настроек</span><span class="sxs-lookup"><span data-stu-id="3802a-105">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="3802a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3802a-106">Properties</span></span>
|<span data-ttu-id="3802a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3802a-107">Property</span></span>|<span data-ttu-id="3802a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3802a-108">Type</span></span>|<span data-ttu-id="3802a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3802a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3802a-110">name</span><span class="sxs-lookup"><span data-stu-id="3802a-110">name</span></span>|<span data-ttu-id="3802a-111">String</span><span class="sxs-lookup"><span data-stu-id="3802a-111">String</span></span>|<span data-ttu-id="3802a-112">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="3802a-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="3802a-113">value</span><span class="sxs-lookup"><span data-stu-id="3802a-113">value</span></span>|<span data-ttu-id="3802a-114">String</span><span class="sxs-lookup"><span data-stu-id="3802a-114">String</span></span>|<span data-ttu-id="3802a-115">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="3802a-115">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="3802a-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="3802a-116">Relationships</span></span>
<span data-ttu-id="3802a-117">Нет</span><span class="sxs-lookup"><span data-stu-id="3802a-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3802a-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3802a-118">JSON Representation</span></span>
<span data-ttu-id="3802a-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3802a-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```



