---
title: Тип ресурса Кэйинтежервалуепаир
description: Значение типа "ключ — значение" с ключом строки и целым значением.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0f2a3f4201956db2cbca001f8d94f6ae6ecc90d7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790435"
---
# <a name="keyintegervaluepair-resource-type"></a><span data-ttu-id="78939-103">Тип ресурса Кэйинтежервалуепаир</span><span class="sxs-lookup"><span data-stu-id="78939-103">keyIntegerValuePair resource type</span></span>

> <span data-ttu-id="78939-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78939-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78939-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="78939-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78939-106">Значение типа "ключ — значение" с ключом строки и целым значением.</span><span class="sxs-lookup"><span data-stu-id="78939-106">A key-value pair with a string key and an integer value.</span></span>


<span data-ttu-id="78939-107">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="78939-107">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="78939-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="78939-108">Properties</span></span>
|<span data-ttu-id="78939-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="78939-109">Property</span></span>|<span data-ttu-id="78939-110">Тип</span><span class="sxs-lookup"><span data-stu-id="78939-110">Type</span></span>|<span data-ttu-id="78939-111">Описание</span><span class="sxs-lookup"><span data-stu-id="78939-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78939-112">key</span><span class="sxs-lookup"><span data-stu-id="78939-112">key</span></span>|<span data-ttu-id="78939-113">String</span><span class="sxs-lookup"><span data-stu-id="78939-113">String</span></span>|<span data-ttu-id="78939-114">Строковый ключ для типа "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="78939-114">The string key of the key-value pair.</span></span> <span data-ttu-id="78939-115">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="78939-115">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="78939-116">value</span><span class="sxs-lookup"><span data-stu-id="78939-116">value</span></span>|<span data-ttu-id="78939-117">Int32</span><span class="sxs-lookup"><span data-stu-id="78939-117">Int32</span></span>|<span data-ttu-id="78939-118">Целочисленное значение для параметра "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="78939-118">The integer value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78939-119">Связи</span><span class="sxs-lookup"><span data-stu-id="78939-119">Relationships</span></span>
<span data-ttu-id="78939-120">Нет</span><span class="sxs-lookup"><span data-stu-id="78939-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="78939-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="78939-121">JSON Representation</span></span>
<span data-ttu-id="78939-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="78939-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyIntegerValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyIntegerValuePair",
  "key": "String",
  "value": 1024
}
```



