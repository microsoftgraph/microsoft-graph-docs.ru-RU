---
title: Тип ресурса auditResource
description: Класс, содержащий свойства ресурса аудита.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9372c69d977be434bc963325f8ec93e68defca50
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42489393"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="06bba-103">Тип ресурса auditResource</span><span class="sxs-lookup"><span data-stu-id="06bba-103">auditResource resource type</span></span>

<span data-ttu-id="06bba-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="06bba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06bba-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06bba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06bba-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="06bba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06bba-107">Класс, содержащий свойства ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="06bba-107">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="06bba-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="06bba-108">Properties</span></span>
|<span data-ttu-id="06bba-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="06bba-109">Property</span></span>|<span data-ttu-id="06bba-110">Тип</span><span class="sxs-lookup"><span data-stu-id="06bba-110">Type</span></span>|<span data-ttu-id="06bba-111">Описание</span><span class="sxs-lookup"><span data-stu-id="06bba-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06bba-112">displayName</span><span class="sxs-lookup"><span data-stu-id="06bba-112">displayName</span></span>|<span data-ttu-id="06bba-113">Строка</span><span class="sxs-lookup"><span data-stu-id="06bba-113">String</span></span>|<span data-ttu-id="06bba-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="06bba-114">Display name.</span></span>|
|<span data-ttu-id="06bba-115">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="06bba-115">modifiedProperties</span></span>|<span data-ttu-id="06bba-116">Коллекция [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="06bba-116">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="06bba-117">Список измененных свойств.</span><span class="sxs-lookup"><span data-stu-id="06bba-117">List of modified properties.</span></span>|
|<span data-ttu-id="06bba-118">type</span><span class="sxs-lookup"><span data-stu-id="06bba-118">type</span></span>|<span data-ttu-id="06bba-119">String</span><span class="sxs-lookup"><span data-stu-id="06bba-119">String</span></span>|<span data-ttu-id="06bba-120">Тип ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="06bba-120">Audit resource's type.</span></span>|
|<span data-ttu-id="06bba-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="06bba-121">resourceId</span></span>|<span data-ttu-id="06bba-122">String</span><span class="sxs-lookup"><span data-stu-id="06bba-122">String</span></span>|<span data-ttu-id="06bba-123">ИД ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="06bba-123">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06bba-124">Связи</span><span class="sxs-lookup"><span data-stu-id="06bba-124">Relationships</span></span>
<span data-ttu-id="06bba-125">Нет</span><span class="sxs-lookup"><span data-stu-id="06bba-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06bba-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="06bba-126">JSON Representation</span></span>
<span data-ttu-id="06bba-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="06bba-127">Here is a JSON representation of the resource.</span></span>
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



