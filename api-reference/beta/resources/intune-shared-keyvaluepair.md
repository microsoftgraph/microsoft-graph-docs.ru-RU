---
title: Тип ресурса keyValuePair
description: Пара "ключ-значение" для хранения пользовательских настроек
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 056dbe1f8504a89e3551402de7aa7ff7bc0ce866
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858445"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="293f5-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="293f5-103">keyValuePair resource type</span></span>

> <span data-ttu-id="293f5-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="293f5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="293f5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="293f5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="293f5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="293f5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="293f5-107">Пара "ключ-значение" для хранения пользовательских настроек</span><span class="sxs-lookup"><span data-stu-id="293f5-107">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="293f5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="293f5-108">Properties</span></span>
|<span data-ttu-id="293f5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="293f5-109">Property</span></span>|<span data-ttu-id="293f5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="293f5-110">Type</span></span>|<span data-ttu-id="293f5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="293f5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="293f5-112">name</span><span class="sxs-lookup"><span data-stu-id="293f5-112">name</span></span>|<span data-ttu-id="293f5-113">Строка</span><span class="sxs-lookup"><span data-stu-id="293f5-113">String</span></span>|<span data-ttu-id="293f5-114">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="293f5-114">Name for this key-value pair</span></span>|
|<span data-ttu-id="293f5-115">value</span><span class="sxs-lookup"><span data-stu-id="293f5-115">value</span></span>|<span data-ttu-id="293f5-116">Строка</span><span class="sxs-lookup"><span data-stu-id="293f5-116">String</span></span>|<span data-ttu-id="293f5-117">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="293f5-117">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="293f5-118">Связи</span><span class="sxs-lookup"><span data-stu-id="293f5-118">Relationships</span></span>
<span data-ttu-id="293f5-119">Нет</span><span class="sxs-lookup"><span data-stu-id="293f5-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="293f5-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="293f5-120">JSON Representation</span></span>
<span data-ttu-id="293f5-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="293f5-121">Here is a JSON representation of the resource.</span></span>
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





