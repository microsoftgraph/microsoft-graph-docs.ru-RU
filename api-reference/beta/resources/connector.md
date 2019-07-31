---
title: Тип ресурса Connector
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ec4d3fdb415533d5b3f2effc72688fe912551bc8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012879"
---
# <a name="connector-resource-type"></a><span data-ttu-id="16dd4-103">Тип ресурса Connector</span><span class="sxs-lookup"><span data-stu-id="16dd4-103">connector resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a><span data-ttu-id="16dd4-104">Методы</span><span class="sxs-lookup"><span data-stu-id="16dd4-104">Methods</span></span>

| <span data-ttu-id="16dd4-105">Метод</span><span class="sxs-lookup"><span data-stu-id="16dd4-105">Method</span></span>           | <span data-ttu-id="16dd4-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="16dd4-106">Return Type</span></span>    |<span data-ttu-id="16dd4-107">Описание</span><span class="sxs-lookup"><span data-stu-id="16dd4-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="16dd4-108">Получение соединителя</span><span class="sxs-lookup"><span data-stu-id="16dd4-108">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="16dd4-109">PDIF</span><span class="sxs-lookup"><span data-stu-id="16dd4-109">connector</span></span>](connector.md) |<span data-ttu-id="16dd4-110">Чтение свойств и связей объекта Connector.</span><span class="sxs-lookup"><span data-stu-id="16dd4-110">Read properties and relationships of connector object.</span></span>|
|[<span data-ttu-id="16dd4-111">Перечисление memberOf</span><span class="sxs-lookup"><span data-stu-id="16dd4-111">List memberOf</span></span>](../api/connector-list-memberof.md) |<span data-ttu-id="16dd4-112">Коллекция [коннекторграуп](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="16dd4-112">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="16dd4-113">Получение объекта Коннекторграуп, связанного с соединителем.</span><span class="sxs-lookup"><span data-stu-id="16dd4-113">Get the connectorGroup object associated with the connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="16dd4-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="16dd4-114">Properties</span></span>
| <span data-ttu-id="16dd4-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="16dd4-115">Property</span></span>     | <span data-ttu-id="16dd4-116">Тип</span><span class="sxs-lookup"><span data-stu-id="16dd4-116">Type</span></span>   |<span data-ttu-id="16dd4-117">Описание</span><span class="sxs-lookup"><span data-stu-id="16dd4-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16dd4-118">Екстерналип</span><span class="sxs-lookup"><span data-stu-id="16dd4-118">externalIp</span></span>|<span data-ttu-id="16dd4-119">String</span><span class="sxs-lookup"><span data-stu-id="16dd4-119">String</span></span>|<span data-ttu-id="16dd4-120">Внешний IP-адрес, обнаруженный службой для соединителного компьютера.</span><span class="sxs-lookup"><span data-stu-id="16dd4-120">The external IP address as detected by the service for the connector machine.</span></span> <span data-ttu-id="16dd4-121">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="16dd4-121">Read-only</span></span>|
|<span data-ttu-id="16dd4-122">id</span><span class="sxs-lookup"><span data-stu-id="16dd4-122">id</span></span>|<span data-ttu-id="16dd4-123">Строка</span><span class="sxs-lookup"><span data-stu-id="16dd4-123">String</span></span>| <span data-ttu-id="16dd4-124">Идентификатор объекта Connector.</span><span class="sxs-lookup"><span data-stu-id="16dd4-124">The object id of the connector.</span></span> <BR><span data-ttu-id="16dd4-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="16dd4-125">Read-only.</span></span>|
|<span data-ttu-id="16dd4-126">ИмяКомпьютера</span><span class="sxs-lookup"><span data-stu-id="16dd4-126">machineName</span></span>|<span data-ttu-id="16dd4-127">String</span><span class="sxs-lookup"><span data-stu-id="16dd4-127">String</span></span>| <span data-ttu-id="16dd4-128">Имя компьютера, на котором работает соединитель.</span><span class="sxs-lookup"><span data-stu-id="16dd4-128">The name of the machine that the connector is running on.</span></span> <BR><span data-ttu-id="16dd4-129">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="16dd4-129">Read-only</span></span>|
|<span data-ttu-id="16dd4-130">status</span><span class="sxs-lookup"><span data-stu-id="16dd4-130">status</span></span>|<span data-ttu-id="16dd4-131">string</span><span class="sxs-lookup"><span data-stu-id="16dd4-131">string</span></span>| <span data-ttu-id="16dd4-132">Указывает состояние соединителя.</span><span class="sxs-lookup"><span data-stu-id="16dd4-132">Indicates the status of the connector.</span></span> <span data-ttu-id="16dd4-133">Возможные значения: `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="16dd4-133">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="16dd4-134">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="16dd4-134">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="16dd4-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="16dd4-135">Relationships</span></span>
| <span data-ttu-id="16dd4-136">Отношение</span><span class="sxs-lookup"><span data-stu-id="16dd4-136">Relationship</span></span> | <span data-ttu-id="16dd4-137">Тип</span><span class="sxs-lookup"><span data-stu-id="16dd4-137">Type</span></span>   |<span data-ttu-id="16dd4-138">Описание</span><span class="sxs-lookup"><span data-stu-id="16dd4-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16dd4-139">memberOf</span><span class="sxs-lookup"><span data-stu-id="16dd4-139">memberOf</span></span>|<span data-ttu-id="16dd4-140">Коллекция [коннекторграуп](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="16dd4-140">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="16dd4-141">Коннекторграуп, участником которого является подключение.</span><span class="sxs-lookup"><span data-stu-id="16dd4-141">The connectorGroup that the connect is a member of.</span></span><br><span data-ttu-id="16dd4-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="16dd4-142">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="16dd4-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="16dd4-143">JSON representation</span></span>

<span data-ttu-id="16dd4-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16dd4-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
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
  "suppressions": []
}
-->
