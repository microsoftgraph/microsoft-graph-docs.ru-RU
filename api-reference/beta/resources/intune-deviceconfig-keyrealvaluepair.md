---
title: Тип ресурса Кэйреалвалуепаир
description: Значение типа "ключ-значение" с ключом строки и реальным значением (с плавающей запятой).
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7b5b9860cb4ef161cc057013db889fd1bb626be6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439968"
---
# <a name="keyrealvaluepair-resource-type"></a><span data-ttu-id="7e20e-103">Тип ресурса Кэйреалвалуепаир</span><span class="sxs-lookup"><span data-stu-id="7e20e-103">keyRealValuePair resource type</span></span>

<span data-ttu-id="7e20e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e20e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7e20e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e20e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e20e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e20e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e20e-107">Значение типа "ключ-значение" с ключом строки и реальным значением (с плавающей запятой).</span><span class="sxs-lookup"><span data-stu-id="7e20e-107">A key-value pair with a string key and a real (floating-point) value.</span></span>


<span data-ttu-id="7e20e-108">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="7e20e-108">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7e20e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7e20e-109">Properties</span></span>
|<span data-ttu-id="7e20e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e20e-110">Property</span></span>|<span data-ttu-id="7e20e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7e20e-111">Type</span></span>|<span data-ttu-id="7e20e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7e20e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e20e-113">key</span><span class="sxs-lookup"><span data-stu-id="7e20e-113">key</span></span>|<span data-ttu-id="7e20e-114">String</span><span class="sxs-lookup"><span data-stu-id="7e20e-114">String</span></span>|<span data-ttu-id="7e20e-115">Строковый ключ для типа "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="7e20e-115">The string key of the key-value pair.</span></span> <span data-ttu-id="7e20e-116">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="7e20e-116">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="7e20e-117">значение</span><span class="sxs-lookup"><span data-stu-id="7e20e-117">value</span></span>|<span data-ttu-id="7e20e-118">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="7e20e-118">Double</span></span>|<span data-ttu-id="7e20e-119">Реальное значение (число с плавающей запятой) для каждой из них: "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="7e20e-119">The real (floating-point) value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e20e-120">Связи</span><span class="sxs-lookup"><span data-stu-id="7e20e-120">Relationships</span></span>
<span data-ttu-id="7e20e-121">Нет</span><span class="sxs-lookup"><span data-stu-id="7e20e-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e20e-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7e20e-122">JSON Representation</span></span>
<span data-ttu-id="7e20e-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e20e-123">Here is a JSON representation of the resource.</span></span>
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



