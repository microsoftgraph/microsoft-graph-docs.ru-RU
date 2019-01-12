---
title: Тип ресурса keyValuePair
description: Пара "ключ-значение" для хранения пользовательских настроек
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9d7b5551bf4ca3237c6a4fc08db51c8e08474c63
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957902"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="b26f3-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="b26f3-103">keyValuePair resource type</span></span>

> <span data-ttu-id="b26f3-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b26f3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b26f3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b26f3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b26f3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b26f3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b26f3-107">Пара "ключ-значение" для хранения пользовательских настроек</span><span class="sxs-lookup"><span data-stu-id="b26f3-107">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="b26f3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b26f3-108">Properties</span></span>
|<span data-ttu-id="b26f3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b26f3-109">Property</span></span>|<span data-ttu-id="b26f3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b26f3-110">Type</span></span>|<span data-ttu-id="b26f3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b26f3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b26f3-112">name</span><span class="sxs-lookup"><span data-stu-id="b26f3-112">name</span></span>|<span data-ttu-id="b26f3-113">Строка</span><span class="sxs-lookup"><span data-stu-id="b26f3-113">String</span></span>|<span data-ttu-id="b26f3-114">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="b26f3-114">Name for this key-value pair</span></span>|
|<span data-ttu-id="b26f3-115">value</span><span class="sxs-lookup"><span data-stu-id="b26f3-115">value</span></span>|<span data-ttu-id="b26f3-116">Строка</span><span class="sxs-lookup"><span data-stu-id="b26f3-116">String</span></span>|<span data-ttu-id="b26f3-117">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="b26f3-117">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="b26f3-118">Связи</span><span class="sxs-lookup"><span data-stu-id="b26f3-118">Relationships</span></span>
<span data-ttu-id="b26f3-119">Нет</span><span class="sxs-lookup"><span data-stu-id="b26f3-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b26f3-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b26f3-120">JSON Representation</span></span>
<span data-ttu-id="b26f3-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b26f3-121">Here is a JSON representation of the resource.</span></span>
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





