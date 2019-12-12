---
title: Тип ресурса Кэйбулеанвалуепаир
description: Значение типа "ключ — значение" с ключом строки и логическим значением.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6f4498f107e3153f6809ceb664c07b3f53a8d8e0
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955647"
---
# <a name="keybooleanvaluepair-resource-type"></a><span data-ttu-id="b3ee8-103">Тип ресурса Кэйбулеанвалуепаир</span><span class="sxs-lookup"><span data-stu-id="b3ee8-103">keyBooleanValuePair resource type</span></span>

> <span data-ttu-id="b3ee8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3ee8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3ee8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b3ee8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3ee8-106">Значение типа "ключ — значение" с ключом строки и логическим значением.</span><span class="sxs-lookup"><span data-stu-id="b3ee8-106">A key-value pair with a string key and a Boolean value.</span></span>


<span data-ttu-id="b3ee8-107">Наследуется от [кэйтипедвалуепаир](../resources/intune-shared-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b3ee8-107">Inherits from [keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b3ee8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b3ee8-108">Properties</span></span>
|<span data-ttu-id="b3ee8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3ee8-109">Property</span></span>|<span data-ttu-id="b3ee8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b3ee8-110">Type</span></span>|<span data-ttu-id="b3ee8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b3ee8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3ee8-112">key</span><span class="sxs-lookup"><span data-stu-id="b3ee8-112">key</span></span>|<span data-ttu-id="b3ee8-113">Строка</span><span class="sxs-lookup"><span data-stu-id="b3ee8-113">String</span></span>|<span data-ttu-id="b3ee8-114">Строковый ключ для типа "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="b3ee8-114">The string key of the key-value pair.</span></span> <span data-ttu-id="b3ee8-115">Наследуется от [кэйтипедвалуепаир](../resources/intune-shared-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b3ee8-115">Inherited from [keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="b3ee8-116">value</span><span class="sxs-lookup"><span data-stu-id="b3ee8-116">value</span></span>|<span data-ttu-id="b3ee8-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3ee8-117">Boolean</span></span>|<span data-ttu-id="b3ee8-118">Логическое значение для параметра "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="b3ee8-118">The Boolean value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3ee8-119">Связи</span><span class="sxs-lookup"><span data-stu-id="b3ee8-119">Relationships</span></span>
<span data-ttu-id="b3ee8-120">Нет</span><span class="sxs-lookup"><span data-stu-id="b3ee8-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3ee8-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b3ee8-121">JSON Representation</span></span>
<span data-ttu-id="b3ee8-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3ee8-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyBooleanValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyBooleanValuePair",
  "key": "String",
  "value": true
}
```



