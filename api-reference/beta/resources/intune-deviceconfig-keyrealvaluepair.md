---
title: Тип ресурса Кэйреалвалуепаир
description: Значение типа "ключ-значение" с ключом строки и реальным значением (с плавающей запятой).
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3f8611f5739862e659abaa2581943a30416f2138
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201307"
---
# <a name="keyrealvaluepair-resource-type"></a><span data-ttu-id="c32f6-103">Тип ресурса Кэйреалвалуепаир</span><span class="sxs-lookup"><span data-stu-id="c32f6-103">keyRealValuePair resource type</span></span>

> <span data-ttu-id="c32f6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c32f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c32f6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c32f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c32f6-106">Значение типа "ключ-значение" с ключом строки и реальным значением (с плавающей запятой).</span><span class="sxs-lookup"><span data-stu-id="c32f6-106">A key-value pair with a string key and a real (floating-point) value.</span></span>


<span data-ttu-id="c32f6-107">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c32f6-107">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c32f6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c32f6-108">Properties</span></span>
|<span data-ttu-id="c32f6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c32f6-109">Property</span></span>|<span data-ttu-id="c32f6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c32f6-110">Type</span></span>|<span data-ttu-id="c32f6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c32f6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c32f6-112">key</span><span class="sxs-lookup"><span data-stu-id="c32f6-112">key</span></span>|<span data-ttu-id="c32f6-113">String.</span><span class="sxs-lookup"><span data-stu-id="c32f6-113">String</span></span>|<span data-ttu-id="c32f6-114">Строковый ключ для типа "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="c32f6-114">The string key of the key-value pair.</span></span> <span data-ttu-id="c32f6-115">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c32f6-115">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="c32f6-116">значение</span><span class="sxs-lookup"><span data-stu-id="c32f6-116">value</span></span>|<span data-ttu-id="c32f6-117">Двойное</span><span class="sxs-lookup"><span data-stu-id="c32f6-117">Double</span></span>|<span data-ttu-id="c32f6-118">Реальное значение (число с плавающей запятой) для каждой из них: "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="c32f6-118">The real (floating-point) value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c32f6-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="c32f6-119">Relationships</span></span>
<span data-ttu-id="c32f6-120">Нет</span><span class="sxs-lookup"><span data-stu-id="c32f6-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c32f6-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c32f6-121">JSON Representation</span></span>
<span data-ttu-id="c32f6-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c32f6-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyRealValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyRealValuePair",
  "key": "String",
  "value": "<Unknown Primitive Type Edm.Double>"
}
```



