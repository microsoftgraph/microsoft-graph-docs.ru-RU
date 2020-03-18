---
title: Тип ресурса keyValuePair
description: Пара "ключ-значение" для хранения пользовательских настроек
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cd97b7cf0729ae9e1cad1c8440ec9727cc321a67
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42769131"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="390b1-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="390b1-103">keyValuePair resource type</span></span>

> <span data-ttu-id="390b1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="390b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="390b1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="390b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="390b1-106">Пара "ключ-значение" для хранения пользовательских настроек</span><span class="sxs-lookup"><span data-stu-id="390b1-106">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="390b1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="390b1-107">Properties</span></span>
|<span data-ttu-id="390b1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="390b1-108">Property</span></span>|<span data-ttu-id="390b1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="390b1-109">Type</span></span>|<span data-ttu-id="390b1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="390b1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="390b1-111">name</span><span class="sxs-lookup"><span data-stu-id="390b1-111">name</span></span>|<span data-ttu-id="390b1-112">String</span><span class="sxs-lookup"><span data-stu-id="390b1-112">String</span></span>|<span data-ttu-id="390b1-113">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="390b1-113">Name for this key-value pair</span></span>|
|<span data-ttu-id="390b1-114">value</span><span class="sxs-lookup"><span data-stu-id="390b1-114">value</span></span>|<span data-ttu-id="390b1-115">String</span><span class="sxs-lookup"><span data-stu-id="390b1-115">String</span></span>|<span data-ttu-id="390b1-116">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="390b1-116">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="390b1-117">Связи</span><span class="sxs-lookup"><span data-stu-id="390b1-117">Relationships</span></span>
<span data-ttu-id="390b1-118">Нет</span><span class="sxs-lookup"><span data-stu-id="390b1-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="390b1-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="390b1-119">JSON Representation</span></span>
<span data-ttu-id="390b1-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="390b1-120">Here is a JSON representation of the resource.</span></span>
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



