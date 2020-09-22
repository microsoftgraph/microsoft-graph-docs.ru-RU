---
title: Тип ресурса Кэйбулеанвалуепаир
description: Значение типа "ключ — значение" с ключом строки и логическим значением.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e8eca8623277e6951e34d7ad627d4bfd193b4b4a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092554"
---
# <a name="keybooleanvaluepair-resource-type"></a><span data-ttu-id="088f8-103">Тип ресурса Кэйбулеанвалуепаир</span><span class="sxs-lookup"><span data-stu-id="088f8-103">keyBooleanValuePair resource type</span></span>

<span data-ttu-id="088f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="088f8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="088f8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="088f8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="088f8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="088f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="088f8-107">Значение типа "ключ — значение" с ключом строки и логическим значением.</span><span class="sxs-lookup"><span data-stu-id="088f8-107">A key-value pair with a string key and a Boolean value.</span></span>


<span data-ttu-id="088f8-108">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="088f8-108">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="088f8-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="088f8-109">Properties</span></span>
|<span data-ttu-id="088f8-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="088f8-110">Property</span></span>|<span data-ttu-id="088f8-111">Тип</span><span class="sxs-lookup"><span data-stu-id="088f8-111">Type</span></span>|<span data-ttu-id="088f8-112">Описание</span><span class="sxs-lookup"><span data-stu-id="088f8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="088f8-113">key</span><span class="sxs-lookup"><span data-stu-id="088f8-113">key</span></span>|<span data-ttu-id="088f8-114">Строка</span><span class="sxs-lookup"><span data-stu-id="088f8-114">String</span></span>|<span data-ttu-id="088f8-115">Строковый ключ для типа "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="088f8-115">The string key of the key-value pair.</span></span> <span data-ttu-id="088f8-116">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="088f8-116">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="088f8-117">value</span><span class="sxs-lookup"><span data-stu-id="088f8-117">value</span></span>|<span data-ttu-id="088f8-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="088f8-118">Boolean</span></span>|<span data-ttu-id="088f8-119">Логическое значение для параметра "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="088f8-119">The Boolean value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="088f8-120">Связи</span><span class="sxs-lookup"><span data-stu-id="088f8-120">Relationships</span></span>
<span data-ttu-id="088f8-121">Нет</span><span class="sxs-lookup"><span data-stu-id="088f8-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="088f8-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="088f8-122">JSON Representation</span></span>
<span data-ttu-id="088f8-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="088f8-123">Here is a JSON representation of the resource.</span></span>
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






