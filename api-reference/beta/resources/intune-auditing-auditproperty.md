---
title: Тип ресурса auditProperty
description: Класс, содержащий свойства для свойства аудита.
ms.openlocfilehash: 944928014eee2e47ee0478053196bfbc1a999fc2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078233"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="15890-103">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="15890-103">auditProperty resource type</span></span>

> <span data-ttu-id="15890-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="15890-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15890-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15890-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15890-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="15890-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15890-107">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="15890-107">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="15890-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="15890-108">Properties</span></span>
|<span data-ttu-id="15890-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="15890-109">Property</span></span>|<span data-ttu-id="15890-110">Тип</span><span class="sxs-lookup"><span data-stu-id="15890-110">Type</span></span>|<span data-ttu-id="15890-111">Описание</span><span class="sxs-lookup"><span data-stu-id="15890-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15890-112">displayName</span><span class="sxs-lookup"><span data-stu-id="15890-112">displayName</span></span>|<span data-ttu-id="15890-113">String</span><span class="sxs-lookup"><span data-stu-id="15890-113">String</span></span>|<span data-ttu-id="15890-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="15890-114">Display name.</span></span>|
|<span data-ttu-id="15890-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="15890-115">oldValue</span></span>|<span data-ttu-id="15890-116">String</span><span class="sxs-lookup"><span data-stu-id="15890-116">String</span></span>|<span data-ttu-id="15890-117">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="15890-117">Old value.</span></span>|
|<span data-ttu-id="15890-118">newValue</span><span class="sxs-lookup"><span data-stu-id="15890-118">newValue</span></span>|<span data-ttu-id="15890-119">String</span><span class="sxs-lookup"><span data-stu-id="15890-119">String</span></span>|<span data-ttu-id="15890-120">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="15890-120">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15890-121">Связи</span><span class="sxs-lookup"><span data-stu-id="15890-121">Relationships</span></span>
<span data-ttu-id="15890-122">Нет</span><span class="sxs-lookup"><span data-stu-id="15890-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="15890-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="15890-123">JSON Representation</span></span>
<span data-ttu-id="15890-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15890-124">Here is a JSON representation of the resource.</span></span>
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





