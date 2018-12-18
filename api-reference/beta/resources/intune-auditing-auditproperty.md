---
title: Тип ресурса auditProperty
description: Класс, содержащий свойства для свойства аудита.
author: tfitzmac
ms.openlocfilehash: 801ac78cb81e126ff49c4c680fc0624611a9f6d6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316319"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="fd824-103">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="fd824-103">auditProperty resource type</span></span>

> <span data-ttu-id="fd824-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fd824-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd824-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd824-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fd824-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fd824-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd824-107">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="fd824-107">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="fd824-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fd824-108">Properties</span></span>
|<span data-ttu-id="fd824-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd824-109">Property</span></span>|<span data-ttu-id="fd824-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fd824-110">Type</span></span>|<span data-ttu-id="fd824-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fd824-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd824-112">displayName</span><span class="sxs-lookup"><span data-stu-id="fd824-112">displayName</span></span>|<span data-ttu-id="fd824-113">String</span><span class="sxs-lookup"><span data-stu-id="fd824-113">String</span></span>|<span data-ttu-id="fd824-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="fd824-114">Display name.</span></span>|
|<span data-ttu-id="fd824-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="fd824-115">oldValue</span></span>|<span data-ttu-id="fd824-116">String</span><span class="sxs-lookup"><span data-stu-id="fd824-116">String</span></span>|<span data-ttu-id="fd824-117">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="fd824-117">Old value.</span></span>|
|<span data-ttu-id="fd824-118">newValue</span><span class="sxs-lookup"><span data-stu-id="fd824-118">newValue</span></span>|<span data-ttu-id="fd824-119">String</span><span class="sxs-lookup"><span data-stu-id="fd824-119">String</span></span>|<span data-ttu-id="fd824-120">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="fd824-120">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd824-121">Связи</span><span class="sxs-lookup"><span data-stu-id="fd824-121">Relationships</span></span>
<span data-ttu-id="fd824-122">Нет</span><span class="sxs-lookup"><span data-stu-id="fd824-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fd824-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fd824-123">JSON Representation</span></span>
<span data-ttu-id="fd824-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd824-124">Here is a JSON representation of the resource.</span></span>
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





