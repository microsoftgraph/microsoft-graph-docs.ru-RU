---
title: Тип ресурса auditResource
description: Класс, содержащий свойства ресурса аудита.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3aae8d82706d25ed95e238c8c4dfa07516c64771
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472099"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="46a82-103">Тип ресурса auditResource</span><span class="sxs-lookup"><span data-stu-id="46a82-103">auditResource resource type</span></span>

<span data-ttu-id="46a82-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46a82-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="46a82-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46a82-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46a82-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46a82-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46a82-107">Класс, содержащий свойства ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="46a82-107">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="46a82-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="46a82-108">Properties</span></span>
|<span data-ttu-id="46a82-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="46a82-109">Property</span></span>|<span data-ttu-id="46a82-110">Тип</span><span class="sxs-lookup"><span data-stu-id="46a82-110">Type</span></span>|<span data-ttu-id="46a82-111">Описание</span><span class="sxs-lookup"><span data-stu-id="46a82-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46a82-112">displayName</span><span class="sxs-lookup"><span data-stu-id="46a82-112">displayName</span></span>|<span data-ttu-id="46a82-113">Строка</span><span class="sxs-lookup"><span data-stu-id="46a82-113">String</span></span>|<span data-ttu-id="46a82-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="46a82-114">Display name.</span></span>|
|<span data-ttu-id="46a82-115">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="46a82-115">modifiedProperties</span></span>|<span data-ttu-id="46a82-116">Коллекция [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="46a82-116">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="46a82-117">Список измененных свойств.</span><span class="sxs-lookup"><span data-stu-id="46a82-117">List of modified properties.</span></span>|
|<span data-ttu-id="46a82-118">type</span><span class="sxs-lookup"><span data-stu-id="46a82-118">type</span></span>|<span data-ttu-id="46a82-119">String</span><span class="sxs-lookup"><span data-stu-id="46a82-119">String</span></span>|<span data-ttu-id="46a82-120">Тип ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="46a82-120">Audit resource's type.</span></span>|
|<span data-ttu-id="46a82-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="46a82-121">resourceId</span></span>|<span data-ttu-id="46a82-122">String</span><span class="sxs-lookup"><span data-stu-id="46a82-122">String</span></span>|<span data-ttu-id="46a82-123">ИД ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="46a82-123">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="46a82-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="46a82-124">Relationships</span></span>
<span data-ttu-id="46a82-125">Нет</span><span class="sxs-lookup"><span data-stu-id="46a82-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="46a82-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="46a82-126">JSON Representation</span></span>
<span data-ttu-id="46a82-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46a82-127">Here is a JSON representation of the resource.</span></span>
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



