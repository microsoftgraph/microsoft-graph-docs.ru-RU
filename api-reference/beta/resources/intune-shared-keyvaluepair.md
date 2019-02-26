---
title: Тип ресурса keyValuePair
description: Пара "ключ-значение" для хранения пользовательских настроек
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5a8feecabeca3cfc916c0bd3ce1b87cab3a68809
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160797"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="4c1f9-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="4c1f9-103">keyValuePair resource type</span></span>

> <span data-ttu-id="4c1f9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c1f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c1f9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4c1f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c1f9-106">Пара "ключ-значение" для хранения пользовательских настроек</span><span class="sxs-lookup"><span data-stu-id="4c1f9-106">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="4c1f9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4c1f9-107">Properties</span></span>
|<span data-ttu-id="4c1f9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c1f9-108">Property</span></span>|<span data-ttu-id="4c1f9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4c1f9-109">Type</span></span>|<span data-ttu-id="4c1f9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4c1f9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c1f9-111">name</span><span class="sxs-lookup"><span data-stu-id="4c1f9-111">name</span></span>|<span data-ttu-id="4c1f9-112">String</span><span class="sxs-lookup"><span data-stu-id="4c1f9-112">String</span></span>|<span data-ttu-id="4c1f9-113">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="4c1f9-113">Name for this key-value pair</span></span>|
|<span data-ttu-id="4c1f9-114">value</span><span class="sxs-lookup"><span data-stu-id="4c1f9-114">value</span></span>|<span data-ttu-id="4c1f9-115">String</span><span class="sxs-lookup"><span data-stu-id="4c1f9-115">String</span></span>|<span data-ttu-id="4c1f9-116">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="4c1f9-116">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c1f9-117">Связи</span><span class="sxs-lookup"><span data-stu-id="4c1f9-117">Relationships</span></span>
<span data-ttu-id="4c1f9-118">Нет</span><span class="sxs-lookup"><span data-stu-id="4c1f9-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c1f9-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4c1f9-119">JSON Representation</span></span>
<span data-ttu-id="4c1f9-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c1f9-120">Here is a JSON representation of the resource.</span></span>
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




