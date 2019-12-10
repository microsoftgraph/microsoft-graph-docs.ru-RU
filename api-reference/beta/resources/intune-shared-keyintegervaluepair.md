---
title: Тип ресурса Кэйинтежервалуепаир
description: Значение типа "ключ — значение" с ключом строки и целым значением.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8dc3185493501436f8cd7d7722379b09287e4dad
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39924551"
---
# <a name="keyintegervaluepair-resource-type"></a><span data-ttu-id="a6609-103">Тип ресурса Кэйинтежервалуепаир</span><span class="sxs-lookup"><span data-stu-id="a6609-103">keyIntegerValuePair resource type</span></span>

> <span data-ttu-id="a6609-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6609-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6609-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a6609-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6609-106">Значение типа "ключ — значение" с ключом строки и целым значением.</span><span class="sxs-lookup"><span data-stu-id="a6609-106">A key-value pair with a string key and an integer value.</span></span>


<span data-ttu-id="a6609-107">Наследуется от [кэйтипедвалуепаир](../resources/intune-shared-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="a6609-107">Inherits from [keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a6609-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a6609-108">Properties</span></span>
|<span data-ttu-id="a6609-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6609-109">Property</span></span>|<span data-ttu-id="a6609-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a6609-110">Type</span></span>|<span data-ttu-id="a6609-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a6609-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6609-112">key</span><span class="sxs-lookup"><span data-stu-id="a6609-112">key</span></span>|<span data-ttu-id="a6609-113">Строка</span><span class="sxs-lookup"><span data-stu-id="a6609-113">String</span></span>|<span data-ttu-id="a6609-114">Строковый ключ для типа "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="a6609-114">The string key of the key-value pair.</span></span> <span data-ttu-id="a6609-115">Наследуется от [кэйтипедвалуепаир](../resources/intune-shared-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="a6609-115">Inherited from [keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="a6609-116">value</span><span class="sxs-lookup"><span data-stu-id="a6609-116">value</span></span>|<span data-ttu-id="a6609-117">Int32</span><span class="sxs-lookup"><span data-stu-id="a6609-117">Int32</span></span>|<span data-ttu-id="a6609-118">Целочисленное значение для параметра "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="a6609-118">The integer value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6609-119">Связи</span><span class="sxs-lookup"><span data-stu-id="a6609-119">Relationships</span></span>
<span data-ttu-id="a6609-120">Нет</span><span class="sxs-lookup"><span data-stu-id="a6609-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a6609-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a6609-121">JSON Representation</span></span>
<span data-ttu-id="a6609-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6609-122">Here is a JSON representation of the resource.</span></span>
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



