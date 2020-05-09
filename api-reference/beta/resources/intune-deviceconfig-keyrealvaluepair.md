---
title: Тип ресурса Кэйреалвалуепаир
description: Значение типа "ключ-значение" с ключом строки и реальным значением (с плавающей запятой).
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1fed06ab52178805defae33fd5b51ce89235cec6
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44175667"
---
# <a name="keyrealvaluepair-resource-type"></a><span data-ttu-id="80ee3-103">Тип ресурса Кэйреалвалуепаир</span><span class="sxs-lookup"><span data-stu-id="80ee3-103">keyRealValuePair resource type</span></span>

<span data-ttu-id="80ee3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80ee3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="80ee3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80ee3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80ee3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="80ee3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80ee3-107">Значение типа "ключ-значение" с ключом строки и реальным значением (с плавающей запятой).</span><span class="sxs-lookup"><span data-stu-id="80ee3-107">A key-value pair with a string key and a real (floating-point) value.</span></span>


<span data-ttu-id="80ee3-108">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="80ee3-108">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="80ee3-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="80ee3-109">Properties</span></span>
|<span data-ttu-id="80ee3-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="80ee3-110">Property</span></span>|<span data-ttu-id="80ee3-111">Тип</span><span class="sxs-lookup"><span data-stu-id="80ee3-111">Type</span></span>|<span data-ttu-id="80ee3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="80ee3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80ee3-113">key</span><span class="sxs-lookup"><span data-stu-id="80ee3-113">key</span></span>|<span data-ttu-id="80ee3-114">Строка</span><span class="sxs-lookup"><span data-stu-id="80ee3-114">String</span></span>|<span data-ttu-id="80ee3-115">Строковый ключ для типа "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="80ee3-115">The string key of the key-value pair.</span></span> <span data-ttu-id="80ee3-116">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="80ee3-116">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="80ee3-117">значение</span><span class="sxs-lookup"><span data-stu-id="80ee3-117">value</span></span>|<span data-ttu-id="80ee3-118">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="80ee3-118">Double</span></span>|<span data-ttu-id="80ee3-119">Реальное значение (число с плавающей запятой) для каждой из них: "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="80ee3-119">The real (floating-point) value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80ee3-120">Связи</span><span class="sxs-lookup"><span data-stu-id="80ee3-120">Relationships</span></span>
<span data-ttu-id="80ee3-121">Нет</span><span class="sxs-lookup"><span data-stu-id="80ee3-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="80ee3-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="80ee3-122">JSON Representation</span></span>
<span data-ttu-id="80ee3-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="80ee3-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyRealValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyRealValuePair",
  "key": "String",
  "value": "4.2"
}
```



