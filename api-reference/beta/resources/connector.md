---
title: Тип соединителя ресурсов
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 98fa998a37b01ad64e556b229912932f4d1cfc75
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884625"
---
# <a name="connector-resource-type"></a><span data-ttu-id="bd22e-103">Тип соединителя ресурсов</span><span class="sxs-lookup"><span data-stu-id="bd22e-103">connector resource type</span></span>

> <span data-ttu-id="bd22e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bd22e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd22e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd22e-105">Use of these APIs in production applications is not supported.</span></span>

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a><span data-ttu-id="bd22e-106">Методы</span><span class="sxs-lookup"><span data-stu-id="bd22e-106">Methods</span></span>

| <span data-ttu-id="bd22e-107">Метод</span><span class="sxs-lookup"><span data-stu-id="bd22e-107">Method</span></span>           | <span data-ttu-id="bd22e-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bd22e-108">Return Type</span></span>    |<span data-ttu-id="bd22e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bd22e-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bd22e-110">Получение соединителя</span><span class="sxs-lookup"><span data-stu-id="bd22e-110">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="bd22e-111">Соединитель</span><span class="sxs-lookup"><span data-stu-id="bd22e-111">connector</span></span>](connector.md) |<span data-ttu-id="bd22e-112">Чтение свойства и связи объекта соединителя.</span><span class="sxs-lookup"><span data-stu-id="bd22e-112">Read properties and relationships of connector object.</span></span>|
|[<span data-ttu-id="bd22e-113">Перечисление memberOf</span><span class="sxs-lookup"><span data-stu-id="bd22e-113">List memberOf</span></span>](../api/connector-list-memberof.md) |<span data-ttu-id="bd22e-114">[connectorGroup](connectorgroup.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="bd22e-114">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="bd22e-115">Получите объект connectorGroup, связанный с соединителем.</span><span class="sxs-lookup"><span data-stu-id="bd22e-115">Get the connectorGroup object associated with the connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="bd22e-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd22e-116">Properties</span></span>
| <span data-ttu-id="bd22e-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd22e-117">Property</span></span>     | <span data-ttu-id="bd22e-118">Тип</span><span class="sxs-lookup"><span data-stu-id="bd22e-118">Type</span></span>   |<span data-ttu-id="bd22e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="bd22e-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd22e-120">externalIp</span><span class="sxs-lookup"><span data-stu-id="bd22e-120">externalIp</span></span>|<span data-ttu-id="bd22e-121">Строка</span><span class="sxs-lookup"><span data-stu-id="bd22e-121">String</span></span>|<span data-ttu-id="bd22e-122">Внешний IP-адрес как вредоносным службой для этого соединителя компьютера.</span><span class="sxs-lookup"><span data-stu-id="bd22e-122">The external IP address as detected by the service for the connector machine.</span></span> <span data-ttu-id="bd22e-123">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="bd22e-123">Read-only</span></span>|
|<span data-ttu-id="bd22e-124">id</span><span class="sxs-lookup"><span data-stu-id="bd22e-124">id</span></span>|<span data-ttu-id="bd22e-125">Строка</span><span class="sxs-lookup"><span data-stu-id="bd22e-125">String</span></span>| <span data-ttu-id="bd22e-126">Идентификатор объекта соединитель.</span><span class="sxs-lookup"><span data-stu-id="bd22e-126">The object id of the connector.</span></span> <BR><span data-ttu-id="bd22e-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bd22e-127">Read-only.</span></span>|
|<span data-ttu-id="bd22e-128">имя_компьютера</span><span class="sxs-lookup"><span data-stu-id="bd22e-128">machineName</span></span>|<span data-ttu-id="bd22e-129">Строка</span><span class="sxs-lookup"><span data-stu-id="bd22e-129">String</span></span>| <span data-ttu-id="bd22e-130">Имя компьютера, на котором работает соединитель.</span><span class="sxs-lookup"><span data-stu-id="bd22e-130">The name of the machine that the connector is running on.</span></span> <BR><span data-ttu-id="bd22e-131">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="bd22e-131">Read-only</span></span>|
|<span data-ttu-id="bd22e-132">status</span><span class="sxs-lookup"><span data-stu-id="bd22e-132">status</span></span>|<span data-ttu-id="bd22e-133">string</span><span class="sxs-lookup"><span data-stu-id="bd22e-133">string</span></span>| <span data-ttu-id="bd22e-134">Указывает состояние соединителя.</span><span class="sxs-lookup"><span data-stu-id="bd22e-134">Indicates the status of the connector.</span></span> <span data-ttu-id="bd22e-135">Возможные значения: `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="bd22e-135">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="bd22e-136">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="bd22e-136">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="bd22e-137">Связи</span><span class="sxs-lookup"><span data-stu-id="bd22e-137">Relationships</span></span>
| <span data-ttu-id="bd22e-138">Связь</span><span class="sxs-lookup"><span data-stu-id="bd22e-138">Relationship</span></span> | <span data-ttu-id="bd22e-139">Тип</span><span class="sxs-lookup"><span data-stu-id="bd22e-139">Type</span></span>   |<span data-ttu-id="bd22e-140">Описание</span><span class="sxs-lookup"><span data-stu-id="bd22e-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd22e-141">memberOf</span><span class="sxs-lookup"><span data-stu-id="bd22e-141">memberOf</span></span>|<span data-ttu-id="bd22e-142">[connectorGroup](connectorgroup.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="bd22e-142">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="bd22e-143">ConnectorGroup, который является членом подключиться.</span><span class="sxs-lookup"><span data-stu-id="bd22e-143">The connectorGroup that the connect is a member of.</span></span><br><span data-ttu-id="bd22e-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bd22e-144">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bd22e-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bd22e-145">JSON representation</span></span>

<span data-ttu-id="bd22e-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd22e-146">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connector"
}-->

```json
{
  "externalIp": "String",
  "id": "String (identifier)",
  "machineName": "String",
  "status": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
