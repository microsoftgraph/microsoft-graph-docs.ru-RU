---
title: Тип ресурса auditResource
description: Класс, содержащий свойства ресурса аудита.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fa30fcb276661e3a673c1942c4d35cc71ca41e6b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759575"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="31603-103">Тип ресурса auditResource</span><span class="sxs-lookup"><span data-stu-id="31603-103">auditResource resource type</span></span>

<span data-ttu-id="31603-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31603-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="31603-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="31603-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31603-106">Класс, содержащий свойства ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="31603-106">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="31603-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="31603-107">Properties</span></span>
|<span data-ttu-id="31603-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="31603-108">Property</span></span>|<span data-ttu-id="31603-109">Тип</span><span class="sxs-lookup"><span data-stu-id="31603-109">Type</span></span>|<span data-ttu-id="31603-110">Описание</span><span class="sxs-lookup"><span data-stu-id="31603-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31603-111">displayName</span><span class="sxs-lookup"><span data-stu-id="31603-111">displayName</span></span>|<span data-ttu-id="31603-112">String</span><span class="sxs-lookup"><span data-stu-id="31603-112">String</span></span>|<span data-ttu-id="31603-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="31603-113">Display name.</span></span>|
|<span data-ttu-id="31603-114">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="31603-114">modifiedProperties</span></span>|<span data-ttu-id="31603-115">Коллекция [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="31603-115">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="31603-116">Список измененных свойств.</span><span class="sxs-lookup"><span data-stu-id="31603-116">List of modified properties.</span></span>|
|<span data-ttu-id="31603-117">type</span><span class="sxs-lookup"><span data-stu-id="31603-117">type</span></span>|<span data-ttu-id="31603-118">String</span><span class="sxs-lookup"><span data-stu-id="31603-118">String</span></span>|<span data-ttu-id="31603-119">Тип ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="31603-119">Audit resource's type.</span></span>|
|<span data-ttu-id="31603-120">resourceId</span><span class="sxs-lookup"><span data-stu-id="31603-120">resourceId</span></span>|<span data-ttu-id="31603-121">String</span><span class="sxs-lookup"><span data-stu-id="31603-121">String</span></span>|<span data-ttu-id="31603-122">ИД ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="31603-122">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="31603-123">Связи</span><span class="sxs-lookup"><span data-stu-id="31603-123">Relationships</span></span>
<span data-ttu-id="31603-124">Нет</span><span class="sxs-lookup"><span data-stu-id="31603-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="31603-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="31603-125">JSON Representation</span></span>
<span data-ttu-id="31603-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31603-126">Here is a JSON representation of the resource.</span></span>
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




