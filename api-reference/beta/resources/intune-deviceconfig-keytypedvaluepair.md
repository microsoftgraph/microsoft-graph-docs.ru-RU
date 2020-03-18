---
title: Тип ресурса Кэйтипедвалуепаир
description: Значение типа "ключ — значение" со строковым ключом и типизированным значением.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f46ea5712c6ab96a4e3678d329e9e2f6cc283fc1
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790400"
---
# <a name="keytypedvaluepair-resource-type"></a><span data-ttu-id="3b3bf-103">Тип ресурса Кэйтипедвалуепаир</span><span class="sxs-lookup"><span data-stu-id="3b3bf-103">keyTypedValuePair resource type</span></span>

> <span data-ttu-id="3b3bf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b3bf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b3bf-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3b3bf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b3bf-106">Значение типа "ключ — значение" со строковым ключом и типизированным значением.</span><span class="sxs-lookup"><span data-stu-id="3b3bf-106">A key-value pair with a string key and a typed value.</span></span>

## <a name="properties"></a><span data-ttu-id="3b3bf-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3b3bf-107">Properties</span></span>
|<span data-ttu-id="3b3bf-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b3bf-108">Property</span></span>|<span data-ttu-id="3b3bf-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3b3bf-109">Type</span></span>|<span data-ttu-id="3b3bf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3b3bf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b3bf-111">key</span><span class="sxs-lookup"><span data-stu-id="3b3bf-111">key</span></span>|<span data-ttu-id="3b3bf-112">String</span><span class="sxs-lookup"><span data-stu-id="3b3bf-112">String</span></span>|<span data-ttu-id="3b3bf-113">Строковый ключ для типа "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="3b3bf-113">The string key of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b3bf-114">Связи</span><span class="sxs-lookup"><span data-stu-id="3b3bf-114">Relationships</span></span>
<span data-ttu-id="3b3bf-115">Нет</span><span class="sxs-lookup"><span data-stu-id="3b3bf-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b3bf-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3b3bf-116">JSON Representation</span></span>
<span data-ttu-id="3b3bf-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b3bf-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyTypedValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyTypedValuePair",
  "key": "String"
}
```



