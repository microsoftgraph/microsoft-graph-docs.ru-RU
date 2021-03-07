---
title: тип ресурса printService
description: Представляет описание конкретного клиента Azure AD экземпляра службы печати. Службы существуют для каждого компонента инфраструктуры печати (например, обнаружения, уведомления, регистрации и IPP) и имеют одну или несколько конечных точек.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 986749028a75f98157ff73138396a4ad56672fc8
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517463"
---
# <a name="printservice-resource-type"></a><span data-ttu-id="7cd08-104">тип ресурса printService</span><span class="sxs-lookup"><span data-stu-id="7cd08-104">printService resource type</span></span>

<span data-ttu-id="7cd08-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7cd08-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="7cd08-106">Представляет описание конкретного клиента Azure AD экземпляра службы печати.</span><span class="sxs-lookup"><span data-stu-id="7cd08-106">Represents an Azure AD tenant-specific description of a print service instance.</span></span> <span data-ttu-id="7cd08-107">Службы существуют для каждого компонента инфраструктуры печати (обнаружения, уведомлений, регистрации и IPP) и имеют одну или несколько конечных точек.</span><span class="sxs-lookup"><span data-stu-id="7cd08-107">Services exist for each component of the printing infrastructure (discovery, notifications, registration, and IPP) and have one or more endpoints.</span></span>

## <a name="methods"></a><span data-ttu-id="7cd08-108">Методы</span><span class="sxs-lookup"><span data-stu-id="7cd08-108">Methods</span></span>
|<span data-ttu-id="7cd08-109">Метод</span><span class="sxs-lookup"><span data-stu-id="7cd08-109">Method</span></span>|<span data-ttu-id="7cd08-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="7cd08-110">Return type</span></span>|<span data-ttu-id="7cd08-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7cd08-111">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="7cd08-112">Службы списка</span><span class="sxs-lookup"><span data-stu-id="7cd08-112">List services</span></span>](../api/print-list-services.md) | <span data-ttu-id="7cd08-113">[коллекция printService](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="7cd08-113">[printService](printservice.md) collection</span></span> | <span data-ttu-id="7cd08-114">Получите список служб универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="7cd08-114">Get a list of Universal Print services.</span></span> |
| [<span data-ttu-id="7cd08-115">Получить службу</span><span class="sxs-lookup"><span data-stu-id="7cd08-115">Get service</span></span>](../api/printservice-get.md) | [<span data-ttu-id="7cd08-116">printService</span><span class="sxs-lookup"><span data-stu-id="7cd08-116">printService</span></span>](printservice.md) | <span data-ttu-id="7cd08-117">Ознакомьтесь с свойствами и отношениями объекта-службы.</span><span class="sxs-lookup"><span data-stu-id="7cd08-117">Read the properties and relationships of service object.</span></span> |
| [<span data-ttu-id="7cd08-118">Перечисление конечных точек</span><span class="sxs-lookup"><span data-stu-id="7cd08-118">List endpoints</span></span>](../api/printservice-list-endpoints.md) | <span data-ttu-id="7cd08-119">[коллекция printServiceEndpoint](printserviceendpoint.md)</span><span class="sxs-lookup"><span data-stu-id="7cd08-119">[printServiceEndpoint](printserviceendpoint.md) collection</span></span> | <span data-ttu-id="7cd08-120">Получите список конечных точек, которые предоставляет служба.</span><span class="sxs-lookup"><span data-stu-id="7cd08-120">Get a list of endpoints that a service provides.</span></span> |

## <a name="properties"></a><span data-ttu-id="7cd08-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="7cd08-121">Properties</span></span>
|<span data-ttu-id="7cd08-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="7cd08-122">Property</span></span>|<span data-ttu-id="7cd08-123">Тип</span><span class="sxs-lookup"><span data-stu-id="7cd08-123">Type</span></span>|<span data-ttu-id="7cd08-124">Описание</span><span class="sxs-lookup"><span data-stu-id="7cd08-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cd08-125">id</span><span class="sxs-lookup"><span data-stu-id="7cd08-125">id</span></span>|<span data-ttu-id="7cd08-126">Строка</span><span class="sxs-lookup"><span data-stu-id="7cd08-126">String</span></span>|<span data-ttu-id="7cd08-127">Идентификатор службы.</span><span class="sxs-lookup"><span data-stu-id="7cd08-127">The service's identifier.</span></span> <span data-ttu-id="7cd08-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7cd08-128">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7cd08-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="7cd08-129">Relationships</span></span>
|<span data-ttu-id="7cd08-130">Связь</span><span class="sxs-lookup"><span data-stu-id="7cd08-130">Relationship</span></span>|<span data-ttu-id="7cd08-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7cd08-131">Type</span></span>|<span data-ttu-id="7cd08-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7cd08-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cd08-133">endpoints</span><span class="sxs-lookup"><span data-stu-id="7cd08-133">endpoints</span></span>|<span data-ttu-id="7cd08-134">[коллекция printServiceEndpoint](printserviceendpoint.md)</span><span class="sxs-lookup"><span data-stu-id="7cd08-134">[printServiceEndpoint](printserviceendpoint.md) collection</span></span>| <span data-ttu-id="7cd08-135">Конечные точки, которые можно использовать для доступа к службе.</span><span class="sxs-lookup"><span data-stu-id="7cd08-135">Endpoints that can be used to access the service.</span></span> <span data-ttu-id="7cd08-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7cd08-136">Read-only.</span></span> <span data-ttu-id="7cd08-137">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7cd08-137">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7cd08-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7cd08-138">JSON representation</span></span>
<span data-ttu-id="7cd08-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7cd08-139">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printService",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printService",
  "id": "String (identifier)"
}
```

