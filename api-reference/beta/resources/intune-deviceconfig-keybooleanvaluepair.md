---
title: Тип ресурса Кэйбулеанвалуепаир
description: Значение типа "ключ — значение" с ключом строки и логическим значением.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: aabdb6e8eef4e41ec5c9aaf5d1a24fca97ae8c2e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526271"
---
# <a name="keybooleanvaluepair-resource-type"></a><span data-ttu-id="4d54b-103">Тип ресурса Кэйбулеанвалуепаир</span><span class="sxs-lookup"><span data-stu-id="4d54b-103">keyBooleanValuePair resource type</span></span>

<span data-ttu-id="4d54b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4d54b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4d54b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d54b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d54b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4d54b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d54b-107">Значение типа "ключ — значение" с ключом строки и логическим значением.</span><span class="sxs-lookup"><span data-stu-id="4d54b-107">A key-value pair with a string key and a Boolean value.</span></span>


<span data-ttu-id="4d54b-108">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="4d54b-108">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4d54b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4d54b-109">Properties</span></span>
|<span data-ttu-id="4d54b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d54b-110">Property</span></span>|<span data-ttu-id="4d54b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4d54b-111">Type</span></span>|<span data-ttu-id="4d54b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4d54b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d54b-113">key</span><span class="sxs-lookup"><span data-stu-id="4d54b-113">key</span></span>|<span data-ttu-id="4d54b-114">String</span><span class="sxs-lookup"><span data-stu-id="4d54b-114">String</span></span>|<span data-ttu-id="4d54b-115">Строковый ключ для типа "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="4d54b-115">The string key of the key-value pair.</span></span> <span data-ttu-id="4d54b-116">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="4d54b-116">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="4d54b-117">value</span><span class="sxs-lookup"><span data-stu-id="4d54b-117">value</span></span>|<span data-ttu-id="4d54b-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d54b-118">Boolean</span></span>|<span data-ttu-id="4d54b-119">Логическое значение для параметра "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="4d54b-119">The Boolean value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d54b-120">Связи</span><span class="sxs-lookup"><span data-stu-id="4d54b-120">Relationships</span></span>
<span data-ttu-id="4d54b-121">Нет</span><span class="sxs-lookup"><span data-stu-id="4d54b-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d54b-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4d54b-122">JSON Representation</span></span>
<span data-ttu-id="4d54b-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d54b-123">Here is a JSON representation of the resource.</span></span>
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



