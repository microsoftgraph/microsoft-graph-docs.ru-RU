---
title: detailsInfo resource type
description: Пакет свойств, который может содержать любую информацию о связанном удостоверении или системе.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 1841c513651131c4bf624c07ee117fae32df79f7
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240778"
---
# <a name="detailsinfo-resource-type"></a><span data-ttu-id="95211-103">detailsInfo resource type</span><span class="sxs-lookup"><span data-stu-id="95211-103">detailsInfo resource type</span></span>

<span data-ttu-id="95211-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95211-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="95211-105">Пакет свойств, который может содержать любую информацию о связанном удостоверении или системе.</span><span class="sxs-lookup"><span data-stu-id="95211-105">A property bag that can contain any information about the associated identity or system.</span></span> <span data-ttu-id="95211-106">Это может включать сведения о свойствах, которые в настоящее время подготовка или источник / целевая система.</span><span class="sxs-lookup"><span data-stu-id="95211-106">This can include details about the property that is being provisioned or the source/target system.</span></span>

## <a name="properties"></a><span data-ttu-id="95211-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="95211-107">Properties</span></span>
<span data-ttu-id="95211-108">Ресурс **detailsInfo** — это строка JSON, которая содержит дополнительные свойства, такие как **ApplicationId,** **ObjectId** и **UPN.**</span><span class="sxs-lookup"><span data-stu-id="95211-108">The **detailsInfo** resource is a JSON string that contains additional properties such as **ApplicationId**, **ObjectId**, and **UPN**.</span></span> <span data-ttu-id="95211-109">Набор свойств зависит от типа ресурса, который будет создан.</span><span class="sxs-lookup"><span data-stu-id="95211-109">The set of properties varies based on the type of resource that is being provisioned.</span></span> <span data-ttu-id="95211-110">[В примере list provisioningObjectSummary.](../api/provisioningobjectsummary-list.md)</span><span class="sxs-lookup"><span data-stu-id="95211-110">[List provisioningObjectSummary](../api/provisioningobjectsummary-list.md) shows an example of this.</span></span>

## <a name="relationships"></a><span data-ttu-id="95211-111">Связи</span><span class="sxs-lookup"><span data-stu-id="95211-111">Relationships</span></span>
<span data-ttu-id="95211-112">Нет</span><span class="sxs-lookup"><span data-stu-id="95211-112">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="95211-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="95211-113">JSON Representation</span></span>
<span data-ttu-id="95211-114">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95211-114">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.detailsInfo",
  "openType": true,
 "optionalProperties": [
 
 ],
}-->
``` json
{
  "@odata.type": "microsoft.graph.detailsInfo"
}
```


