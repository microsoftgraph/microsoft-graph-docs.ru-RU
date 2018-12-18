---
title: Тип ресурса keyValuePair
description: Пара "ключ-значение" для хранения пользовательских настроек
author: tfitzmac
ms.openlocfilehash: f6438d97376d46f66e02026acc87c948ab2a91bb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329318"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="e7dfc-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="e7dfc-103">keyValuePair resource type</span></span>

> <span data-ttu-id="e7dfc-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e7dfc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7dfc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7dfc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e7dfc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e7dfc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7dfc-107">Пара "ключ-значение" для хранения пользовательских настроек</span><span class="sxs-lookup"><span data-stu-id="e7dfc-107">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="e7dfc-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e7dfc-108">Properties</span></span>
|<span data-ttu-id="e7dfc-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7dfc-109">Property</span></span>|<span data-ttu-id="e7dfc-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e7dfc-110">Type</span></span>|<span data-ttu-id="e7dfc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e7dfc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7dfc-112">name</span><span class="sxs-lookup"><span data-stu-id="e7dfc-112">name</span></span>|<span data-ttu-id="e7dfc-113">Строка</span><span class="sxs-lookup"><span data-stu-id="e7dfc-113">String</span></span>|<span data-ttu-id="e7dfc-114">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="e7dfc-114">Name for this key-value pair</span></span>|
|<span data-ttu-id="e7dfc-115">value</span><span class="sxs-lookup"><span data-stu-id="e7dfc-115">value</span></span>|<span data-ttu-id="e7dfc-116">Строка</span><span class="sxs-lookup"><span data-stu-id="e7dfc-116">String</span></span>|<span data-ttu-id="e7dfc-117">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="e7dfc-117">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7dfc-118">Связи</span><span class="sxs-lookup"><span data-stu-id="e7dfc-118">Relationships</span></span>
<span data-ttu-id="e7dfc-119">Нет</span><span class="sxs-lookup"><span data-stu-id="e7dfc-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e7dfc-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e7dfc-120">JSON Representation</span></span>
<span data-ttu-id="e7dfc-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7dfc-121">Here is a JSON representation of the resource.</span></span>
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





