---
title: Тип ресурса auditProperty
description: Класс, содержащий свойства для свойства аудита.
author: tfitzmac
ms.openlocfilehash: 2d7cd7f1fbbf9f813cf447ca53e0d4652eb0feda
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312903"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="02eb5-103">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="02eb5-103">auditProperty resource type</span></span>

> <span data-ttu-id="02eb5-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="02eb5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="02eb5-105">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="02eb5-105">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="02eb5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="02eb5-106">Properties</span></span>
|<span data-ttu-id="02eb5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="02eb5-107">Property</span></span>|<span data-ttu-id="02eb5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="02eb5-108">Type</span></span>|<span data-ttu-id="02eb5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="02eb5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02eb5-110">displayName</span><span class="sxs-lookup"><span data-stu-id="02eb5-110">displayName</span></span>|<span data-ttu-id="02eb5-111">String</span><span class="sxs-lookup"><span data-stu-id="02eb5-111">String</span></span>|<span data-ttu-id="02eb5-112">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="02eb5-112">Display name.</span></span>|
|<span data-ttu-id="02eb5-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="02eb5-113">oldValue</span></span>|<span data-ttu-id="02eb5-114">String</span><span class="sxs-lookup"><span data-stu-id="02eb5-114">String</span></span>|<span data-ttu-id="02eb5-115">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="02eb5-115">Old value.</span></span>|
|<span data-ttu-id="02eb5-116">newValue</span><span class="sxs-lookup"><span data-stu-id="02eb5-116">newValue</span></span>|<span data-ttu-id="02eb5-117">String</span><span class="sxs-lookup"><span data-stu-id="02eb5-117">String</span></span>|<span data-ttu-id="02eb5-118">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="02eb5-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02eb5-119">Связи</span><span class="sxs-lookup"><span data-stu-id="02eb5-119">Relationships</span></span>
<span data-ttu-id="02eb5-120">Нет</span><span class="sxs-lookup"><span data-stu-id="02eb5-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="02eb5-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="02eb5-121">JSON Representation</span></span>
<span data-ttu-id="02eb5-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02eb5-122">Here is a JSON representation of the resource.</span></span>
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



