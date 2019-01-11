---
title: Тип ресурса keyValue
description: Определение значения ключа.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: aae0fea85c5dd4f647a72c0fe66890bd8b82520b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885017"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="85e7a-103">Тип ресурса keyValue</span><span class="sxs-lookup"><span data-stu-id="85e7a-103">keyValue resource type</span></span>

> <span data-ttu-id="85e7a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="85e7a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85e7a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85e7a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85e7a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="85e7a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85e7a-107">Определение значения ключа.</span><span class="sxs-lookup"><span data-stu-id="85e7a-107">Key Value definition.</span></span>
## <a name="properties"></a><span data-ttu-id="85e7a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="85e7a-108">Properties</span></span>
|<span data-ttu-id="85e7a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="85e7a-109">Property</span></span>|<span data-ttu-id="85e7a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="85e7a-110">Type</span></span>|<span data-ttu-id="85e7a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="85e7a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85e7a-112">key</span><span class="sxs-lookup"><span data-stu-id="85e7a-112">key</span></span>|<span data-ttu-id="85e7a-113">Строка</span><span class="sxs-lookup"><span data-stu-id="85e7a-113">String</span></span>|<span data-ttu-id="85e7a-114">Ключ.</span><span class="sxs-lookup"><span data-stu-id="85e7a-114">Key.</span></span>|
|<span data-ttu-id="85e7a-115">value</span><span class="sxs-lookup"><span data-stu-id="85e7a-115">value</span></span>|<span data-ttu-id="85e7a-116">Строка</span><span class="sxs-lookup"><span data-stu-id="85e7a-116">String</span></span>|<span data-ttu-id="85e7a-117">Значение</span><span class="sxs-lookup"><span data-stu-id="85e7a-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85e7a-118">Связи</span><span class="sxs-lookup"><span data-stu-id="85e7a-118">Relationships</span></span>
<span data-ttu-id="85e7a-119">Нет</span><span class="sxs-lookup"><span data-stu-id="85e7a-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="85e7a-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="85e7a-120">JSON Representation</span></span>
<span data-ttu-id="85e7a-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85e7a-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValue",
  "key": "String",
  "value": "String"
}
```





