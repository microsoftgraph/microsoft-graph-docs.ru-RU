---
title: Тип ресурса auditProperty
description: Класс, содержащий свойства для свойства аудита.
ms.openlocfilehash: eaffa5552d611ac2ef8bb236009b9520d1134586
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027849"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="54206-103">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="54206-103">auditProperty resource type</span></span>

> <span data-ttu-id="54206-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="54206-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="54206-105">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="54206-105">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="54206-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="54206-106">Properties</span></span>
|<span data-ttu-id="54206-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="54206-107">Property</span></span>|<span data-ttu-id="54206-108">Тип</span><span class="sxs-lookup"><span data-stu-id="54206-108">Type</span></span>|<span data-ttu-id="54206-109">Описание</span><span class="sxs-lookup"><span data-stu-id="54206-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54206-110">displayName</span><span class="sxs-lookup"><span data-stu-id="54206-110">displayName</span></span>|<span data-ttu-id="54206-111">String</span><span class="sxs-lookup"><span data-stu-id="54206-111">String</span></span>|<span data-ttu-id="54206-112">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="54206-112">Display name.</span></span>|
|<span data-ttu-id="54206-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="54206-113">oldValue</span></span>|<span data-ttu-id="54206-114">String</span><span class="sxs-lookup"><span data-stu-id="54206-114">String</span></span>|<span data-ttu-id="54206-115">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="54206-115">Old value.</span></span>|
|<span data-ttu-id="54206-116">newValue</span><span class="sxs-lookup"><span data-stu-id="54206-116">newValue</span></span>|<span data-ttu-id="54206-117">String</span><span class="sxs-lookup"><span data-stu-id="54206-117">String</span></span>|<span data-ttu-id="54206-118">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="54206-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54206-119">Связи</span><span class="sxs-lookup"><span data-stu-id="54206-119">Relationships</span></span>
<span data-ttu-id="54206-120">Нет</span><span class="sxs-lookup"><span data-stu-id="54206-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="54206-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="54206-121">JSON Representation</span></span>
<span data-ttu-id="54206-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54206-122">Here is a JSON representation of the resource.</span></span>
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



