---
title: Тип ресурса Кэйреалвалуепаир
description: Значение типа "ключ-значение" с ключом строки и реальным значением (с плавающей запятой).
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6b90c7faa0bb3ffabe5b057d03503745801af8c8
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790428"
---
# <a name="keyrealvaluepair-resource-type"></a><span data-ttu-id="10221-103">Тип ресурса Кэйреалвалуепаир</span><span class="sxs-lookup"><span data-stu-id="10221-103">keyRealValuePair resource type</span></span>

> <span data-ttu-id="10221-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10221-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10221-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="10221-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10221-106">Значение типа "ключ-значение" с ключом строки и реальным значением (с плавающей запятой).</span><span class="sxs-lookup"><span data-stu-id="10221-106">A key-value pair with a string key and a real (floating-point) value.</span></span>


<span data-ttu-id="10221-107">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="10221-107">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="10221-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="10221-108">Properties</span></span>
|<span data-ttu-id="10221-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="10221-109">Property</span></span>|<span data-ttu-id="10221-110">Тип</span><span class="sxs-lookup"><span data-stu-id="10221-110">Type</span></span>|<span data-ttu-id="10221-111">Описание</span><span class="sxs-lookup"><span data-stu-id="10221-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10221-112">key</span><span class="sxs-lookup"><span data-stu-id="10221-112">key</span></span>|<span data-ttu-id="10221-113">String</span><span class="sxs-lookup"><span data-stu-id="10221-113">String</span></span>|<span data-ttu-id="10221-114">Строковый ключ для типа "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="10221-114">The string key of the key-value pair.</span></span> <span data-ttu-id="10221-115">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="10221-115">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="10221-116">значение</span><span class="sxs-lookup"><span data-stu-id="10221-116">value</span></span>|<span data-ttu-id="10221-117">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="10221-117">Double</span></span>|<span data-ttu-id="10221-118">Реальное значение (число с плавающей запятой) для каждой из них: "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="10221-118">The real (floating-point) value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10221-119">Связи</span><span class="sxs-lookup"><span data-stu-id="10221-119">Relationships</span></span>
<span data-ttu-id="10221-120">Нет</span><span class="sxs-lookup"><span data-stu-id="10221-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10221-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="10221-121">JSON Representation</span></span>
<span data-ttu-id="10221-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10221-122">Here is a JSON representation of the resource.</span></span>
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



