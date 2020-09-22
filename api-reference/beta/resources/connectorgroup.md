---
title: Тип ресурса Коннекторграуп
description: Представляет прокси приложения Коннекторграуп.
localization_priority: Normal
ms.prod: microsoft-identity-platform
author: japere
doc_type: resourcePageType
ms.openlocfilehash: ec56137fab8a929ae3823dcdd339ea6e3b8e174b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027148"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="5c147-103">Тип ресурса Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="5c147-103">connectorGroup resource type</span></span>

<span data-ttu-id="5c147-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c147-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c147-105">Каждый соединитель [прокси приложения Azure AD](https://aka.ms/whyappproxy) всегда является частью группы соединителей.</span><span class="sxs-lookup"><span data-stu-id="5c147-105">Each [Azure AD Application Proxy](https://aka.ms/whyappproxy) connector is always part of a connector group.</span></span> <span data-ttu-id="5c147-106">Все соединители, принадлежащие одной и той же группе соединителей, действуют как отдельные единицы для обеспечения высокого уровня доступности и балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="5c147-106">All the connectors that belong to the same connector group act as a separate unit for high-availability and load balancing.</span></span> <span data-ttu-id="5c147-107">Если вы не создадите группы соединителей, все соединители будут входить в группу по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5c147-107">If you don't create connector groups, all your connectors will be part of the default group.</span></span> <span data-ttu-id="5c147-108">При настройке приложения с помощью прокси для приложения также необходимо указать группу соединителей, которой необходимо назначить приложение.</span><span class="sxs-lookup"><span data-stu-id="5c147-108">When configuring an application with Application Proxy, you must also specify which connector group to assign the application to.</span></span>

<span data-ttu-id="5c147-109">После создания группы соединителей можно добавить или переместить соединители в группу соединителей с помощью [Add Connector](../api/connectorgroup-post-members.md).</span><span class="sxs-lookup"><span data-stu-id="5c147-109">After a connector group is created, you can add or move connectors to the connector group by using [Add connector](../api/connectorgroup-post-members.md).</span></span> <span data-ttu-id="5c147-110">Вы также можете использовать [Add Application](../api/connectorgroup-post-applications.md) , чтобы назначить приложение для группы соединителей.</span><span class="sxs-lookup"><span data-stu-id="5c147-110">You can also use [Add application](../api/connectorgroup-post-applications.md) to assign an application to a connector group.</span></span>

## <a name="methods"></a><span data-ttu-id="5c147-111">Методы</span><span class="sxs-lookup"><span data-stu-id="5c147-111">Methods</span></span>

| <span data-ttu-id="5c147-112">Метод</span><span class="sxs-lookup"><span data-stu-id="5c147-112">Method</span></span>           | <span data-ttu-id="5c147-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5c147-113">Return Type</span></span>    |<span data-ttu-id="5c147-114">Описание</span><span class="sxs-lookup"><span data-stu-id="5c147-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5c147-115">Список Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="5c147-115">List connectorGroup</span></span>](../api/connectorgroup-list.md) |<span data-ttu-id="5c147-116">Коллекция [коннекторграуп](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="5c147-116">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="5c147-117">Получение списка объектов Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="5c147-117">Retrieve a list of connectorGroup objects.</span></span> |
|[<span data-ttu-id="5c147-118">Создание connectorGroup</span><span class="sxs-lookup"><span data-stu-id="5c147-118">Create connectorGroup</span></span>](../api/connectorgroup-post.md) |<span data-ttu-id="5c147-119">Коллекция [коннекторграуп](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="5c147-119">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="5c147-120">Создание объекта Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="5c147-120">Create a connectorGroup object.</span></span> |
|[<span data-ttu-id="5c147-121">Получение connectorGroup</span><span class="sxs-lookup"><span data-stu-id="5c147-121">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="5c147-122">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="5c147-122">connectorGroup</span></span>](connectorgroup.md) | <span data-ttu-id="5c147-123">Чтение свойств и связей объекта Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="5c147-123">Read properties and relationships of a connectorGroup object.</span></span> |
|[<span data-ttu-id="5c147-124">Обновление connectorGroup</span><span class="sxs-lookup"><span data-stu-id="5c147-124">Update connectorGroup</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="5c147-125">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="5c147-125">connectorGroup</span></span>](connectorgroup.md)| <span data-ttu-id="5c147-126">Обновление объекта Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="5c147-126">Update a connectorGroup object.</span></span> |
|[<span data-ttu-id="5c147-127">Удаление connectorGroup</span><span class="sxs-lookup"><span data-stu-id="5c147-127">Delete connectorGroup</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="5c147-128">Нет</span><span class="sxs-lookup"><span data-stu-id="5c147-128">None</span></span> | <span data-ttu-id="5c147-129">Удаление объекта Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="5c147-129">Delete a connectorGroup object.</span></span> <span data-ttu-id="5c147-130">Прежде чем Коннекторграуп можно будет удалить, необходимо удалить все соединители из Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="5c147-130">All connectors must be removed from the connectorGroup before a connectorGroup can be deleted.</span></span> |
|[<span data-ttu-id="5c147-131">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="5c147-131">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="5c147-132">Коллекция [соединителей](connector.md)</span><span class="sxs-lookup"><span data-stu-id="5c147-132">[connector](connector.md) collection</span></span>| <span data-ttu-id="5c147-133">Получение коллекции объектов Connector.</span><span class="sxs-lookup"><span data-stu-id="5c147-133">Get a connector object collection.</span></span> |
|[<span data-ttu-id="5c147-134">Перечисление приложений</span><span class="sxs-lookup"><span data-stu-id="5c147-134">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="5c147-135">Коллекция [application](application.md)</span><span class="sxs-lookup"><span data-stu-id="5c147-135">[application](application.md) collection</span></span>| <span data-ttu-id="5c147-136">Получение коллекции объектов Application, связанной с Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="5c147-136">Get the application object collection associated with the connectorGroup.</span></span> |
|[<span data-ttu-id="5c147-137">Добавление приложения</span><span class="sxs-lookup"><span data-stu-id="5c147-137">Add application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="5c147-138">application</span><span class="sxs-lookup"><span data-stu-id="5c147-138">application</span></span>](application.md)| <span data-ttu-id="5c147-139">Свяжите приложение с Коннекторграуп, размещая в коллекции Applications.</span><span class="sxs-lookup"><span data-stu-id="5c147-139">Associate an application with the connectorGroup by posting to the applications collection.</span></span> |
|[<span data-ttu-id="5c147-140">Добавление соединителя</span><span class="sxs-lookup"><span data-stu-id="5c147-140">Add connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="5c147-141">PDIF</span><span class="sxs-lookup"><span data-stu-id="5c147-141">connector</span></span>](connector.md)| <span data-ttu-id="5c147-142">Добавление соединителя в Коннекторграуп путем публикации в коллекции Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="5c147-142">Add a connector to the connectorGroup by posting to the connectorGroup collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="5c147-143">Свойства</span><span class="sxs-lookup"><span data-stu-id="5c147-143">Properties</span></span>
| <span data-ttu-id="5c147-144">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c147-144">Property</span></span>     | <span data-ttu-id="5c147-145">Тип</span><span class="sxs-lookup"><span data-stu-id="5c147-145">Type</span></span>   |<span data-ttu-id="5c147-146">Описание</span><span class="sxs-lookup"><span data-stu-id="5c147-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c147-147">коннекторграуптипе</span><span class="sxs-lookup"><span data-stu-id="5c147-147">connectorGroupType</span></span>|<span data-ttu-id="5c147-148">string</span><span class="sxs-lookup"><span data-stu-id="5c147-148">string</span></span>| <span data-ttu-id="5c147-149">Указывает тип гибридного агента.</span><span class="sxs-lookup"><span data-stu-id="5c147-149">Indicates the type of hybrid agent.</span></span> <span data-ttu-id="5c147-150">Это предварительно заданное системой.</span><span class="sxs-lookup"><span data-stu-id="5c147-150">This pre-set by the system.</span></span> <span data-ttu-id="5c147-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5c147-151">Read-only.</span></span> |
|<span data-ttu-id="5c147-152">id</span><span class="sxs-lookup"><span data-stu-id="5c147-152">id</span></span>|<span data-ttu-id="5c147-153">string</span><span class="sxs-lookup"><span data-stu-id="5c147-153">string</span></span>| <span data-ttu-id="5c147-154">Уникальный идентификатор для этого Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="5c147-154">Unique identifier for this connectorGroup.</span></span> <span data-ttu-id="5c147-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5c147-155">Read-only.</span></span> |
|<span data-ttu-id="5c147-156">isDefault</span><span class="sxs-lookup"><span data-stu-id="5c147-156">isDefault</span></span>|<span data-ttu-id="5c147-157">boolean</span><span class="sxs-lookup"><span data-stu-id="5c147-157">boolean</span></span>| <span data-ttu-id="5c147-158">Указывает, является ли Коннекторграуп Коннекторграуп по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5c147-158">Indicates if the connectorGroup is the default connectorGroup.</span></span> <span data-ttu-id="5c147-159">Только одна группа соединителей может быть Коннекторграуп по умолчанию, и она предопределена системой.</span><span class="sxs-lookup"><span data-stu-id="5c147-159">Only a single connector group can be the default connectorGroup and this is pre-set by the system.</span></span> <span data-ttu-id="5c147-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5c147-160">Read-only.</span></span> |
|<span data-ttu-id="5c147-161">name</span><span class="sxs-lookup"><span data-stu-id="5c147-161">name</span></span>|<span data-ttu-id="5c147-162">string</span><span class="sxs-lookup"><span data-stu-id="5c147-162">string</span></span>| <span data-ttu-id="5c147-163">Имя, связанное с Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="5c147-163">The name associated with the connectorGroup.</span></span> |
|<span data-ttu-id="5c147-164">региональных</span><span class="sxs-lookup"><span data-stu-id="5c147-164">region</span></span>|<span data-ttu-id="5c147-165">string</span><span class="sxs-lookup"><span data-stu-id="5c147-165">string</span></span>| <span data-ttu-id="5c147-166">Регион, которому назначена Коннекторграуп, и который оптимизирует трафик для.</span><span class="sxs-lookup"><span data-stu-id="5c147-166">The region the connectorGroup is assigned to and will optimize traffic for.</span></span> <span data-ttu-id="5c147-167">Эту область можно задать только в том случае, если Коннекторграуп **не назначен ни один из соединителей или приложений** .</span><span class="sxs-lookup"><span data-stu-id="5c147-167">This region can only be set if **no connectors or applications** are assigned to the connectorGroup.</span></span> <span data-ttu-id="5c147-168">Доступны следующие регионы: Северная Америка, Европа, Австралия, Азия и Индии.</span><span class="sxs-lookup"><span data-stu-id="5c147-168">The regions available include: North America, Europe, Australia, Asia, and India.</span></span> <span data-ttu-id="5c147-169">Возможные значения: `nam`, `eur`, `aus`, `asia`, `ind`.</span><span class="sxs-lookup"><span data-stu-id="5c147-169">Possible values are: `nam`, `eur`, `aus`, `asia`, `ind`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c147-170">Отношения</span><span class="sxs-lookup"><span data-stu-id="5c147-170">Relationships</span></span>
| <span data-ttu-id="5c147-171">Связь</span><span class="sxs-lookup"><span data-stu-id="5c147-171">Relationship</span></span> | <span data-ttu-id="5c147-172">Тип</span><span class="sxs-lookup"><span data-stu-id="5c147-172">Type</span></span>   |<span data-ttu-id="5c147-173">Описание</span><span class="sxs-lookup"><span data-stu-id="5c147-173">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c147-174">заявлен</span><span class="sxs-lookup"><span data-stu-id="5c147-174">applications</span></span>|<span data-ttu-id="5c147-175">Коллекция [application](application.md)</span><span class="sxs-lookup"><span data-stu-id="5c147-175">[application](application.md) collection</span></span>| <span data-ttu-id="5c147-176">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5c147-176">Read-only.</span></span> <span data-ttu-id="5c147-177">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5c147-177">Nullable.</span></span>|
|<span data-ttu-id="5c147-178">members</span><span class="sxs-lookup"><span data-stu-id="5c147-178">members</span></span>|<span data-ttu-id="5c147-179">Коллекция [соединителей](connector.md)</span><span class="sxs-lookup"><span data-stu-id="5c147-179">[connector](connector.md) collection</span></span>| <span data-ttu-id="5c147-p109">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5c147-p109">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5c147-182">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5c147-182">JSON representation</span></span>

<span data-ttu-id="5c147-183">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c147-183">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectorGroup"
}-->

```json
{
  "id": "String (identifier)",
  "isDefault": true,
  "name": "String",
  "region": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "connectorGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


