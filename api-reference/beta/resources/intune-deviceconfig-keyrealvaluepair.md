---
title: Тип ресурса Кэйреалвалуепаир
description: Значение типа "ключ-значение" с ключом строки и реальным значением (с плавающей запятой).
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 407ac4da833a75aa0a6708b6e392c9b1e08e9ba4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526264"
---
# <a name="keyrealvaluepair-resource-type"></a><span data-ttu-id="edd8c-103">Тип ресурса Кэйреалвалуепаир</span><span class="sxs-lookup"><span data-stu-id="edd8c-103">keyRealValuePair resource type</span></span>

<span data-ttu-id="edd8c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="edd8c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="edd8c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edd8c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="edd8c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="edd8c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edd8c-107">Значение типа "ключ-значение" с ключом строки и реальным значением (с плавающей запятой).</span><span class="sxs-lookup"><span data-stu-id="edd8c-107">A key-value pair with a string key and a real (floating-point) value.</span></span>


<span data-ttu-id="edd8c-108">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="edd8c-108">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="edd8c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="edd8c-109">Properties</span></span>
|<span data-ttu-id="edd8c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="edd8c-110">Property</span></span>|<span data-ttu-id="edd8c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="edd8c-111">Type</span></span>|<span data-ttu-id="edd8c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="edd8c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edd8c-113">key</span><span class="sxs-lookup"><span data-stu-id="edd8c-113">key</span></span>|<span data-ttu-id="edd8c-114">String</span><span class="sxs-lookup"><span data-stu-id="edd8c-114">String</span></span>|<span data-ttu-id="edd8c-115">Строковый ключ для типа "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="edd8c-115">The string key of the key-value pair.</span></span> <span data-ttu-id="edd8c-116">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="edd8c-116">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="edd8c-117">значение</span><span class="sxs-lookup"><span data-stu-id="edd8c-117">value</span></span>|<span data-ttu-id="edd8c-118">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="edd8c-118">Double</span></span>|<span data-ttu-id="edd8c-119">Реальное значение (число с плавающей запятой) для каждой из них: "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="edd8c-119">The real (floating-point) value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="edd8c-120">Связи</span><span class="sxs-lookup"><span data-stu-id="edd8c-120">Relationships</span></span>
<span data-ttu-id="edd8c-121">Нет</span><span class="sxs-lookup"><span data-stu-id="edd8c-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="edd8c-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="edd8c-122">JSON Representation</span></span>
<span data-ttu-id="edd8c-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="edd8c-123">Here is a JSON representation of the resource.</span></span>
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



