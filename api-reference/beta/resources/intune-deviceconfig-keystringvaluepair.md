---
title: Тип ресурса Кэйстрингвалуепаир
description: Значение типа "ключ — значение" со строковым ключом и строковым значением.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 029ebbe04532b729b49115fd51cdbcf4ea22a6a3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790407"
---
# <a name="keystringvaluepair-resource-type"></a><span data-ttu-id="81ba0-103">Тип ресурса Кэйстрингвалуепаир</span><span class="sxs-lookup"><span data-stu-id="81ba0-103">keyStringValuePair resource type</span></span>

> <span data-ttu-id="81ba0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81ba0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81ba0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="81ba0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81ba0-106">Значение типа "ключ — значение" со строковым ключом и строковым значением.</span><span class="sxs-lookup"><span data-stu-id="81ba0-106">A key-value pair with a string key and a string value.</span></span>


<span data-ttu-id="81ba0-107">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="81ba0-107">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="81ba0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="81ba0-108">Properties</span></span>
|<span data-ttu-id="81ba0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="81ba0-109">Property</span></span>|<span data-ttu-id="81ba0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="81ba0-110">Type</span></span>|<span data-ttu-id="81ba0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="81ba0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81ba0-112">key</span><span class="sxs-lookup"><span data-stu-id="81ba0-112">key</span></span>|<span data-ttu-id="81ba0-113">String</span><span class="sxs-lookup"><span data-stu-id="81ba0-113">String</span></span>|<span data-ttu-id="81ba0-114">Строковый ключ для типа "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="81ba0-114">The string key of the key-value pair.</span></span> <span data-ttu-id="81ba0-115">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="81ba0-115">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="81ba0-116">value</span><span class="sxs-lookup"><span data-stu-id="81ba0-116">value</span></span>|<span data-ttu-id="81ba0-117">String</span><span class="sxs-lookup"><span data-stu-id="81ba0-117">String</span></span>|<span data-ttu-id="81ba0-118">Строковое значение для параметра "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="81ba0-118">The string value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81ba0-119">Связи</span><span class="sxs-lookup"><span data-stu-id="81ba0-119">Relationships</span></span>
<span data-ttu-id="81ba0-120">Нет</span><span class="sxs-lookup"><span data-stu-id="81ba0-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81ba0-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="81ba0-121">JSON Representation</span></span>
<span data-ttu-id="81ba0-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81ba0-122">Here is a JSON representation of the resource.</span></span>
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



