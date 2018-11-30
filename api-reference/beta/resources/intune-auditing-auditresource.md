---
title: Тип ресурса auditResource
description: Класс, содержащий свойства ресурса аудита.
ms.openlocfilehash: a3825418c1406bbe9fcce7feeba96217342c735e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080408"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="e2bb7-103">Тип ресурса auditResource</span><span class="sxs-lookup"><span data-stu-id="e2bb7-103">auditResource resource type</span></span>

> <span data-ttu-id="e2bb7-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e2bb7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2bb7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2bb7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2bb7-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e2bb7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2bb7-107">Класс, содержащий свойства ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="e2bb7-107">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="e2bb7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e2bb7-108">Properties</span></span>
|<span data-ttu-id="e2bb7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2bb7-109">Property</span></span>|<span data-ttu-id="e2bb7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e2bb7-110">Type</span></span>|<span data-ttu-id="e2bb7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e2bb7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2bb7-112">displayName</span><span class="sxs-lookup"><span data-stu-id="e2bb7-112">displayName</span></span>|<span data-ttu-id="e2bb7-113">String</span><span class="sxs-lookup"><span data-stu-id="e2bb7-113">String</span></span>|<span data-ttu-id="e2bb7-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="e2bb7-114">Display name.</span></span>|
|<span data-ttu-id="e2bb7-115">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="e2bb7-115">modifiedProperties</span></span>|<span data-ttu-id="e2bb7-116">Коллекция [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="e2bb7-116">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="e2bb7-117">Список измененных свойств.</span><span class="sxs-lookup"><span data-stu-id="e2bb7-117">List of modified properties.</span></span>|
|<span data-ttu-id="e2bb7-118">type</span><span class="sxs-lookup"><span data-stu-id="e2bb7-118">type</span></span>|<span data-ttu-id="e2bb7-119">String</span><span class="sxs-lookup"><span data-stu-id="e2bb7-119">String</span></span>|<span data-ttu-id="e2bb7-120">Тип ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="e2bb7-120">Audit resource's type.</span></span>|
|<span data-ttu-id="e2bb7-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="e2bb7-121">resourceId</span></span>|<span data-ttu-id="e2bb7-122">String</span><span class="sxs-lookup"><span data-stu-id="e2bb7-122">String</span></span>|<span data-ttu-id="e2bb7-123">ИД ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="e2bb7-123">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2bb7-124">Связи</span><span class="sxs-lookup"><span data-stu-id="e2bb7-124">Relationships</span></span>
<span data-ttu-id="e2bb7-125">Нет</span><span class="sxs-lookup"><span data-stu-id="e2bb7-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e2bb7-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e2bb7-126">JSON Representation</span></span>
<span data-ttu-id="e2bb7-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2bb7-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.auditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```





