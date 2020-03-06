---
title: Тип ресурса auditProperty
description: Класс, содержащий свойства для свойства аудита.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c63f390e31e83cfed64ee2a28bba4e4af0dfa756
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532729"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="6f0a6-103">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="6f0a6-103">auditProperty resource type</span></span>

<span data-ttu-id="6f0a6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f0a6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f0a6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6f0a6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f0a6-106">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="6f0a6-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="6f0a6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f0a6-107">Properties</span></span>
|<span data-ttu-id="6f0a6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f0a6-108">Property</span></span>|<span data-ttu-id="6f0a6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6f0a6-109">Type</span></span>|<span data-ttu-id="6f0a6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6f0a6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f0a6-111">displayName</span><span class="sxs-lookup"><span data-stu-id="6f0a6-111">displayName</span></span>|<span data-ttu-id="6f0a6-112">Строка</span><span class="sxs-lookup"><span data-stu-id="6f0a6-112">String</span></span>|<span data-ttu-id="6f0a6-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="6f0a6-113">Display name.</span></span>|
|<span data-ttu-id="6f0a6-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="6f0a6-114">oldValue</span></span>|<span data-ttu-id="6f0a6-115">Строка</span><span class="sxs-lookup"><span data-stu-id="6f0a6-115">String</span></span>|<span data-ttu-id="6f0a6-116">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="6f0a6-116">Old value.</span></span>|
|<span data-ttu-id="6f0a6-117">newValue</span><span class="sxs-lookup"><span data-stu-id="6f0a6-117">newValue</span></span>|<span data-ttu-id="6f0a6-118">String</span><span class="sxs-lookup"><span data-stu-id="6f0a6-118">String</span></span>|<span data-ttu-id="6f0a6-119">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="6f0a6-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f0a6-120">Связи</span><span class="sxs-lookup"><span data-stu-id="6f0a6-120">Relationships</span></span>
<span data-ttu-id="6f0a6-121">Нет</span><span class="sxs-lookup"><span data-stu-id="6f0a6-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f0a6-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f0a6-122">JSON Representation</span></span>
<span data-ttu-id="6f0a6-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f0a6-123">Here is a JSON representation of the resource.</span></span>
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




