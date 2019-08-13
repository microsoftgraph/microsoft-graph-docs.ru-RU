---
title: Тип ресурса auditProperty
description: Класс, содержащий свойства для свойства аудита.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 331c786d7fd21687a0581ae56746d9e0b48f7c04
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335230"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="81296-103">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="81296-103">auditProperty resource type</span></span>

> <span data-ttu-id="81296-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81296-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81296-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="81296-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81296-106">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="81296-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="81296-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="81296-107">Properties</span></span>
|<span data-ttu-id="81296-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="81296-108">Property</span></span>|<span data-ttu-id="81296-109">Тип</span><span class="sxs-lookup"><span data-stu-id="81296-109">Type</span></span>|<span data-ttu-id="81296-110">Описание</span><span class="sxs-lookup"><span data-stu-id="81296-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81296-111">displayName</span><span class="sxs-lookup"><span data-stu-id="81296-111">displayName</span></span>|<span data-ttu-id="81296-112">String</span><span class="sxs-lookup"><span data-stu-id="81296-112">String</span></span>|<span data-ttu-id="81296-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="81296-113">Display name.</span></span>|
|<span data-ttu-id="81296-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="81296-114">oldValue</span></span>|<span data-ttu-id="81296-115">String</span><span class="sxs-lookup"><span data-stu-id="81296-115">String</span></span>|<span data-ttu-id="81296-116">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="81296-116">Old value.</span></span>|
|<span data-ttu-id="81296-117">newValue</span><span class="sxs-lookup"><span data-stu-id="81296-117">newValue</span></span>|<span data-ttu-id="81296-118">String</span><span class="sxs-lookup"><span data-stu-id="81296-118">String</span></span>|<span data-ttu-id="81296-119">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="81296-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81296-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="81296-120">Relationships</span></span>
<span data-ttu-id="81296-121">Нет</span><span class="sxs-lookup"><span data-stu-id="81296-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81296-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="81296-122">JSON Representation</span></span>
<span data-ttu-id="81296-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81296-123">Here is a JSON representation of the resource.</span></span>
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



