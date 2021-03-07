---
title: тип ресурса printServiceEndpoint
description: Представляет URI и идентифицирует сведения для экземпляра службы печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 0dd339d433be593e6982b6c38818635830a2d471
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517458"
---
# <a name="printserviceendpoint-resource-type"></a><span data-ttu-id="cb918-103">тип ресурса printServiceEndpoint</span><span class="sxs-lookup"><span data-stu-id="cb918-103">printServiceEndpoint resource type</span></span>

<span data-ttu-id="cb918-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb918-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="cb918-105">Представляет URI и идентифицирует сведения для экземпляра службы печати.</span><span class="sxs-lookup"><span data-stu-id="cb918-105">Represents URI and identifying information for a print service instance.</span></span>

## <a name="methods"></a><span data-ttu-id="cb918-106">Методы</span><span class="sxs-lookup"><span data-stu-id="cb918-106">Methods</span></span>
|<span data-ttu-id="cb918-107">Метод</span><span class="sxs-lookup"><span data-stu-id="cb918-107">Method</span></span>|<span data-ttu-id="cb918-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="cb918-108">Return type</span></span>|<span data-ttu-id="cb918-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cb918-109">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="cb918-110">Получение конечной точки</span><span class="sxs-lookup"><span data-stu-id="cb918-110">Get endpoint</span></span>](../api/printserviceendpoint-get.md) | [<span data-ttu-id="cb918-111">printServiceEndpoint</span><span class="sxs-lookup"><span data-stu-id="cb918-111">printServiceEndpoint</span></span>](printserviceendpoint.md) | <span data-ttu-id="cb918-112">Ознакомьтесь с свойствами и отношениями конечного объекта.</span><span class="sxs-lookup"><span data-stu-id="cb918-112">Read the properties and relationships of endpoint object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cb918-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb918-113">Properties</span></span>
|<span data-ttu-id="cb918-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb918-114">Property</span></span>|<span data-ttu-id="cb918-115">Тип</span><span class="sxs-lookup"><span data-stu-id="cb918-115">Type</span></span>|<span data-ttu-id="cb918-116">Описание</span><span class="sxs-lookup"><span data-stu-id="cb918-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb918-117">displayName</span><span class="sxs-lookup"><span data-stu-id="cb918-117">displayName</span></span>|<span data-ttu-id="cb918-118">Строка</span><span class="sxs-lookup"><span data-stu-id="cb918-118">String</span></span>|<span data-ttu-id="cb918-119">Имя отображения для конечной точки с читаемым для человека.</span><span class="sxs-lookup"><span data-stu-id="cb918-119">A human-readable display name for the endpoint.</span></span>|
|<span data-ttu-id="cb918-120">id</span><span class="sxs-lookup"><span data-stu-id="cb918-120">id</span></span>|<span data-ttu-id="cb918-121">Строка</span><span class="sxs-lookup"><span data-stu-id="cb918-121">String</span></span>|<span data-ttu-id="cb918-122">Уникальное имя, которое идентифицирует службу, которую предоставляет конечная точка.</span><span class="sxs-lookup"><span data-stu-id="cb918-122">A unique name that identifies the service that the endpoint provides.</span></span> <span data-ttu-id="cb918-123">Возможные значения: `discovery` (Служба обнаружения), `notification` (Служба уведомлений), `ipp` (служба IPP) и `registration` (Служба регистрации).</span><span class="sxs-lookup"><span data-stu-id="cb918-123">Possible values are: `discovery` (Discovery Service), `notification` (Notification Service), `ipp` (IPP Service), and `registration` (Registration Service).</span></span> <span data-ttu-id="cb918-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb918-124">Read-only.</span></span>|
|<span data-ttu-id="cb918-125">uri</span><span class="sxs-lookup"><span data-stu-id="cb918-125">uri</span></span>|<span data-ttu-id="cb918-126">Строка</span><span class="sxs-lookup"><span data-stu-id="cb918-126">String</span></span>|<span data-ttu-id="cb918-127">URI, который можно использовать для доступа к службе.</span><span class="sxs-lookup"><span data-stu-id="cb918-127">The URI that can be used to access the service.</span></span>|


## <a name="relationships"></a><span data-ttu-id="cb918-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="cb918-128">Relationships</span></span>
<span data-ttu-id="cb918-129">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cb918-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb918-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="cb918-130">JSON representation</span></span>
<span data-ttu-id="cb918-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb918-131">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printServiceEndpoint",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printServiceEndpoint",
  "id": "String (identifier)",
  "displayName": "String",
  "uri": "String"
}
```

