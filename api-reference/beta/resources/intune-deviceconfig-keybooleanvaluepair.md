---
title: Тип ресурса Кэйбулеанвалуепаир
description: Значение типа "ключ — значение" с ключом строки и логическим значением.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c525c1880c8a77dd8bf29c1ee5c8fb2864ab928b
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201310"
---
# <a name="keybooleanvaluepair-resource-type"></a><span data-ttu-id="4442a-103">Тип ресурса Кэйбулеанвалуепаир</span><span class="sxs-lookup"><span data-stu-id="4442a-103">keyBooleanValuePair resource type</span></span>

> <span data-ttu-id="4442a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4442a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4442a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4442a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4442a-106">Значение типа "ключ — значение" с ключом строки и логическим значением.</span><span class="sxs-lookup"><span data-stu-id="4442a-106">A key-value pair with a string key and a Boolean value.</span></span>


<span data-ttu-id="4442a-107">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="4442a-107">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4442a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4442a-108">Properties</span></span>
|<span data-ttu-id="4442a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4442a-109">Property</span></span>|<span data-ttu-id="4442a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4442a-110">Type</span></span>|<span data-ttu-id="4442a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4442a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4442a-112">key</span><span class="sxs-lookup"><span data-stu-id="4442a-112">key</span></span>|<span data-ttu-id="4442a-113">String.</span><span class="sxs-lookup"><span data-stu-id="4442a-113">String</span></span>|<span data-ttu-id="4442a-114">Строковый ключ для типа "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="4442a-114">The string key of the key-value pair.</span></span> <span data-ttu-id="4442a-115">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="4442a-115">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="4442a-116">value</span><span class="sxs-lookup"><span data-stu-id="4442a-116">value</span></span>|<span data-ttu-id="4442a-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="4442a-117">Boolean</span></span>|<span data-ttu-id="4442a-118">Логическое значение для параметра "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="4442a-118">The Boolean value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4442a-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="4442a-119">Relationships</span></span>
<span data-ttu-id="4442a-120">Нет</span><span class="sxs-lookup"><span data-stu-id="4442a-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4442a-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4442a-121">JSON Representation</span></span>
<span data-ttu-id="4442a-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4442a-122">Here is a JSON representation of the resource.</span></span>
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



