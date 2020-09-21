---
title: Тип ресурса auditResource
description: Класс, содержащий свойства ресурса аудита.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 895f88bf20219447e9f9609271b731b941263798
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965682"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="029ef-103">Тип ресурса auditResource</span><span class="sxs-lookup"><span data-stu-id="029ef-103">auditResource resource type</span></span>

<span data-ttu-id="029ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="029ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="029ef-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="029ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="029ef-106">Класс, содержащий свойства ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="029ef-106">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="029ef-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="029ef-107">Properties</span></span>
|<span data-ttu-id="029ef-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="029ef-108">Property</span></span>|<span data-ttu-id="029ef-109">Тип</span><span class="sxs-lookup"><span data-stu-id="029ef-109">Type</span></span>|<span data-ttu-id="029ef-110">Описание</span><span class="sxs-lookup"><span data-stu-id="029ef-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="029ef-111">displayName</span><span class="sxs-lookup"><span data-stu-id="029ef-111">displayName</span></span>|<span data-ttu-id="029ef-112">String</span><span class="sxs-lookup"><span data-stu-id="029ef-112">String</span></span>|<span data-ttu-id="029ef-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="029ef-113">Display name.</span></span>|
|<span data-ttu-id="029ef-114">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="029ef-114">modifiedProperties</span></span>|<span data-ttu-id="029ef-115">Коллекция [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="029ef-115">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="029ef-116">Список измененных свойств.</span><span class="sxs-lookup"><span data-stu-id="029ef-116">List of modified properties.</span></span>|
|<span data-ttu-id="029ef-117">type</span><span class="sxs-lookup"><span data-stu-id="029ef-117">type</span></span>|<span data-ttu-id="029ef-118">String</span><span class="sxs-lookup"><span data-stu-id="029ef-118">String</span></span>|<span data-ttu-id="029ef-119">Тип ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="029ef-119">Audit resource's type.</span></span>|
|<span data-ttu-id="029ef-120">resourceId</span><span class="sxs-lookup"><span data-stu-id="029ef-120">resourceId</span></span>|<span data-ttu-id="029ef-121">String</span><span class="sxs-lookup"><span data-stu-id="029ef-121">String</span></span>|<span data-ttu-id="029ef-122">ИД ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="029ef-122">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="029ef-123">Связи</span><span class="sxs-lookup"><span data-stu-id="029ef-123">Relationships</span></span>
<span data-ttu-id="029ef-124">Нет</span><span class="sxs-lookup"><span data-stu-id="029ef-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="029ef-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="029ef-125">JSON Representation</span></span>
<span data-ttu-id="029ef-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="029ef-126">Here is a JSON representation of the resource.</span></span>
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









