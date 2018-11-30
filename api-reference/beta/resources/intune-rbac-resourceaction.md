---
title: Тип ресурса resourceAction
description: Н/Д
ms.openlocfilehash: d4f585ec52096cc9bd6d1430825d61426df644fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079234"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="998e3-103">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="998e3-103">resourceAction resource type</span></span>

> <span data-ttu-id="998e3-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="998e3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="998e3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="998e3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="998e3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="998e3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="998e3-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="998e3-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="998e3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="998e3-108">Properties</span></span>
|<span data-ttu-id="998e3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="998e3-109">Property</span></span>|<span data-ttu-id="998e3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="998e3-110">Type</span></span>|<span data-ttu-id="998e3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="998e3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="998e3-112">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="998e3-112">allowedResourceActions</span></span>|<span data-ttu-id="998e3-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="998e3-113">String collection</span></span>|<span data-ttu-id="998e3-114">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="998e3-114">Allowed Actions</span></span>|
|<span data-ttu-id="998e3-115">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="998e3-115">notAllowedResourceActions</span></span>|<span data-ttu-id="998e3-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="998e3-116">String collection</span></span>|<span data-ttu-id="998e3-117">Запрещенные действия</span><span class="sxs-lookup"><span data-stu-id="998e3-117">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="998e3-118">Связи</span><span class="sxs-lookup"><span data-stu-id="998e3-118">Relationships</span></span>
<span data-ttu-id="998e3-119">Нет</span><span class="sxs-lookup"><span data-stu-id="998e3-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="998e3-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="998e3-120">JSON Representation</span></span>
<span data-ttu-id="998e3-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="998e3-121">Here is a JSON representation of the resource.</span></span>
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





