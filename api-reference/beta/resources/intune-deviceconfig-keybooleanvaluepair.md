---
title: Тип ресурса Кэйбулеанвалуепаир
description: Значение типа "ключ — значение" с ключом строки и логическим значением.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 20362eadb79f94fab1d7fc7c454995710a0ab9ab
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439989"
---
# <a name="keybooleanvaluepair-resource-type"></a><span data-ttu-id="c9426-103">Тип ресурса Кэйбулеанвалуепаир</span><span class="sxs-lookup"><span data-stu-id="c9426-103">keyBooleanValuePair resource type</span></span>

<span data-ttu-id="c9426-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9426-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c9426-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9426-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9426-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c9426-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9426-107">Значение типа "ключ — значение" с ключом строки и логическим значением.</span><span class="sxs-lookup"><span data-stu-id="c9426-107">A key-value pair with a string key and a Boolean value.</span></span>


<span data-ttu-id="c9426-108">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c9426-108">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c9426-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c9426-109">Properties</span></span>
|<span data-ttu-id="c9426-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9426-110">Property</span></span>|<span data-ttu-id="c9426-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c9426-111">Type</span></span>|<span data-ttu-id="c9426-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c9426-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9426-113">key</span><span class="sxs-lookup"><span data-stu-id="c9426-113">key</span></span>|<span data-ttu-id="c9426-114">String</span><span class="sxs-lookup"><span data-stu-id="c9426-114">String</span></span>|<span data-ttu-id="c9426-115">Строковый ключ для типа "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="c9426-115">The string key of the key-value pair.</span></span> <span data-ttu-id="c9426-116">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c9426-116">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="c9426-117">value</span><span class="sxs-lookup"><span data-stu-id="c9426-117">value</span></span>|<span data-ttu-id="c9426-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9426-118">Boolean</span></span>|<span data-ttu-id="c9426-119">Логическое значение для параметра "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="c9426-119">The Boolean value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9426-120">Связи</span><span class="sxs-lookup"><span data-stu-id="c9426-120">Relationships</span></span>
<span data-ttu-id="c9426-121">Нет</span><span class="sxs-lookup"><span data-stu-id="c9426-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9426-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c9426-122">JSON Representation</span></span>
<span data-ttu-id="c9426-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9426-123">Here is a JSON representation of the resource.</span></span>
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



