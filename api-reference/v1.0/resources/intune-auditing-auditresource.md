---
title: Тип ресурса auditResource
description: Класс, содержащий свойства ресурса аудита.
author: tfitzmac
ms.openlocfilehash: 5cfc23a80b2247b9f561d802ce844091c623ef62
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302662"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="c2c5a-103">Тип ресурса auditResource</span><span class="sxs-lookup"><span data-stu-id="c2c5a-103">auditResource resource type</span></span>

> <span data-ttu-id="c2c5a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c2c5a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c2c5a-105">Класс, содержащий свойства ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="c2c5a-105">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="c2c5a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2c5a-106">Properties</span></span>
|<span data-ttu-id="c2c5a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2c5a-107">Property</span></span>|<span data-ttu-id="c2c5a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c2c5a-108">Type</span></span>|<span data-ttu-id="c2c5a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c2c5a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2c5a-110">displayName</span><span class="sxs-lookup"><span data-stu-id="c2c5a-110">displayName</span></span>|<span data-ttu-id="c2c5a-111">String</span><span class="sxs-lookup"><span data-stu-id="c2c5a-111">String</span></span>|<span data-ttu-id="c2c5a-112">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="c2c5a-112">Display name.</span></span>|
|<span data-ttu-id="c2c5a-113">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="c2c5a-113">modifiedProperties</span></span>|<span data-ttu-id="c2c5a-114">Коллекция [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="c2c5a-114">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="c2c5a-115">Список измененных свойств.</span><span class="sxs-lookup"><span data-stu-id="c2c5a-115">List of modified properties.</span></span>|
|<span data-ttu-id="c2c5a-116">type</span><span class="sxs-lookup"><span data-stu-id="c2c5a-116">type</span></span>|<span data-ttu-id="c2c5a-117">String</span><span class="sxs-lookup"><span data-stu-id="c2c5a-117">String</span></span>|<span data-ttu-id="c2c5a-118">Тип ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="c2c5a-118">Audit resource's type.</span></span>|
|<span data-ttu-id="c2c5a-119">resourceId</span><span class="sxs-lookup"><span data-stu-id="c2c5a-119">resourceId</span></span>|<span data-ttu-id="c2c5a-120">String</span><span class="sxs-lookup"><span data-stu-id="c2c5a-120">String</span></span>|<span data-ttu-id="c2c5a-121">ИД ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="c2c5a-121">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2c5a-122">Связи</span><span class="sxs-lookup"><span data-stu-id="c2c5a-122">Relationships</span></span>
<span data-ttu-id="c2c5a-123">Нет</span><span class="sxs-lookup"><span data-stu-id="c2c5a-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c2c5a-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2c5a-124">JSON Representation</span></span>
<span data-ttu-id="c2c5a-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2c5a-125">Here is a JSON representation of the resource.</span></span>
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



