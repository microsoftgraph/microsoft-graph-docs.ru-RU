---
title: Тип ресурса detailsInfo
description: Пакет свойств, который может содержать любые сведения о связанном удостоверении или системе.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 25441071581af0b9e35ef941d8c82998bdea7b38
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135662"
---
# <a name="detailsinfo-resource-type"></a><span data-ttu-id="f89f7-103">Тип ресурса detailsInfo</span><span class="sxs-lookup"><span data-stu-id="f89f7-103">detailsInfo resource type</span></span>

<span data-ttu-id="f89f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f89f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f89f7-105">Пакет свойств, который может содержать любые сведения о связанном удостоверении или системе.</span><span class="sxs-lookup"><span data-stu-id="f89f7-105">A property bag that can contain any information about the associated identity or system.</span></span> <span data-ttu-id="f89f7-106">Это может включать сведения о свойстве, которое необходимо получить, или источник/целевая система.</span><span class="sxs-lookup"><span data-stu-id="f89f7-106">This can include details about the property that is being provisioned or the source/target system.</span></span>

## <a name="properties"></a><span data-ttu-id="f89f7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f89f7-107">Properties</span></span>
<span data-ttu-id="f89f7-108">Ресурс **detailsInfo —** это строка JSON, которая содержит дополнительные свойства, такие как **ApplicationId,** **ObjectId** и **UPN.**</span><span class="sxs-lookup"><span data-stu-id="f89f7-108">The **detailsInfo** resource is a JSON string that contains additional properties such as **ApplicationId**, **ObjectId**, and **UPN**.</span></span> <span data-ttu-id="f89f7-109">Набор свойств зависит от типа ресурса, который необходимо создать.</span><span class="sxs-lookup"><span data-stu-id="f89f7-109">The set of properties varies based on the type of resource that is being provisioned.</span></span> <span data-ttu-id="f89f7-110">[Пример этого показан в списке provisioningObjectSummary.](../api/provisioningobjectsummary-list.md)</span><span class="sxs-lookup"><span data-stu-id="f89f7-110">[List provisioningObjectSummary](../api/provisioningobjectsummary-list.md) shows an example of this.</span></span>

## <a name="relationships"></a><span data-ttu-id="f89f7-111">Связи</span><span class="sxs-lookup"><span data-stu-id="f89f7-111">Relationships</span></span>
<span data-ttu-id="f89f7-112">Нет</span><span class="sxs-lookup"><span data-stu-id="f89f7-112">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f89f7-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f89f7-113">JSON Representation</span></span>
<span data-ttu-id="f89f7-114">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f89f7-114">Here is a JSON representation of the resource.</span></span>
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


