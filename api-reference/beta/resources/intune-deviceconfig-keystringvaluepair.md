---
title: Тип ресурса Кэйстрингвалуепаир
description: Значение типа "ключ — значение" со строковым ключом и строковым значением.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0bb9d540f098c88065d7d12536b3a2be73af7e93
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201305"
---
# <a name="keystringvaluepair-resource-type"></a><span data-ttu-id="2e3d1-103">Тип ресурса Кэйстрингвалуепаир</span><span class="sxs-lookup"><span data-stu-id="2e3d1-103">keyStringValuePair resource type</span></span>

> <span data-ttu-id="2e3d1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e3d1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e3d1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e3d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e3d1-106">Значение типа "ключ — значение" со строковым ключом и строковым значением.</span><span class="sxs-lookup"><span data-stu-id="2e3d1-106">A key-value pair with a string key and a string value.</span></span>


<span data-ttu-id="2e3d1-107">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="2e3d1-107">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2e3d1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e3d1-108">Properties</span></span>
|<span data-ttu-id="2e3d1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e3d1-109">Property</span></span>|<span data-ttu-id="2e3d1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2e3d1-110">Type</span></span>|<span data-ttu-id="2e3d1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2e3d1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e3d1-112">key</span><span class="sxs-lookup"><span data-stu-id="2e3d1-112">key</span></span>|<span data-ttu-id="2e3d1-113">String.</span><span class="sxs-lookup"><span data-stu-id="2e3d1-113">String</span></span>|<span data-ttu-id="2e3d1-114">Строковый ключ для типа "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="2e3d1-114">The string key of the key-value pair.</span></span> <span data-ttu-id="2e3d1-115">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="2e3d1-115">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="2e3d1-116">value</span><span class="sxs-lookup"><span data-stu-id="2e3d1-116">value</span></span>|<span data-ttu-id="2e3d1-117">String</span><span class="sxs-lookup"><span data-stu-id="2e3d1-117">String</span></span>|<span data-ttu-id="2e3d1-118">Строковое значение для параметра "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="2e3d1-118">The string value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e3d1-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="2e3d1-119">Relationships</span></span>
<span data-ttu-id="2e3d1-120">Нет</span><span class="sxs-lookup"><span data-stu-id="2e3d1-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e3d1-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2e3d1-121">JSON Representation</span></span>
<span data-ttu-id="2e3d1-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e3d1-122">Here is a JSON representation of the resource.</span></span>
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



