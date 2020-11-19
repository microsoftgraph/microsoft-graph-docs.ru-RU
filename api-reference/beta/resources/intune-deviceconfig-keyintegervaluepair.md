---
title: Тип ресурса Кэйинтежервалуепаир
description: Значение типа "ключ — значение" с ключом строки и целым значением.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f8cdc38003e1c16c91b1ff734e74e1c7bd6fee18
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49269177"
---
# <a name="keyintegervaluepair-resource-type"></a><span data-ttu-id="4ea07-103">Тип ресурса Кэйинтежервалуепаир</span><span class="sxs-lookup"><span data-stu-id="4ea07-103">keyIntegerValuePair resource type</span></span>

<span data-ttu-id="4ea07-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ea07-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ea07-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ea07-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ea07-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4ea07-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ea07-107">Значение типа "ключ — значение" с ключом строки и целым значением.</span><span class="sxs-lookup"><span data-stu-id="4ea07-107">A key-value pair with a string key and an integer value.</span></span>


<span data-ttu-id="4ea07-108">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="4ea07-108">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4ea07-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ea07-109">Properties</span></span>
|<span data-ttu-id="4ea07-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ea07-110">Property</span></span>|<span data-ttu-id="4ea07-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4ea07-111">Type</span></span>|<span data-ttu-id="4ea07-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4ea07-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ea07-113">key</span><span class="sxs-lookup"><span data-stu-id="4ea07-113">key</span></span>|<span data-ttu-id="4ea07-114">String</span><span class="sxs-lookup"><span data-stu-id="4ea07-114">String</span></span>|<span data-ttu-id="4ea07-115">Строковый ключ для типа "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="4ea07-115">The string key of the key-value pair.</span></span> <span data-ttu-id="4ea07-116">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="4ea07-116">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="4ea07-117">value</span><span class="sxs-lookup"><span data-stu-id="4ea07-117">value</span></span>|<span data-ttu-id="4ea07-118">Int32</span><span class="sxs-lookup"><span data-stu-id="4ea07-118">Int32</span></span>|<span data-ttu-id="4ea07-119">Целочисленное значение для параметра "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="4ea07-119">The integer value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ea07-120">Связи</span><span class="sxs-lookup"><span data-stu-id="4ea07-120">Relationships</span></span>
<span data-ttu-id="4ea07-121">Нет</span><span class="sxs-lookup"><span data-stu-id="4ea07-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ea07-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ea07-122">JSON Representation</span></span>
<span data-ttu-id="4ea07-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ea07-123">Here is a JSON representation of the resource.</span></span>
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




