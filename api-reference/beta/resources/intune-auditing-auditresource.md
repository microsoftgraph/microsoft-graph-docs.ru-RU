---
title: Тип ресурса auditResource
description: Класс, содержащий свойства ресурса аудита.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a390f43daca9d86320eea29eb139406ad52476fe
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335223"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="899fa-103">Тип ресурса auditResource</span><span class="sxs-lookup"><span data-stu-id="899fa-103">auditResource resource type</span></span>

> <span data-ttu-id="899fa-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="899fa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="899fa-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="899fa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="899fa-106">Класс, содержащий свойства ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="899fa-106">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="899fa-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="899fa-107">Properties</span></span>
|<span data-ttu-id="899fa-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="899fa-108">Property</span></span>|<span data-ttu-id="899fa-109">Тип</span><span class="sxs-lookup"><span data-stu-id="899fa-109">Type</span></span>|<span data-ttu-id="899fa-110">Описание</span><span class="sxs-lookup"><span data-stu-id="899fa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="899fa-111">displayName</span><span class="sxs-lookup"><span data-stu-id="899fa-111">displayName</span></span>|<span data-ttu-id="899fa-112">Строка</span><span class="sxs-lookup"><span data-stu-id="899fa-112">String</span></span>|<span data-ttu-id="899fa-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="899fa-113">Display name.</span></span>|
|<span data-ttu-id="899fa-114">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="899fa-114">modifiedProperties</span></span>|<span data-ttu-id="899fa-115">Коллекция [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="899fa-115">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="899fa-116">Список измененных свойств.</span><span class="sxs-lookup"><span data-stu-id="899fa-116">List of modified properties.</span></span>|
|<span data-ttu-id="899fa-117">type</span><span class="sxs-lookup"><span data-stu-id="899fa-117">type</span></span>|<span data-ttu-id="899fa-118">String</span><span class="sxs-lookup"><span data-stu-id="899fa-118">String</span></span>|<span data-ttu-id="899fa-119">Тип ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="899fa-119">Audit resource's type.</span></span>|
|<span data-ttu-id="899fa-120">resourceId</span><span class="sxs-lookup"><span data-stu-id="899fa-120">resourceId</span></span>|<span data-ttu-id="899fa-121">String</span><span class="sxs-lookup"><span data-stu-id="899fa-121">String</span></span>|<span data-ttu-id="899fa-122">ИД ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="899fa-122">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="899fa-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="899fa-123">Relationships</span></span>
<span data-ttu-id="899fa-124">Нет</span><span class="sxs-lookup"><span data-stu-id="899fa-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="899fa-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="899fa-125">JSON Representation</span></span>
<span data-ttu-id="899fa-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="899fa-126">Here is a JSON representation of the resource.</span></span>
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



