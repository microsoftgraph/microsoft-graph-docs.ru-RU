---
title: Тип ресурса keyValuePair
description: Пара "ключ-значение" для хранения пользовательских настроек
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b5d4a294be690e012d43893e44540658e919c123
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010429"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="fdebe-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="fdebe-103">keyValuePair resource type</span></span>

> <span data-ttu-id="fdebe-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdebe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fdebe-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fdebe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdebe-106">Пара "ключ-значение" для хранения пользовательских настроек</span><span class="sxs-lookup"><span data-stu-id="fdebe-106">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="fdebe-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fdebe-107">Properties</span></span>
|<span data-ttu-id="fdebe-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdebe-108">Property</span></span>|<span data-ttu-id="fdebe-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fdebe-109">Type</span></span>|<span data-ttu-id="fdebe-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fdebe-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdebe-111">name</span><span class="sxs-lookup"><span data-stu-id="fdebe-111">name</span></span>|<span data-ttu-id="fdebe-112">String</span><span class="sxs-lookup"><span data-stu-id="fdebe-112">String</span></span>|<span data-ttu-id="fdebe-113">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="fdebe-113">Name for this key-value pair</span></span>|
|<span data-ttu-id="fdebe-114">value</span><span class="sxs-lookup"><span data-stu-id="fdebe-114">value</span></span>|<span data-ttu-id="fdebe-115">String</span><span class="sxs-lookup"><span data-stu-id="fdebe-115">String</span></span>|<span data-ttu-id="fdebe-116">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="fdebe-116">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="fdebe-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="fdebe-117">Relationships</span></span>
<span data-ttu-id="fdebe-118">Нет</span><span class="sxs-lookup"><span data-stu-id="fdebe-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fdebe-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fdebe-119">JSON Representation</span></span>
<span data-ttu-id="fdebe-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fdebe-120">Here is a JSON representation of the resource.</span></span>
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





