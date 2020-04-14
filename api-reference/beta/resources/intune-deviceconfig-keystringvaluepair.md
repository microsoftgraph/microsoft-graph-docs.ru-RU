---
title: Тип ресурса Кэйстрингвалуепаир
description: Значение типа "ключ — значение" со строковым ключом и строковым значением.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c79775d4822476ab0922330581dd6b54639e4eb3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439923"
---
# <a name="keystringvaluepair-resource-type"></a><span data-ttu-id="c2623-103">Тип ресурса Кэйстрингвалуепаир</span><span class="sxs-lookup"><span data-stu-id="c2623-103">keyStringValuePair resource type</span></span>

<span data-ttu-id="c2623-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2623-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2623-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2623-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2623-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2623-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2623-107">Значение типа "ключ — значение" со строковым ключом и строковым значением.</span><span class="sxs-lookup"><span data-stu-id="c2623-107">A key-value pair with a string key and a string value.</span></span>


<span data-ttu-id="c2623-108">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c2623-108">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c2623-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2623-109">Properties</span></span>
|<span data-ttu-id="c2623-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2623-110">Property</span></span>|<span data-ttu-id="c2623-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c2623-111">Type</span></span>|<span data-ttu-id="c2623-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c2623-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2623-113">key</span><span class="sxs-lookup"><span data-stu-id="c2623-113">key</span></span>|<span data-ttu-id="c2623-114">String</span><span class="sxs-lookup"><span data-stu-id="c2623-114">String</span></span>|<span data-ttu-id="c2623-115">Строковый ключ для типа "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="c2623-115">The string key of the key-value pair.</span></span> <span data-ttu-id="c2623-116">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c2623-116">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="c2623-117">value</span><span class="sxs-lookup"><span data-stu-id="c2623-117">value</span></span>|<span data-ttu-id="c2623-118">String</span><span class="sxs-lookup"><span data-stu-id="c2623-118">String</span></span>|<span data-ttu-id="c2623-119">Строковое значение для параметра "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="c2623-119">The string value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2623-120">Связи</span><span class="sxs-lookup"><span data-stu-id="c2623-120">Relationships</span></span>
<span data-ttu-id="c2623-121">Нет</span><span class="sxs-lookup"><span data-stu-id="c2623-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2623-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2623-122">JSON Representation</span></span>
<span data-ttu-id="c2623-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2623-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyStringValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyStringValuePair",
  "key": "String",
  "value": "String"
}
```



