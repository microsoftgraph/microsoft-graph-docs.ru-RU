---
title: Тип ресурса Кэйинтежервалуепаир
description: Значение типа "ключ — значение" с ключом строки и целым значением.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 67a48f48f52c613c13552506d9cc76823bb042f7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439982"
---
# <a name="keyintegervaluepair-resource-type"></a><span data-ttu-id="43bb5-103">Тип ресурса Кэйинтежервалуепаир</span><span class="sxs-lookup"><span data-stu-id="43bb5-103">keyIntegerValuePair resource type</span></span>

<span data-ttu-id="43bb5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43bb5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43bb5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43bb5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43bb5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="43bb5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43bb5-107">Значение типа "ключ — значение" с ключом строки и целым значением.</span><span class="sxs-lookup"><span data-stu-id="43bb5-107">A key-value pair with a string key and an integer value.</span></span>


<span data-ttu-id="43bb5-108">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="43bb5-108">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="43bb5-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="43bb5-109">Properties</span></span>
|<span data-ttu-id="43bb5-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="43bb5-110">Property</span></span>|<span data-ttu-id="43bb5-111">Тип</span><span class="sxs-lookup"><span data-stu-id="43bb5-111">Type</span></span>|<span data-ttu-id="43bb5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="43bb5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43bb5-113">key</span><span class="sxs-lookup"><span data-stu-id="43bb5-113">key</span></span>|<span data-ttu-id="43bb5-114">String</span><span class="sxs-lookup"><span data-stu-id="43bb5-114">String</span></span>|<span data-ttu-id="43bb5-115">Строковый ключ для типа "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="43bb5-115">The string key of the key-value pair.</span></span> <span data-ttu-id="43bb5-116">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="43bb5-116">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="43bb5-117">value</span><span class="sxs-lookup"><span data-stu-id="43bb5-117">value</span></span>|<span data-ttu-id="43bb5-118">Int32</span><span class="sxs-lookup"><span data-stu-id="43bb5-118">Int32</span></span>|<span data-ttu-id="43bb5-119">Целочисленное значение для параметра "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="43bb5-119">The integer value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43bb5-120">Связи</span><span class="sxs-lookup"><span data-stu-id="43bb5-120">Relationships</span></span>
<span data-ttu-id="43bb5-121">Нет</span><span class="sxs-lookup"><span data-stu-id="43bb5-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="43bb5-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="43bb5-122">JSON Representation</span></span>
<span data-ttu-id="43bb5-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="43bb5-123">Here is a JSON representation of the resource.</span></span>
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



