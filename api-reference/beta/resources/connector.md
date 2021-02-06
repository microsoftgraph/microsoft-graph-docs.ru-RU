---
title: Тип ресурса connector
description: Представляет соединители прокси приложения.
author: japere
localization_priority: Normal
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 53a5726456ce3d03ea537e87ec0dddb901623601
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136781"
---
# <a name="connector-resource-type"></a><span data-ttu-id="5ea61-103">Тип ресурса connector</span><span class="sxs-lookup"><span data-stu-id="5ea61-103">connector resource type</span></span>

<span data-ttu-id="5ea61-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ea61-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ea61-105">Соединители — это облегченные агенты, которые находятся локально и облегчают исходящие подключения к службе прокси приложения [Azure AD.](https://aka.ms/whyappproxy)</span><span class="sxs-lookup"><span data-stu-id="5ea61-105">Connectors are lightweight agents that sit on-premises and facilitate the outbound connection to the [Azure AD Application Proxy](https://aka.ms/whyappproxy) service.</span></span> <span data-ttu-id="5ea61-106">Каждый соединители являются частью [connectorGroup.](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="5ea61-106">Each connector is part of a [connectorGroup](connectorgroup.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5ea61-107">Методы</span><span class="sxs-lookup"><span data-stu-id="5ea61-107">Methods</span></span>

| <span data-ttu-id="5ea61-108">Метод</span><span class="sxs-lookup"><span data-stu-id="5ea61-108">Method</span></span>       | <span data-ttu-id="5ea61-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5ea61-109">Return Type</span></span> | <span data-ttu-id="5ea61-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5ea61-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5ea61-111">Перечисление соединителей</span><span class="sxs-lookup"><span data-stu-id="5ea61-111">List connectors</span></span>](../api/connector-list.md) | <span data-ttu-id="5ea61-112">[коллекция соединители](connector.md)</span><span class="sxs-lookup"><span data-stu-id="5ea61-112">[connector](connector.md) collection</span></span> | <span data-ttu-id="5ea61-113">Получить список объектов соединители.</span><span class="sxs-lookup"><span data-stu-id="5ea61-113">Retrieve a list of connector objects.</span></span> | 
| [<span data-ttu-id="5ea61-114">Получение соединителя</span><span class="sxs-lookup"><span data-stu-id="5ea61-114">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="5ea61-115">connector</span><span class="sxs-lookup"><span data-stu-id="5ea61-115">connector</span></span>](connector.md) | <span data-ttu-id="5ea61-116">Чтение свойств и связей объекта соединители.</span><span class="sxs-lookup"><span data-stu-id="5ea61-116">Read properties and relationships of connector object.</span></span> |
| [<span data-ttu-id="5ea61-117">Перечисление memberOf</span><span class="sxs-lookup"><span data-stu-id="5ea61-117">List memberOf</span></span>](../api/connector-list-memberof.md) | <span data-ttu-id="5ea61-118">[Коллекция connectorGroup](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="5ea61-118">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="5ea61-119">Укажете коллекцию объектов connectorGroup, участником группы.</span><span class="sxs-lookup"><span data-stu-id="5ea61-119">List the connectorGroup object collection the connector is a member of.</span></span> |
| [<span data-ttu-id="5ea61-120">Добавление соединителя для connectorGroup</span><span class="sxs-lookup"><span data-stu-id="5ea61-120">Add connector to connectorGroup</span></span>](../api/connector-post-memberof.md)| [<span data-ttu-id="5ea61-121">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="5ea61-121">connectorGroup</span></span>](connectorgroup.md) | <span data-ttu-id="5ea61-122">Добавление соединителю в connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="5ea61-122">Add a connector to a connectorGroup.</span></span> |


## <a name="properties"></a><span data-ttu-id="5ea61-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="5ea61-123">Properties</span></span>
| <span data-ttu-id="5ea61-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ea61-124">Property</span></span>     | <span data-ttu-id="5ea61-125">Тип</span><span class="sxs-lookup"><span data-stu-id="5ea61-125">Type</span></span>        | <span data-ttu-id="5ea61-126">Описание</span><span class="sxs-lookup"><span data-stu-id="5ea61-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5ea61-127">externalIp</span><span class="sxs-lookup"><span data-stu-id="5ea61-127">externalIp</span></span>|<span data-ttu-id="5ea61-128">Строка</span><span class="sxs-lookup"><span data-stu-id="5ea61-128">String</span></span>| <span data-ttu-id="5ea61-129">Внешний IP-адрес, обнаруженный сервером соединители.</span><span class="sxs-lookup"><span data-stu-id="5ea61-129">The external IP address as detected by the the connector server.</span></span> <span data-ttu-id="5ea61-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5ea61-130">Read-only.</span></span> |
|<span data-ttu-id="5ea61-131">id</span><span class="sxs-lookup"><span data-stu-id="5ea61-131">id</span></span>|<span data-ttu-id="5ea61-132">Строка</span><span class="sxs-lookup"><span data-stu-id="5ea61-132">String</span></span>| <span data-ttu-id="5ea61-133">Уникальный идентификатор соединители.</span><span class="sxs-lookup"><span data-stu-id="5ea61-133">Unique identifier of the connector.</span></span> <span data-ttu-id="5ea61-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5ea61-134">Read-only.</span></span> |
|<span data-ttu-id="5ea61-135">machineName</span><span class="sxs-lookup"><span data-stu-id="5ea61-135">machineName</span></span>|<span data-ttu-id="5ea61-136">Строка</span><span class="sxs-lookup"><span data-stu-id="5ea61-136">String</span></span>| <span data-ttu-id="5ea61-137">Имя компьютера, на который установлен и запущен соедините.</span><span class="sxs-lookup"><span data-stu-id="5ea61-137">The machine name the connector is installed and running on.</span></span> |
|<span data-ttu-id="5ea61-138">status</span><span class="sxs-lookup"><span data-stu-id="5ea61-138">status</span></span>|<span data-ttu-id="5ea61-139">string</span><span class="sxs-lookup"><span data-stu-id="5ea61-139">string</span></span>| <span data-ttu-id="5ea61-140">Указывает состояние соединители.</span><span class="sxs-lookup"><span data-stu-id="5ea61-140">Indicates the status of the connector.</span></span> <span data-ttu-id="5ea61-141">Возможные значения: `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="5ea61-141">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="5ea61-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5ea61-142">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5ea61-143">Связи</span><span class="sxs-lookup"><span data-stu-id="5ea61-143">Relationships</span></span>
| <span data-ttu-id="5ea61-144">Связь</span><span class="sxs-lookup"><span data-stu-id="5ea61-144">Relationship</span></span> | <span data-ttu-id="5ea61-145">Тип</span><span class="sxs-lookup"><span data-stu-id="5ea61-145">Type</span></span>   |<span data-ttu-id="5ea61-146">Описание</span><span class="sxs-lookup"><span data-stu-id="5ea61-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ea61-147">memberOf</span><span class="sxs-lookup"><span data-stu-id="5ea61-147">memberOf</span></span>|<span data-ttu-id="5ea61-148">[Коллекция connectorGroup](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="5ea61-148">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="5ea61-149">СоединителиГруппы, в которые входит соединитестройка.</span><span class="sxs-lookup"><span data-stu-id="5ea61-149">The connectorGroup that the connector is a member of.</span></span> <span data-ttu-id="5ea61-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5ea61-150">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5ea61-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5ea61-151">JSON representation</span></span>

<span data-ttu-id="5ea61-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ea61-152">The following is a JSON representation of the resource.</span></span>

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



