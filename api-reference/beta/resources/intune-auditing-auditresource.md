---
title: Тип ресурса auditResource
description: Класс, содержащий свойства ресурса аудита.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ac2aa3f39f88635f403a0b5dbccd8b366fc1683e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797418"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="9effd-103">Тип ресурса auditResource</span><span class="sxs-lookup"><span data-stu-id="9effd-103">auditResource resource type</span></span>

> <span data-ttu-id="9effd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9effd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9effd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9effd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9effd-106">Класс, содержащий свойства ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="9effd-106">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="9effd-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9effd-107">Properties</span></span>
|<span data-ttu-id="9effd-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9effd-108">Property</span></span>|<span data-ttu-id="9effd-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9effd-109">Type</span></span>|<span data-ttu-id="9effd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9effd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9effd-111">displayName</span><span class="sxs-lookup"><span data-stu-id="9effd-111">displayName</span></span>|<span data-ttu-id="9effd-112">Строка</span><span class="sxs-lookup"><span data-stu-id="9effd-112">String</span></span>|<span data-ttu-id="9effd-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="9effd-113">Display name.</span></span>|
|<span data-ttu-id="9effd-114">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="9effd-114">modifiedProperties</span></span>|<span data-ttu-id="9effd-115">Коллекция [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="9effd-115">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="9effd-116">Список измененных свойств.</span><span class="sxs-lookup"><span data-stu-id="9effd-116">List of modified properties.</span></span>|
|<span data-ttu-id="9effd-117">type</span><span class="sxs-lookup"><span data-stu-id="9effd-117">type</span></span>|<span data-ttu-id="9effd-118">String</span><span class="sxs-lookup"><span data-stu-id="9effd-118">String</span></span>|<span data-ttu-id="9effd-119">Тип ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="9effd-119">Audit resource's type.</span></span>|
|<span data-ttu-id="9effd-120">resourceId</span><span class="sxs-lookup"><span data-stu-id="9effd-120">resourceId</span></span>|<span data-ttu-id="9effd-121">String</span><span class="sxs-lookup"><span data-stu-id="9effd-121">String</span></span>|<span data-ttu-id="9effd-122">ИД ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="9effd-122">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9effd-123">Связи</span><span class="sxs-lookup"><span data-stu-id="9effd-123">Relationships</span></span>
<span data-ttu-id="9effd-124">Нет</span><span class="sxs-lookup"><span data-stu-id="9effd-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9effd-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9effd-125">JSON Representation</span></span>
<span data-ttu-id="9effd-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9effd-126">Here is a JSON representation of the resource.</span></span>
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



