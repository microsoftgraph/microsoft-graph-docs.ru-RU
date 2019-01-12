---
title: Тип ресурса auditProperty
description: Класс, содержащий свойства для свойства аудита.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bd251fa942d526b01abca4191f041eb5a76745e5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952267"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="c101a-103">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="c101a-103">auditProperty resource type</span></span>

> <span data-ttu-id="c101a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c101a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c101a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c101a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c101a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c101a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c101a-107">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="c101a-107">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="c101a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c101a-108">Properties</span></span>
|<span data-ttu-id="c101a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c101a-109">Property</span></span>|<span data-ttu-id="c101a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c101a-110">Type</span></span>|<span data-ttu-id="c101a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c101a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c101a-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c101a-112">displayName</span></span>|<span data-ttu-id="c101a-113">String</span><span class="sxs-lookup"><span data-stu-id="c101a-113">String</span></span>|<span data-ttu-id="c101a-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="c101a-114">Display name.</span></span>|
|<span data-ttu-id="c101a-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="c101a-115">oldValue</span></span>|<span data-ttu-id="c101a-116">String</span><span class="sxs-lookup"><span data-stu-id="c101a-116">String</span></span>|<span data-ttu-id="c101a-117">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="c101a-117">Old value.</span></span>|
|<span data-ttu-id="c101a-118">newValue</span><span class="sxs-lookup"><span data-stu-id="c101a-118">newValue</span></span>|<span data-ttu-id="c101a-119">String</span><span class="sxs-lookup"><span data-stu-id="c101a-119">String</span></span>|<span data-ttu-id="c101a-120">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="c101a-120">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c101a-121">Связи</span><span class="sxs-lookup"><span data-stu-id="c101a-121">Relationships</span></span>
<span data-ttu-id="c101a-122">Нет</span><span class="sxs-lookup"><span data-stu-id="c101a-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c101a-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c101a-123">JSON Representation</span></span>
<span data-ttu-id="c101a-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c101a-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```





