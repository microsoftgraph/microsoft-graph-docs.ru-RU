---
title: Тип ресурса auditProperty
description: Класс, содержащий свойства для свойства аудита.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3425c59ae4f30b30b04bd22f74cb1b27ad99191f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416645"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="c66c9-103">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="c66c9-103">auditProperty resource type</span></span>

> <span data-ttu-id="c66c9-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c66c9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c66c9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c66c9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c66c9-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c66c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c66c9-107">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="c66c9-107">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="c66c9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c66c9-108">Properties</span></span>
|<span data-ttu-id="c66c9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c66c9-109">Property</span></span>|<span data-ttu-id="c66c9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c66c9-110">Type</span></span>|<span data-ttu-id="c66c9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c66c9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c66c9-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c66c9-112">displayName</span></span>|<span data-ttu-id="c66c9-113">String</span><span class="sxs-lookup"><span data-stu-id="c66c9-113">String</span></span>|<span data-ttu-id="c66c9-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="c66c9-114">Display name.</span></span>|
|<span data-ttu-id="c66c9-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="c66c9-115">oldValue</span></span>|<span data-ttu-id="c66c9-116">String</span><span class="sxs-lookup"><span data-stu-id="c66c9-116">String</span></span>|<span data-ttu-id="c66c9-117">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="c66c9-117">Old value.</span></span>|
|<span data-ttu-id="c66c9-118">newValue</span><span class="sxs-lookup"><span data-stu-id="c66c9-118">newValue</span></span>|<span data-ttu-id="c66c9-119">String</span><span class="sxs-lookup"><span data-stu-id="c66c9-119">String</span></span>|<span data-ttu-id="c66c9-120">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="c66c9-120">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c66c9-121">Связи</span><span class="sxs-lookup"><span data-stu-id="c66c9-121">Relationships</span></span>
<span data-ttu-id="c66c9-122">Нет</span><span class="sxs-lookup"><span data-stu-id="c66c9-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c66c9-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c66c9-123">JSON Representation</span></span>
<span data-ttu-id="c66c9-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c66c9-124">Here is a JSON representation of the resource.</span></span>
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




