---
title: Тип ресурса Кэйинтежервалуепаир
description: Значение типа "ключ — значение" с ключом строки и целым значением.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c0f9a3f05982daa036b1a2f38a09cb34011a3fb9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730469"
---
# <a name="keyintegervaluepair-resource-type"></a><span data-ttu-id="306a6-103">Тип ресурса Кэйинтежервалуепаир</span><span class="sxs-lookup"><span data-stu-id="306a6-103">keyIntegerValuePair resource type</span></span>

<span data-ttu-id="306a6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="306a6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="306a6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="306a6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="306a6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="306a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="306a6-107">Значение типа "ключ — значение" с ключом строки и целым значением.</span><span class="sxs-lookup"><span data-stu-id="306a6-107">A key-value pair with a string key and an integer value.</span></span>


<span data-ttu-id="306a6-108">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="306a6-108">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="306a6-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="306a6-109">Properties</span></span>
|<span data-ttu-id="306a6-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="306a6-110">Property</span></span>|<span data-ttu-id="306a6-111">Тип</span><span class="sxs-lookup"><span data-stu-id="306a6-111">Type</span></span>|<span data-ttu-id="306a6-112">Описание</span><span class="sxs-lookup"><span data-stu-id="306a6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="306a6-113">key</span><span class="sxs-lookup"><span data-stu-id="306a6-113">key</span></span>|<span data-ttu-id="306a6-114">Строка</span><span class="sxs-lookup"><span data-stu-id="306a6-114">String</span></span>|<span data-ttu-id="306a6-115">Строковый ключ для типа "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="306a6-115">The string key of the key-value pair.</span></span> <span data-ttu-id="306a6-116">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="306a6-116">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="306a6-117">value</span><span class="sxs-lookup"><span data-stu-id="306a6-117">value</span></span>|<span data-ttu-id="306a6-118">Int32</span><span class="sxs-lookup"><span data-stu-id="306a6-118">Int32</span></span>|<span data-ttu-id="306a6-119">Целочисленное значение для параметра "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="306a6-119">The integer value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="306a6-120">Связи</span><span class="sxs-lookup"><span data-stu-id="306a6-120">Relationships</span></span>
<span data-ttu-id="306a6-121">Нет</span><span class="sxs-lookup"><span data-stu-id="306a6-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="306a6-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="306a6-122">JSON Representation</span></span>
<span data-ttu-id="306a6-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="306a6-123">Here is a JSON representation of the resource.</span></span>
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





