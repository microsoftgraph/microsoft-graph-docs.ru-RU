---
title: Тип ресурса auditProperty
description: Класс, содержащий свойства для свойства аудита.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e91f3771be981f6ff410e8774f6a8ac9fbc121dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870919"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="e1717-103">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="e1717-103">auditProperty resource type</span></span>

> <span data-ttu-id="e1717-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e1717-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1717-105">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="e1717-105">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="e1717-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e1717-106">Properties</span></span>
|<span data-ttu-id="e1717-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1717-107">Property</span></span>|<span data-ttu-id="e1717-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e1717-108">Type</span></span>|<span data-ttu-id="e1717-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e1717-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1717-110">displayName</span><span class="sxs-lookup"><span data-stu-id="e1717-110">displayName</span></span>|<span data-ttu-id="e1717-111">String</span><span class="sxs-lookup"><span data-stu-id="e1717-111">String</span></span>|<span data-ttu-id="e1717-112">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="e1717-112">Display name.</span></span>|
|<span data-ttu-id="e1717-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="e1717-113">oldValue</span></span>|<span data-ttu-id="e1717-114">String</span><span class="sxs-lookup"><span data-stu-id="e1717-114">String</span></span>|<span data-ttu-id="e1717-115">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="e1717-115">Old value.</span></span>|
|<span data-ttu-id="e1717-116">newValue</span><span class="sxs-lookup"><span data-stu-id="e1717-116">newValue</span></span>|<span data-ttu-id="e1717-117">String</span><span class="sxs-lookup"><span data-stu-id="e1717-117">String</span></span>|<span data-ttu-id="e1717-118">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="e1717-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1717-119">Связи</span><span class="sxs-lookup"><span data-stu-id="e1717-119">Relationships</span></span>
<span data-ttu-id="e1717-120">Нет</span><span class="sxs-lookup"><span data-stu-id="e1717-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e1717-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e1717-121">JSON Representation</span></span>
<span data-ttu-id="e1717-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1717-122">Here is a JSON representation of the resource.</span></span>
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



