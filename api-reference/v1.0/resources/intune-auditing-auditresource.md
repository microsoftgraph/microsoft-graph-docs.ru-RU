---
title: Тип ресурса auditResource
description: Класс, содержащий свойства ресурса аудита.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7f8fc3a96b3d17759e1e65eaa17c6571e4cec347
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844739"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="03800-103">Тип ресурса auditResource</span><span class="sxs-lookup"><span data-stu-id="03800-103">auditResource resource type</span></span>

> <span data-ttu-id="03800-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="03800-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03800-105">Класс, содержащий свойства ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="03800-105">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="03800-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="03800-106">Properties</span></span>
|<span data-ttu-id="03800-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="03800-107">Property</span></span>|<span data-ttu-id="03800-108">Тип</span><span class="sxs-lookup"><span data-stu-id="03800-108">Type</span></span>|<span data-ttu-id="03800-109">Описание</span><span class="sxs-lookup"><span data-stu-id="03800-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03800-110">displayName</span><span class="sxs-lookup"><span data-stu-id="03800-110">displayName</span></span>|<span data-ttu-id="03800-111">String</span><span class="sxs-lookup"><span data-stu-id="03800-111">String</span></span>|<span data-ttu-id="03800-112">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="03800-112">Display name.</span></span>|
|<span data-ttu-id="03800-113">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="03800-113">modifiedProperties</span></span>|<span data-ttu-id="03800-114">Коллекция [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="03800-114">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="03800-115">Список измененных свойств.</span><span class="sxs-lookup"><span data-stu-id="03800-115">List of modified properties.</span></span>|
|<span data-ttu-id="03800-116">type</span><span class="sxs-lookup"><span data-stu-id="03800-116">type</span></span>|<span data-ttu-id="03800-117">String</span><span class="sxs-lookup"><span data-stu-id="03800-117">String</span></span>|<span data-ttu-id="03800-118">Тип ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="03800-118">Audit resource's type.</span></span>|
|<span data-ttu-id="03800-119">resourceId</span><span class="sxs-lookup"><span data-stu-id="03800-119">resourceId</span></span>|<span data-ttu-id="03800-120">String</span><span class="sxs-lookup"><span data-stu-id="03800-120">String</span></span>|<span data-ttu-id="03800-121">ИД ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="03800-121">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03800-122">Связи</span><span class="sxs-lookup"><span data-stu-id="03800-122">Relationships</span></span>
<span data-ttu-id="03800-123">Нет</span><span class="sxs-lookup"><span data-stu-id="03800-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="03800-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="03800-124">JSON Representation</span></span>
<span data-ttu-id="03800-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03800-125">Here is a JSON representation of the resource.</span></span>
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



