---
title: Тип ресурса Connector
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 25d350e48aaddbda2b931ae5a9e177ec6caa9799
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507480"
---
# <a name="connector-resource-type"></a><span data-ttu-id="c74e8-103">Тип ресурса Connector</span><span class="sxs-lookup"><span data-stu-id="c74e8-103">connector resource type</span></span>

<span data-ttu-id="c74e8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c74e8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a><span data-ttu-id="c74e8-105">Методы</span><span class="sxs-lookup"><span data-stu-id="c74e8-105">Methods</span></span>

| <span data-ttu-id="c74e8-106">Метод</span><span class="sxs-lookup"><span data-stu-id="c74e8-106">Method</span></span>           | <span data-ttu-id="c74e8-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c74e8-107">Return Type</span></span>    |<span data-ttu-id="c74e8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c74e8-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c74e8-109">Получение соединителя</span><span class="sxs-lookup"><span data-stu-id="c74e8-109">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="c74e8-110">PDIF</span><span class="sxs-lookup"><span data-stu-id="c74e8-110">connector</span></span>](connector.md) |<span data-ttu-id="c74e8-111">Чтение свойств и связей объекта Connector.</span><span class="sxs-lookup"><span data-stu-id="c74e8-111">Read properties and relationships of connector object.</span></span>|
|[<span data-ttu-id="c74e8-112">Перечисление memberOf</span><span class="sxs-lookup"><span data-stu-id="c74e8-112">List memberOf</span></span>](../api/connector-list-memberof.md) |<span data-ttu-id="c74e8-113">Коллекция [коннекторграуп](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="c74e8-113">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="c74e8-114">Получение объекта Коннекторграуп, связанного с соединителем.</span><span class="sxs-lookup"><span data-stu-id="c74e8-114">Get the connectorGroup object associated with the connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="c74e8-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="c74e8-115">Properties</span></span>
| <span data-ttu-id="c74e8-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="c74e8-116">Property</span></span>     | <span data-ttu-id="c74e8-117">Тип</span><span class="sxs-lookup"><span data-stu-id="c74e8-117">Type</span></span>   |<span data-ttu-id="c74e8-118">Описание</span><span class="sxs-lookup"><span data-stu-id="c74e8-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c74e8-119">екстерналип</span><span class="sxs-lookup"><span data-stu-id="c74e8-119">externalIp</span></span>|<span data-ttu-id="c74e8-120">String</span><span class="sxs-lookup"><span data-stu-id="c74e8-120">String</span></span>|<span data-ttu-id="c74e8-121">Внешний IP-адрес, обнаруженный службой для соединителного компьютера.</span><span class="sxs-lookup"><span data-stu-id="c74e8-121">The external IP address as detected by the service for the connector machine.</span></span> <span data-ttu-id="c74e8-122">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="c74e8-122">Read-only</span></span>|
|<span data-ttu-id="c74e8-123">id</span><span class="sxs-lookup"><span data-stu-id="c74e8-123">id</span></span>|<span data-ttu-id="c74e8-124">Строка</span><span class="sxs-lookup"><span data-stu-id="c74e8-124">String</span></span>| <span data-ttu-id="c74e8-125">Идентификатор объекта Connector.</span><span class="sxs-lookup"><span data-stu-id="c74e8-125">The object id of the connector.</span></span> <BR><span data-ttu-id="c74e8-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c74e8-126">Read-only.</span></span>|
|<span data-ttu-id="c74e8-127">ИмяКомпьютера</span><span class="sxs-lookup"><span data-stu-id="c74e8-127">machineName</span></span>|<span data-ttu-id="c74e8-128">String</span><span class="sxs-lookup"><span data-stu-id="c74e8-128">String</span></span>| <span data-ttu-id="c74e8-129">Имя компьютера, на котором работает соединитель.</span><span class="sxs-lookup"><span data-stu-id="c74e8-129">The name of the machine that the connector is running on.</span></span> <BR><span data-ttu-id="c74e8-130">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="c74e8-130">Read-only</span></span>|
|<span data-ttu-id="c74e8-131">status</span><span class="sxs-lookup"><span data-stu-id="c74e8-131">status</span></span>|<span data-ttu-id="c74e8-132">string</span><span class="sxs-lookup"><span data-stu-id="c74e8-132">string</span></span>| <span data-ttu-id="c74e8-133">Указывает состояние соединителя.</span><span class="sxs-lookup"><span data-stu-id="c74e8-133">Indicates the status of the connector.</span></span> <span data-ttu-id="c74e8-134">Возможные значения: `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="c74e8-134">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="c74e8-135">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="c74e8-135">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="c74e8-136">Связи</span><span class="sxs-lookup"><span data-stu-id="c74e8-136">Relationships</span></span>
| <span data-ttu-id="c74e8-137">Связь</span><span class="sxs-lookup"><span data-stu-id="c74e8-137">Relationship</span></span> | <span data-ttu-id="c74e8-138">Тип</span><span class="sxs-lookup"><span data-stu-id="c74e8-138">Type</span></span>   |<span data-ttu-id="c74e8-139">Описание</span><span class="sxs-lookup"><span data-stu-id="c74e8-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c74e8-140">memberOf</span><span class="sxs-lookup"><span data-stu-id="c74e8-140">memberOf</span></span>|<span data-ttu-id="c74e8-141">Коллекция [коннекторграуп](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="c74e8-141">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="c74e8-142">Коннекторграуп, участником которого является подключение.</span><span class="sxs-lookup"><span data-stu-id="c74e8-142">The connectorGroup that the connect is a member of.</span></span><br><span data-ttu-id="c74e8-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c74e8-143">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c74e8-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c74e8-144">JSON representation</span></span>

<span data-ttu-id="c74e8-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c74e8-145">Here is a JSON representation of the resource.</span></span>

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
