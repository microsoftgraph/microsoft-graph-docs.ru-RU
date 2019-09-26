---
title: Тип ресурса Кэйинтежервалуепаир
description: Значение типа "ключ — значение" с ключом строки и целым значением.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0cd9c4de9f7c2505b12eada575ebc5d869480758
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201308"
---
# <a name="keyintegervaluepair-resource-type"></a><span data-ttu-id="4a792-103">Тип ресурса Кэйинтежервалуепаир</span><span class="sxs-lookup"><span data-stu-id="4a792-103">keyIntegerValuePair resource type</span></span>

> <span data-ttu-id="4a792-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a792-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a792-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a792-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a792-106">Значение типа "ключ — значение" с ключом строки и целым значением.</span><span class="sxs-lookup"><span data-stu-id="4a792-106">A key-value pair with a string key and an integer value.</span></span>


<span data-ttu-id="4a792-107">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="4a792-107">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4a792-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4a792-108">Properties</span></span>
|<span data-ttu-id="4a792-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a792-109">Property</span></span>|<span data-ttu-id="4a792-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4a792-110">Type</span></span>|<span data-ttu-id="4a792-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4a792-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a792-112">key</span><span class="sxs-lookup"><span data-stu-id="4a792-112">key</span></span>|<span data-ttu-id="4a792-113">String.</span><span class="sxs-lookup"><span data-stu-id="4a792-113">String</span></span>|<span data-ttu-id="4a792-114">Строковый ключ для типа "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="4a792-114">The string key of the key-value pair.</span></span> <span data-ttu-id="4a792-115">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="4a792-115">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="4a792-116">value</span><span class="sxs-lookup"><span data-stu-id="4a792-116">value</span></span>|<span data-ttu-id="4a792-117">Int32</span><span class="sxs-lookup"><span data-stu-id="4a792-117">Int32</span></span>|<span data-ttu-id="4a792-118">Целочисленное значение для параметра "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="4a792-118">The integer value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a792-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="4a792-119">Relationships</span></span>
<span data-ttu-id="4a792-120">Нет</span><span class="sxs-lookup"><span data-stu-id="4a792-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a792-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4a792-121">JSON Representation</span></span>
<span data-ttu-id="4a792-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a792-122">Here is a JSON representation of the resource.</span></span>
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



