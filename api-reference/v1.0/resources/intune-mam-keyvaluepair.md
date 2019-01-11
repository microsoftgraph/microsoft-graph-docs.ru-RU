---
title: Тип ресурса keyValuePair
description: Пара "ключ-значение" для хранения пользовательских настроек
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 44f1765fb4f03a287665fe4ed1faef7012a43459
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805896"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="ac581-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="ac581-103">keyValuePair resource type</span></span>

> <span data-ttu-id="ac581-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ac581-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ac581-105">Пара "ключ-значение" для хранения пользовательских настроек</span><span class="sxs-lookup"><span data-stu-id="ac581-105">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="ac581-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ac581-106">Properties</span></span>
|<span data-ttu-id="ac581-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac581-107">Property</span></span>|<span data-ttu-id="ac581-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ac581-108">Type</span></span>|<span data-ttu-id="ac581-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ac581-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac581-110">name</span><span class="sxs-lookup"><span data-stu-id="ac581-110">name</span></span>|<span data-ttu-id="ac581-111">Строка</span><span class="sxs-lookup"><span data-stu-id="ac581-111">String</span></span>|<span data-ttu-id="ac581-112">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="ac581-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="ac581-113">value</span><span class="sxs-lookup"><span data-stu-id="ac581-113">value</span></span>|<span data-ttu-id="ac581-114">Строка</span><span class="sxs-lookup"><span data-stu-id="ac581-114">String</span></span>|<span data-ttu-id="ac581-115">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="ac581-115">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac581-116">Связи</span><span class="sxs-lookup"><span data-stu-id="ac581-116">Relationships</span></span>
<span data-ttu-id="ac581-117">Нет</span><span class="sxs-lookup"><span data-stu-id="ac581-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ac581-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ac581-118">JSON Representation</span></span>
<span data-ttu-id="ac581-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac581-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```



