---
title: Тип ресурса keyValuePair
description: Пара "ключ-значение" для хранения пользовательских настроек
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 69924cf755192d8ddefa074b9ec1cfed53a0d5f7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347950"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="77bd0-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="77bd0-103">keyValuePair resource type</span></span>

> <span data-ttu-id="77bd0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77bd0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77bd0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77bd0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77bd0-106">Пара "ключ-значение" для хранения пользовательских настроек</span><span class="sxs-lookup"><span data-stu-id="77bd0-106">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="77bd0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="77bd0-107">Properties</span></span>
|<span data-ttu-id="77bd0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="77bd0-108">Property</span></span>|<span data-ttu-id="77bd0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="77bd0-109">Type</span></span>|<span data-ttu-id="77bd0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="77bd0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77bd0-111">name</span><span class="sxs-lookup"><span data-stu-id="77bd0-111">name</span></span>|<span data-ttu-id="77bd0-112">String</span><span class="sxs-lookup"><span data-stu-id="77bd0-112">String</span></span>|<span data-ttu-id="77bd0-113">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="77bd0-113">Name for this key-value pair</span></span>|
|<span data-ttu-id="77bd0-114">value</span><span class="sxs-lookup"><span data-stu-id="77bd0-114">value</span></span>|<span data-ttu-id="77bd0-115">String</span><span class="sxs-lookup"><span data-stu-id="77bd0-115">String</span></span>|<span data-ttu-id="77bd0-116">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="77bd0-116">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="77bd0-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="77bd0-117">Relationships</span></span>
<span data-ttu-id="77bd0-118">Нет</span><span class="sxs-lookup"><span data-stu-id="77bd0-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77bd0-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="77bd0-119">JSON Representation</span></span>
<span data-ttu-id="77bd0-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77bd0-120">Here is a JSON representation of the resource.</span></span>
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



