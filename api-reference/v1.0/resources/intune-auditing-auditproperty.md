---
title: Тип ресурса auditProperty
description: Класс, содержащий свойства для свойства аудита.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 290aae8c245fd09c17fc766cedd7c2e253626943
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912031"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="99f5d-103">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="99f5d-103">auditProperty resource type</span></span>

> <span data-ttu-id="99f5d-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="99f5d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="99f5d-105">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="99f5d-105">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="99f5d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="99f5d-106">Properties</span></span>
|<span data-ttu-id="99f5d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="99f5d-107">Property</span></span>|<span data-ttu-id="99f5d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="99f5d-108">Type</span></span>|<span data-ttu-id="99f5d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="99f5d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99f5d-110">displayName</span><span class="sxs-lookup"><span data-stu-id="99f5d-110">displayName</span></span>|<span data-ttu-id="99f5d-111">String</span><span class="sxs-lookup"><span data-stu-id="99f5d-111">String</span></span>|<span data-ttu-id="99f5d-112">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="99f5d-112">Display name.</span></span>|
|<span data-ttu-id="99f5d-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="99f5d-113">oldValue</span></span>|<span data-ttu-id="99f5d-114">String</span><span class="sxs-lookup"><span data-stu-id="99f5d-114">String</span></span>|<span data-ttu-id="99f5d-115">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="99f5d-115">Old value.</span></span>|
|<span data-ttu-id="99f5d-116">newValue</span><span class="sxs-lookup"><span data-stu-id="99f5d-116">newValue</span></span>|<span data-ttu-id="99f5d-117">String</span><span class="sxs-lookup"><span data-stu-id="99f5d-117">String</span></span>|<span data-ttu-id="99f5d-118">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="99f5d-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99f5d-119">Связи</span><span class="sxs-lookup"><span data-stu-id="99f5d-119">Relationships</span></span>
<span data-ttu-id="99f5d-120">Нет</span><span class="sxs-lookup"><span data-stu-id="99f5d-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="99f5d-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="99f5d-121">JSON Representation</span></span>
<span data-ttu-id="99f5d-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99f5d-122">Here is a JSON representation of the resource.</span></span>
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



