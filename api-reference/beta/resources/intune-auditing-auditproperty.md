---
title: Тип ресурса auditProperty
description: Класс, содержащий свойства для свойства аудита.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 67a70ff1cafab25372931597392c21eb77dd6c7b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42489400"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="35344-103">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="35344-103">auditProperty resource type</span></span>

<span data-ttu-id="35344-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="35344-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="35344-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35344-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35344-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="35344-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35344-107">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="35344-107">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="35344-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="35344-108">Properties</span></span>
|<span data-ttu-id="35344-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="35344-109">Property</span></span>|<span data-ttu-id="35344-110">Тип</span><span class="sxs-lookup"><span data-stu-id="35344-110">Type</span></span>|<span data-ttu-id="35344-111">Описание</span><span class="sxs-lookup"><span data-stu-id="35344-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35344-112">displayName</span><span class="sxs-lookup"><span data-stu-id="35344-112">displayName</span></span>|<span data-ttu-id="35344-113">String</span><span class="sxs-lookup"><span data-stu-id="35344-113">String</span></span>|<span data-ttu-id="35344-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="35344-114">Display name.</span></span>|
|<span data-ttu-id="35344-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="35344-115">oldValue</span></span>|<span data-ttu-id="35344-116">String</span><span class="sxs-lookup"><span data-stu-id="35344-116">String</span></span>|<span data-ttu-id="35344-117">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="35344-117">Old value.</span></span>|
|<span data-ttu-id="35344-118">newValue</span><span class="sxs-lookup"><span data-stu-id="35344-118">newValue</span></span>|<span data-ttu-id="35344-119">String</span><span class="sxs-lookup"><span data-stu-id="35344-119">String</span></span>|<span data-ttu-id="35344-120">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="35344-120">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35344-121">Связи</span><span class="sxs-lookup"><span data-stu-id="35344-121">Relationships</span></span>
<span data-ttu-id="35344-122">Нет</span><span class="sxs-lookup"><span data-stu-id="35344-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35344-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35344-123">JSON Representation</span></span>
<span data-ttu-id="35344-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35344-124">Here is a JSON representation of the resource.</span></span>
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



