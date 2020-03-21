---
title: Тип ресурса Принтсервицеендпоинт
description: Представляет URI и идентификационные данные для экземпляра службы печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 7f28245c22916575d505b3e9f8db65070cbbbf5e
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896062"
---
# <a name="printserviceendpoint-resource-type"></a><span data-ttu-id="434cc-103">Тип ресурса Принтсервицеендпоинт</span><span class="sxs-lookup"><span data-stu-id="434cc-103">printServiceEndpoint resource type</span></span>

<span data-ttu-id="434cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="434cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="434cc-105">Представляет URI и идентификационные данные для экземпляра службы печати.</span><span class="sxs-lookup"><span data-stu-id="434cc-105">Represents URI and identifying information for a print service instance.</span></span>

## <a name="methods"></a><span data-ttu-id="434cc-106">Методы</span><span class="sxs-lookup"><span data-stu-id="434cc-106">Methods</span></span>

| <span data-ttu-id="434cc-107">Метод</span><span class="sxs-lookup"><span data-stu-id="434cc-107">Method</span></span>       | <span data-ttu-id="434cc-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="434cc-108">Return Type</span></span> | <span data-ttu-id="434cc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="434cc-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="434cc-110">Получение конечной точки</span><span class="sxs-lookup"><span data-stu-id="434cc-110">Get endpoint</span></span>](../api/printserviceendpoint-get.md) | [<span data-ttu-id="434cc-111">принтсервицеендпоинт</span><span class="sxs-lookup"><span data-stu-id="434cc-111">printServiceEndpoint</span></span>](printserviceendpoint.md) | <span data-ttu-id="434cc-112">Считывание свойств и связей объекта Endpoint.</span><span class="sxs-lookup"><span data-stu-id="434cc-112">Read the properties and relationships of endpoint object.</span></span> |

## <a name="properties"></a><span data-ttu-id="434cc-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="434cc-113">Properties</span></span>
| <span data-ttu-id="434cc-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="434cc-114">Property</span></span>     | <span data-ttu-id="434cc-115">Тип</span><span class="sxs-lookup"><span data-stu-id="434cc-115">Type</span></span>        | <span data-ttu-id="434cc-116">Описание</span><span class="sxs-lookup"><span data-stu-id="434cc-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="434cc-117">displayName</span><span class="sxs-lookup"><span data-stu-id="434cc-117">displayName</span></span>|<span data-ttu-id="434cc-118">Строка</span><span class="sxs-lookup"><span data-stu-id="434cc-118">String</span></span>|<span data-ttu-id="434cc-119">Понятное для пользователя отображаемое имя для конечной точки.</span><span class="sxs-lookup"><span data-stu-id="434cc-119">A human-readable display name for the endpoint.</span></span>|
|<span data-ttu-id="434cc-120">name</span><span class="sxs-lookup"><span data-stu-id="434cc-120">name</span></span>|<span data-ttu-id="434cc-121">String</span><span class="sxs-lookup"><span data-stu-id="434cc-121">String</span></span>|<span data-ttu-id="434cc-122">Уникальное имя, идентифицирующее службу, которую предоставляет конечная точка.</span><span class="sxs-lookup"><span data-stu-id="434cc-122">A unique name that identifies the service that the endpoint provides.</span></span> <span data-ttu-id="434cc-123">`discovery` Возможные значения: (служба обнаружения) `notification` , (служба уведомлений), `ipp` (Служба протокола IPP) и `registration` (служба регистрации).</span><span class="sxs-lookup"><span data-stu-id="434cc-123">Possible values are: `discovery` (Discovery Service), `notification` (Notification Service), `ipp` (IPP Service), and `registration` (Registration Service).</span></span> <span data-ttu-id="434cc-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="434cc-124">Read-only.</span></span>|
|<span data-ttu-id="434cc-125">URI</span><span class="sxs-lookup"><span data-stu-id="434cc-125">uri</span></span>|<span data-ttu-id="434cc-126">String</span><span class="sxs-lookup"><span data-stu-id="434cc-126">String</span></span>|<span data-ttu-id="434cc-127">Универсальный код ресурса (URI), который можно использовать для доступа к службе.</span><span class="sxs-lookup"><span data-stu-id="434cc-127">The URI that can be used to access the service.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="434cc-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="434cc-128">JSON representation</span></span>

<span data-ttu-id="434cc-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="434cc-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printServiceEndpoint"
}-->

```json
{
  "displayName": "String",
  "name": "String (identifier)",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printServiceEndpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->