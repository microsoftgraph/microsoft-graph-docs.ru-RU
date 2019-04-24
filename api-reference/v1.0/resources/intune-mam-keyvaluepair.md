---
title: Тип ресурса keyValuePair
description: Пара "ключ-значение" для хранения пользовательских настроек
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ed4af707320da09c9b72537168f8fd77a424c790
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465435"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="8bd0c-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="8bd0c-103">keyValuePair resource type</span></span>

> <span data-ttu-id="8bd0c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8bd0c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bd0c-105">Пара "ключ-значение" для хранения пользовательских настроек</span><span class="sxs-lookup"><span data-stu-id="8bd0c-105">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="8bd0c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8bd0c-106">Properties</span></span>
|<span data-ttu-id="8bd0c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bd0c-107">Property</span></span>|<span data-ttu-id="8bd0c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8bd0c-108">Type</span></span>|<span data-ttu-id="8bd0c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8bd0c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bd0c-110">name</span><span class="sxs-lookup"><span data-stu-id="8bd0c-110">name</span></span>|<span data-ttu-id="8bd0c-111">String</span><span class="sxs-lookup"><span data-stu-id="8bd0c-111">String</span></span>|<span data-ttu-id="8bd0c-112">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="8bd0c-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="8bd0c-113">value</span><span class="sxs-lookup"><span data-stu-id="8bd0c-113">value</span></span>|<span data-ttu-id="8bd0c-114">String</span><span class="sxs-lookup"><span data-stu-id="8bd0c-114">String</span></span>|<span data-ttu-id="8bd0c-115">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="8bd0c-115">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="8bd0c-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="8bd0c-116">Relationships</span></span>
<span data-ttu-id="8bd0c-117">Нет</span><span class="sxs-lookup"><span data-stu-id="8bd0c-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8bd0c-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8bd0c-118">JSON Representation</span></span>
<span data-ttu-id="8bd0c-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8bd0c-119">Here is a JSON representation of the resource.</span></span>
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



