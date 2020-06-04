---
title: Тип ресурса Connector
description: Представляет соединитель прокси приложения.
author: japere
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 864d76d7e6a7cb3724a91a753e5c5198e274780a
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556179"
---
# <a name="connector-resource-type"></a><span data-ttu-id="8494f-103">Тип ресурса Connector</span><span class="sxs-lookup"><span data-stu-id="8494f-103">connector resource type</span></span>

<span data-ttu-id="8494f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8494f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8494f-105">Соединители это простые агенты, которые размещаются локально и упрощают исходящее подключение к службе [прокси приложения Azure AD](https://aka.ms/whyappproxy) .</span><span class="sxs-lookup"><span data-stu-id="8494f-105">Connectors are lightweight agents that sit on-premises and facilitate the outbound connection to the [Azure AD Application Proxy](https://aka.ms/whyappproxy) service.</span></span> <span data-ttu-id="8494f-106">Каждый соединитель является частью [коннекторграуп](connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="8494f-106">Each connector is part of a [connectorGroup](connectorgroup.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8494f-107">Методы</span><span class="sxs-lookup"><span data-stu-id="8494f-107">Methods</span></span>

| <span data-ttu-id="8494f-108">Метод</span><span class="sxs-lookup"><span data-stu-id="8494f-108">Method</span></span>       | <span data-ttu-id="8494f-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8494f-109">Return Type</span></span> | <span data-ttu-id="8494f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8494f-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8494f-111">Список соединителей</span><span class="sxs-lookup"><span data-stu-id="8494f-111">List connectors</span></span>](../api/connector-list.md) | <span data-ttu-id="8494f-112">Коллекция [соединителей](connector.md)</span><span class="sxs-lookup"><span data-stu-id="8494f-112">[connector](connector.md) collection</span></span> | <span data-ttu-id="8494f-113">Получение списка объектов Connector.</span><span class="sxs-lookup"><span data-stu-id="8494f-113">Retrieve a list of connector objects.</span></span> | 
| [<span data-ttu-id="8494f-114">Получение соединителя</span><span class="sxs-lookup"><span data-stu-id="8494f-114">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="8494f-115">PDIF</span><span class="sxs-lookup"><span data-stu-id="8494f-115">connector</span></span>](connector.md) | <span data-ttu-id="8494f-116">Чтение свойств и связей объекта Connector.</span><span class="sxs-lookup"><span data-stu-id="8494f-116">Read properties and relationships of connector object.</span></span> |
| [<span data-ttu-id="8494f-117">Перечисление memberOf</span><span class="sxs-lookup"><span data-stu-id="8494f-117">List memberOf</span></span>](../api/connector-list-memberof.md) | <span data-ttu-id="8494f-118">Коллекция [коннекторграуп](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="8494f-118">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="8494f-119">Список коллекций объектов Коннекторграуп, участником которых является соединитель.</span><span class="sxs-lookup"><span data-stu-id="8494f-119">List the connectorGroup object collection the connector is a member of.</span></span> |
| [<span data-ttu-id="8494f-120">Добавление соединителя в Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="8494f-120">Add connector to connectorGroup</span></span>](../api/connector-post-memberof.md)| [<span data-ttu-id="8494f-121">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="8494f-121">connectorGroup</span></span>](connectorgroup.md) | <span data-ttu-id="8494f-122">Добавление соединителя в Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="8494f-122">Add a connector to a connectorGroup.</span></span> |


## <a name="properties"></a><span data-ttu-id="8494f-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="8494f-123">Properties</span></span>
| <span data-ttu-id="8494f-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="8494f-124">Property</span></span>     | <span data-ttu-id="8494f-125">Тип</span><span class="sxs-lookup"><span data-stu-id="8494f-125">Type</span></span>        | <span data-ttu-id="8494f-126">Описание</span><span class="sxs-lookup"><span data-stu-id="8494f-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8494f-127">екстерналип</span><span class="sxs-lookup"><span data-stu-id="8494f-127">externalIp</span></span>|<span data-ttu-id="8494f-128">String</span><span class="sxs-lookup"><span data-stu-id="8494f-128">String</span></span>| <span data-ttu-id="8494f-129">Внешний IP-адрес, обнаруженный сервером соединителей.</span><span class="sxs-lookup"><span data-stu-id="8494f-129">The external IP address as detected by the the connector server.</span></span> <span data-ttu-id="8494f-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8494f-130">Read-only.</span></span> |
|<span data-ttu-id="8494f-131">id</span><span class="sxs-lookup"><span data-stu-id="8494f-131">id</span></span>|<span data-ttu-id="8494f-132">Строка</span><span class="sxs-lookup"><span data-stu-id="8494f-132">String</span></span>| <span data-ttu-id="8494f-133">Уникальный идентификатор соединителя.</span><span class="sxs-lookup"><span data-stu-id="8494f-133">Unique identifier of the connector.</span></span> <span data-ttu-id="8494f-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8494f-134">Read-only.</span></span> |
|<span data-ttu-id="8494f-135">ИмяКомпьютера</span><span class="sxs-lookup"><span data-stu-id="8494f-135">machineName</span></span>|<span data-ttu-id="8494f-136">String</span><span class="sxs-lookup"><span data-stu-id="8494f-136">String</span></span>| <span data-ttu-id="8494f-137">Имя компьютера, на котором установлен и запущен соединитель.</span><span class="sxs-lookup"><span data-stu-id="8494f-137">The machine name the connector is installed and running on.</span></span> |
|<span data-ttu-id="8494f-138">status</span><span class="sxs-lookup"><span data-stu-id="8494f-138">status</span></span>|<span data-ttu-id="8494f-139">string</span><span class="sxs-lookup"><span data-stu-id="8494f-139">string</span></span>| <span data-ttu-id="8494f-140">Указывает состояние соединителя.</span><span class="sxs-lookup"><span data-stu-id="8494f-140">Indicates the status of the connector.</span></span> <span data-ttu-id="8494f-141">Возможные значения: `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="8494f-141">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="8494f-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8494f-142">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8494f-143">Отношения</span><span class="sxs-lookup"><span data-stu-id="8494f-143">Relationships</span></span>
| <span data-ttu-id="8494f-144">Связь</span><span class="sxs-lookup"><span data-stu-id="8494f-144">Relationship</span></span> | <span data-ttu-id="8494f-145">Тип</span><span class="sxs-lookup"><span data-stu-id="8494f-145">Type</span></span>   |<span data-ttu-id="8494f-146">Описание</span><span class="sxs-lookup"><span data-stu-id="8494f-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8494f-147">memberOf</span><span class="sxs-lookup"><span data-stu-id="8494f-147">memberOf</span></span>|<span data-ttu-id="8494f-148">Коллекция [коннекторграуп](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="8494f-148">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="8494f-149">Коннекторграуп, участником которого является соединитель.</span><span class="sxs-lookup"><span data-stu-id="8494f-149">The connectorGroup that the connector is a member of.</span></span> <span data-ttu-id="8494f-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8494f-150">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8494f-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8494f-151">JSON representation</span></span>

<span data-ttu-id="8494f-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8494f-152">The following is a JSON representation of the resource.</span></span>

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
