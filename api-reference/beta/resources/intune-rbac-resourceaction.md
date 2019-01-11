---
title: Тип ресурса resourceAction
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8d607ca2b250e9d2af55b74ef568a82c522bf761
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876386"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="a2486-103">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="a2486-103">resourceAction resource type</span></span>

> <span data-ttu-id="a2486-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a2486-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2486-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2486-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a2486-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a2486-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2486-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a2486-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="a2486-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a2486-108">Properties</span></span>
|<span data-ttu-id="a2486-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2486-109">Property</span></span>|<span data-ttu-id="a2486-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a2486-110">Type</span></span>|<span data-ttu-id="a2486-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a2486-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2486-112">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="a2486-112">allowedResourceActions</span></span>|<span data-ttu-id="a2486-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a2486-113">String collection</span></span>|<span data-ttu-id="a2486-114">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="a2486-114">Allowed Actions</span></span>|
|<span data-ttu-id="a2486-115">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="a2486-115">notAllowedResourceActions</span></span>|<span data-ttu-id="a2486-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a2486-116">String collection</span></span>|<span data-ttu-id="a2486-117">Запрещенные действия</span><span class="sxs-lookup"><span data-stu-id="a2486-117">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2486-118">Связи</span><span class="sxs-lookup"><span data-stu-id="a2486-118">Relationships</span></span>
<span data-ttu-id="a2486-119">Нет</span><span class="sxs-lookup"><span data-stu-id="a2486-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a2486-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a2486-120">JSON Representation</span></span>
<span data-ttu-id="a2486-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2486-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```





