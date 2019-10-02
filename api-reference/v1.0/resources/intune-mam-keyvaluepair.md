---
title: Тип ресурса keyValuePair
description: Пара "ключ-значение" для хранения пользовательских настроек
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2849e6adfc0b43b9091764cd2706d5c572826774
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356438"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="89c59-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="89c59-103">keyValuePair resource type</span></span>

> <span data-ttu-id="89c59-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89c59-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89c59-105">Пара "ключ-значение" для хранения пользовательских настроек</span><span class="sxs-lookup"><span data-stu-id="89c59-105">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="89c59-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="89c59-106">Properties</span></span>
|<span data-ttu-id="89c59-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="89c59-107">Property</span></span>|<span data-ttu-id="89c59-108">Тип</span><span class="sxs-lookup"><span data-stu-id="89c59-108">Type</span></span>|<span data-ttu-id="89c59-109">Описание</span><span class="sxs-lookup"><span data-stu-id="89c59-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89c59-110">name</span><span class="sxs-lookup"><span data-stu-id="89c59-110">name</span></span>|<span data-ttu-id="89c59-111">String</span><span class="sxs-lookup"><span data-stu-id="89c59-111">String</span></span>|<span data-ttu-id="89c59-112">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="89c59-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="89c59-113">value</span><span class="sxs-lookup"><span data-stu-id="89c59-113">value</span></span>|<span data-ttu-id="89c59-114">String</span><span class="sxs-lookup"><span data-stu-id="89c59-114">String</span></span>|<span data-ttu-id="89c59-115">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="89c59-115">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="89c59-116">Связи</span><span class="sxs-lookup"><span data-stu-id="89c59-116">Relationships</span></span>
<span data-ttu-id="89c59-117">Нет</span><span class="sxs-lookup"><span data-stu-id="89c59-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="89c59-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="89c59-118">JSON Representation</span></span>
<span data-ttu-id="89c59-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89c59-119">Here is a JSON representation of the resource.</span></span>
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




