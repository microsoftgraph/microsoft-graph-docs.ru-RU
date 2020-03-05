---
title: Тип ресурса Кэйинтежервалуепаир
description: Значение типа "ключ — значение" с ключом строки и целым значением.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d399c7b9b0dae17beb6928682e88460ba9999b16
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529797"
---
# <a name="keyintegervaluepair-resource-type"></a><span data-ttu-id="0aedf-103">Тип ресурса Кэйинтежервалуепаир</span><span class="sxs-lookup"><span data-stu-id="0aedf-103">keyIntegerValuePair resource type</span></span>

<span data-ttu-id="0aedf-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0aedf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0aedf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0aedf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0aedf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0aedf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0aedf-107">Значение типа "ключ — значение" с ключом строки и целым значением.</span><span class="sxs-lookup"><span data-stu-id="0aedf-107">A key-value pair with a string key and an integer value.</span></span>


<span data-ttu-id="0aedf-108">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="0aedf-108">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0aedf-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="0aedf-109">Properties</span></span>
|<span data-ttu-id="0aedf-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="0aedf-110">Property</span></span>|<span data-ttu-id="0aedf-111">Тип</span><span class="sxs-lookup"><span data-stu-id="0aedf-111">Type</span></span>|<span data-ttu-id="0aedf-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0aedf-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0aedf-113">key</span><span class="sxs-lookup"><span data-stu-id="0aedf-113">key</span></span>|<span data-ttu-id="0aedf-114">String</span><span class="sxs-lookup"><span data-stu-id="0aedf-114">String</span></span>|<span data-ttu-id="0aedf-115">Строковый ключ для типа "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="0aedf-115">The string key of the key-value pair.</span></span> <span data-ttu-id="0aedf-116">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="0aedf-116">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="0aedf-117">value</span><span class="sxs-lookup"><span data-stu-id="0aedf-117">value</span></span>|<span data-ttu-id="0aedf-118">Int32</span><span class="sxs-lookup"><span data-stu-id="0aedf-118">Int32</span></span>|<span data-ttu-id="0aedf-119">Целочисленное значение для параметра "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="0aedf-119">The integer value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0aedf-120">Связи</span><span class="sxs-lookup"><span data-stu-id="0aedf-120">Relationships</span></span>
<span data-ttu-id="0aedf-121">Нет</span><span class="sxs-lookup"><span data-stu-id="0aedf-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0aedf-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0aedf-122">JSON Representation</span></span>
<span data-ttu-id="0aedf-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0aedf-123">Here is a JSON representation of the resource.</span></span>
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



