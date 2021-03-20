---
title: тип ресурса соединитетеля
description: Представляет соединители прокси-сервер приложений.
author: japere
localization_priority: Normal
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 567b67576c5300419c9671de8bd82df84bf49685
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945699"
---
# <a name="connector-resource-type"></a><span data-ttu-id="ed9e7-103">тип ресурса соединитетеля</span><span class="sxs-lookup"><span data-stu-id="ed9e7-103">connector resource type</span></span>

<span data-ttu-id="ed9e7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed9e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed9e7-105">Соединители — это легкие агенты, которые находятся на месте и облегчают исходящие подключения к прокси-службе [приложения Azure AD.](https://aka.ms/whyappproxy)</span><span class="sxs-lookup"><span data-stu-id="ed9e7-105">Connectors are lightweight agents that sit on-premises and facilitate the outbound connection to the [Azure AD Application Proxy](https://aka.ms/whyappproxy) service.</span></span> <span data-ttu-id="ed9e7-106">Каждый соединитектор является частью [соединителиГруп](connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="ed9e7-106">Each connector is part of a [connectorGroup](connectorgroup.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ed9e7-107">Методы</span><span class="sxs-lookup"><span data-stu-id="ed9e7-107">Methods</span></span>

| <span data-ttu-id="ed9e7-108">Метод</span><span class="sxs-lookup"><span data-stu-id="ed9e7-108">Method</span></span>       | <span data-ttu-id="ed9e7-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ed9e7-109">Return Type</span></span> | <span data-ttu-id="ed9e7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ed9e7-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ed9e7-111">Перечисление соединителей</span><span class="sxs-lookup"><span data-stu-id="ed9e7-111">List connectors</span></span>](../api/connector-list.md) | <span data-ttu-id="ed9e7-112">[коллекция соединители](connector.md)</span><span class="sxs-lookup"><span data-stu-id="ed9e7-112">[connector](connector.md) collection</span></span> | <span data-ttu-id="ed9e7-113">Извлечение списка объектов соединители.</span><span class="sxs-lookup"><span data-stu-id="ed9e7-113">Retrieve a list of connector objects.</span></span> | 
| [<span data-ttu-id="ed9e7-114">Получение соединителя</span><span class="sxs-lookup"><span data-stu-id="ed9e7-114">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="ed9e7-115">connector</span><span class="sxs-lookup"><span data-stu-id="ed9e7-115">connector</span></span>](connector.md) | <span data-ttu-id="ed9e7-116">Чтение свойств и связей соединитеного объекта.</span><span class="sxs-lookup"><span data-stu-id="ed9e7-116">Read properties and relationships of connector object.</span></span> |
| [<span data-ttu-id="ed9e7-117">Перечисление memberOf</span><span class="sxs-lookup"><span data-stu-id="ed9e7-117">List memberOf</span></span>](../api/connector-list-memberof.md) | <span data-ttu-id="ed9e7-118">[коллекция connectorGroup](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="ed9e7-118">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="ed9e7-119">Укажете коллекцию объектов connectorGroup, членом в которая является соедините.</span><span class="sxs-lookup"><span data-stu-id="ed9e7-119">List the connectorGroup object collection the connector is a member of.</span></span> |
| [<span data-ttu-id="ed9e7-120">Добавление соединителя для connectorGroup</span><span class="sxs-lookup"><span data-stu-id="ed9e7-120">Add connector to connectorGroup</span></span>](../api/connector-post-memberof.md)| [<span data-ttu-id="ed9e7-121">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="ed9e7-121">connectorGroup</span></span>](connectorgroup.md) | <span data-ttu-id="ed9e7-122">Добавьте соединителю в соединителюGroup.</span><span class="sxs-lookup"><span data-stu-id="ed9e7-122">Add a connector to a connectorGroup.</span></span> |


## <a name="properties"></a><span data-ttu-id="ed9e7-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="ed9e7-123">Properties</span></span>
| <span data-ttu-id="ed9e7-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed9e7-124">Property</span></span>     | <span data-ttu-id="ed9e7-125">Тип</span><span class="sxs-lookup"><span data-stu-id="ed9e7-125">Type</span></span>        | <span data-ttu-id="ed9e7-126">Описание</span><span class="sxs-lookup"><span data-stu-id="ed9e7-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ed9e7-127">externalIp</span><span class="sxs-lookup"><span data-stu-id="ed9e7-127">externalIp</span></span>|<span data-ttu-id="ed9e7-128">Строка</span><span class="sxs-lookup"><span data-stu-id="ed9e7-128">String</span></span>| <span data-ttu-id="ed9e7-129">Внешний IP-адрес, обнаруженный сервером соединители.</span><span class="sxs-lookup"><span data-stu-id="ed9e7-129">The external IP address as detected by the the connector server.</span></span> <span data-ttu-id="ed9e7-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ed9e7-130">Read-only.</span></span> |
|<span data-ttu-id="ed9e7-131">id</span><span class="sxs-lookup"><span data-stu-id="ed9e7-131">id</span></span>|<span data-ttu-id="ed9e7-132">Строка</span><span class="sxs-lookup"><span data-stu-id="ed9e7-132">String</span></span>| <span data-ttu-id="ed9e7-133">Уникальный идентификатор соединитетеля.</span><span class="sxs-lookup"><span data-stu-id="ed9e7-133">Unique identifier of the connector.</span></span> <span data-ttu-id="ed9e7-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ed9e7-134">Read-only.</span></span> |
|<span data-ttu-id="ed9e7-135">machineName</span><span class="sxs-lookup"><span data-stu-id="ed9e7-135">machineName</span></span>|<span data-ttu-id="ed9e7-136">Строка</span><span class="sxs-lookup"><span data-stu-id="ed9e7-136">String</span></span>| <span data-ttu-id="ed9e7-137">Имя машины, на которое установлен соединитатель, и запущено.</span><span class="sxs-lookup"><span data-stu-id="ed9e7-137">The machine name the connector is installed and running on.</span></span> |
|<span data-ttu-id="ed9e7-138">status</span><span class="sxs-lookup"><span data-stu-id="ed9e7-138">status</span></span>|<span data-ttu-id="ed9e7-139">connectorStatus</span><span class="sxs-lookup"><span data-stu-id="ed9e7-139">connectorStatus</span></span>| <span data-ttu-id="ed9e7-140">Указывает состояние соединитетеля.</span><span class="sxs-lookup"><span data-stu-id="ed9e7-140">Indicates the status of the connector.</span></span> <span data-ttu-id="ed9e7-141">Возможные значения: `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="ed9e7-141">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="ed9e7-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ed9e7-142">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ed9e7-143">Связи</span><span class="sxs-lookup"><span data-stu-id="ed9e7-143">Relationships</span></span>
| <span data-ttu-id="ed9e7-144">Связь</span><span class="sxs-lookup"><span data-stu-id="ed9e7-144">Relationship</span></span> | <span data-ttu-id="ed9e7-145">Тип</span><span class="sxs-lookup"><span data-stu-id="ed9e7-145">Type</span></span>   |<span data-ttu-id="ed9e7-146">Описание</span><span class="sxs-lookup"><span data-stu-id="ed9e7-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed9e7-147">memberOf</span><span class="sxs-lookup"><span data-stu-id="ed9e7-147">memberOf</span></span>|<span data-ttu-id="ed9e7-148">[коллекция connectorGroup](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="ed9e7-148">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="ed9e7-149">СоединитекторGroup, членом который является соединитектор.</span><span class="sxs-lookup"><span data-stu-id="ed9e7-149">The connectorGroup that the connector is a member of.</span></span> <span data-ttu-id="ed9e7-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ed9e7-150">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ed9e7-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ed9e7-151">JSON representation</span></span>

<span data-ttu-id="ed9e7-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed9e7-152">The following is a JSON representation of the resource.</span></span>

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



