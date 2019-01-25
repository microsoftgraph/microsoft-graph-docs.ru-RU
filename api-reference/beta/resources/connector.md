---
title: Тип соединителя ресурсов
description: Ниже показано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: eed936c808e920f35a741a836a1fab64b2754bf8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525733"
---
# <a name="connector-resource-type"></a><span data-ttu-id="0ceb3-103">Тип соединителя ресурсов</span><span class="sxs-lookup"><span data-stu-id="0ceb3-103">connector resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a><span data-ttu-id="0ceb3-104">Методы</span><span class="sxs-lookup"><span data-stu-id="0ceb3-104">Methods</span></span>

| <span data-ttu-id="0ceb3-105">Метод</span><span class="sxs-lookup"><span data-stu-id="0ceb3-105">Method</span></span>           | <span data-ttu-id="0ceb3-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0ceb3-106">Return Type</span></span>    |<span data-ttu-id="0ceb3-107">Описание</span><span class="sxs-lookup"><span data-stu-id="0ceb3-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0ceb3-108">Получение соединителя</span><span class="sxs-lookup"><span data-stu-id="0ceb3-108">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="0ceb3-109">Connector</span><span class="sxs-lookup"><span data-stu-id="0ceb3-109">connector</span></span>](connector.md) |<span data-ttu-id="0ceb3-110">Чтение свойства и связи объекта соединителя.</span><span class="sxs-lookup"><span data-stu-id="0ceb3-110">Read properties and relationships of connector object.</span></span>|
|[<span data-ttu-id="0ceb3-111">Перечисление memberOf</span><span class="sxs-lookup"><span data-stu-id="0ceb3-111">List memberOf</span></span>](../api/connector-list-memberof.md) |<span data-ttu-id="0ceb3-112">[connectorGroup](connectorgroup.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="0ceb3-112">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="0ceb3-113">Получите объект connectorGroup, связанный с соединителем.</span><span class="sxs-lookup"><span data-stu-id="0ceb3-113">Get the connectorGroup object associated with the connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="0ceb3-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="0ceb3-114">Properties</span></span>
| <span data-ttu-id="0ceb3-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ceb3-115">Property</span></span>     | <span data-ttu-id="0ceb3-116">Тип</span><span class="sxs-lookup"><span data-stu-id="0ceb3-116">Type</span></span>   |<span data-ttu-id="0ceb3-117">Описание</span><span class="sxs-lookup"><span data-stu-id="0ceb3-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ceb3-118">externalIp</span><span class="sxs-lookup"><span data-stu-id="0ceb3-118">externalIp</span></span>|<span data-ttu-id="0ceb3-119">String</span><span class="sxs-lookup"><span data-stu-id="0ceb3-119">String</span></span>|<span data-ttu-id="0ceb3-120">Внешний IP-адрес как вредоносным службой для этого соединителя компьютера.</span><span class="sxs-lookup"><span data-stu-id="0ceb3-120">The external IP address as detected by the service for the connector machine.</span></span> <span data-ttu-id="0ceb3-121">Только чтение</span><span class="sxs-lookup"><span data-stu-id="0ceb3-121">Read-only</span></span>|
|<span data-ttu-id="0ceb3-122">id</span><span class="sxs-lookup"><span data-stu-id="0ceb3-122">id</span></span>|<span data-ttu-id="0ceb3-123">String</span><span class="sxs-lookup"><span data-stu-id="0ceb3-123">String</span></span>| <span data-ttu-id="0ceb3-124">Идентификатор объекта соединитель.</span><span class="sxs-lookup"><span data-stu-id="0ceb3-124">The object id of the connector.</span></span> <BR><span data-ttu-id="0ceb3-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0ceb3-125">Read-only.</span></span>|
|<span data-ttu-id="0ceb3-126">имя_компьютера</span><span class="sxs-lookup"><span data-stu-id="0ceb3-126">machineName</span></span>|<span data-ttu-id="0ceb3-127">String</span><span class="sxs-lookup"><span data-stu-id="0ceb3-127">String</span></span>| <span data-ttu-id="0ceb3-128">Имя компьютера, на котором работает соединитель.</span><span class="sxs-lookup"><span data-stu-id="0ceb3-128">The name of the machine that the connector is running on.</span></span> <BR><span data-ttu-id="0ceb3-129">Только чтение</span><span class="sxs-lookup"><span data-stu-id="0ceb3-129">Read-only</span></span>|
|<span data-ttu-id="0ceb3-130">status</span><span class="sxs-lookup"><span data-stu-id="0ceb3-130">status</span></span>|<span data-ttu-id="0ceb3-131">string</span><span class="sxs-lookup"><span data-stu-id="0ceb3-131">string</span></span>| <span data-ttu-id="0ceb3-132">Указывает состояние соединителя.</span><span class="sxs-lookup"><span data-stu-id="0ceb3-132">Indicates the status of the connector.</span></span> <span data-ttu-id="0ceb3-133">Возможные значения: `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="0ceb3-133">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="0ceb3-134">Только чтение</span><span class="sxs-lookup"><span data-stu-id="0ceb3-134">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="0ceb3-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="0ceb3-135">Relationships</span></span>
| <span data-ttu-id="0ceb3-136">Связь</span><span class="sxs-lookup"><span data-stu-id="0ceb3-136">Relationship</span></span> | <span data-ttu-id="0ceb3-137">Тип</span><span class="sxs-lookup"><span data-stu-id="0ceb3-137">Type</span></span>   |<span data-ttu-id="0ceb3-138">Описание</span><span class="sxs-lookup"><span data-stu-id="0ceb3-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ceb3-139">memberOf</span><span class="sxs-lookup"><span data-stu-id="0ceb3-139">memberOf</span></span>|<span data-ttu-id="0ceb3-140">[connectorGroup](connectorgroup.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="0ceb3-140">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="0ceb3-141">ConnectorGroup, который является членом подключиться.</span><span class="sxs-lookup"><span data-stu-id="0ceb3-141">The connectorGroup that the connect is a member of.</span></span><br><span data-ttu-id="0ceb3-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0ceb3-142">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0ceb3-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0ceb3-143">JSON representation</span></span>

<span data-ttu-id="0ceb3-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ceb3-144">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "connector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/connector.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
