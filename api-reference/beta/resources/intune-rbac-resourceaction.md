---
title: Тип ресурса resourceAction
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 17d8bd52996ca9b129292c204dd498fcc5a65ac6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963243"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="c41c8-103">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="c41c8-103">resourceAction resource type</span></span>

> <span data-ttu-id="c41c8-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c41c8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c41c8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c41c8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c41c8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c41c8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c41c8-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c41c8-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c41c8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c41c8-108">Properties</span></span>
|<span data-ttu-id="c41c8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c41c8-109">Property</span></span>|<span data-ttu-id="c41c8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c41c8-110">Type</span></span>|<span data-ttu-id="c41c8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c41c8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c41c8-112">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="c41c8-112">allowedResourceActions</span></span>|<span data-ttu-id="c41c8-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c41c8-113">String collection</span></span>|<span data-ttu-id="c41c8-114">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="c41c8-114">Allowed Actions</span></span>|
|<span data-ttu-id="c41c8-115">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="c41c8-115">notAllowedResourceActions</span></span>|<span data-ttu-id="c41c8-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c41c8-116">String collection</span></span>|<span data-ttu-id="c41c8-117">Запрещенные действия</span><span class="sxs-lookup"><span data-stu-id="c41c8-117">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="c41c8-118">Связи</span><span class="sxs-lookup"><span data-stu-id="c41c8-118">Relationships</span></span>
<span data-ttu-id="c41c8-119">Нет</span><span class="sxs-lookup"><span data-stu-id="c41c8-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c41c8-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c41c8-120">JSON Representation</span></span>
<span data-ttu-id="c41c8-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c41c8-121">Here is a JSON representation of the resource.</span></span>
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





