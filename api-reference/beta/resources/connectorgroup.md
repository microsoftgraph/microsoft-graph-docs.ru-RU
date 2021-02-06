---
title: Тип ресурса connectorGroup
description: Представляет соединители соединители прокси приложения.
localization_priority: Normal
ms.prod: applications
author: japere
doc_type: resourcePageType
ms.openlocfilehash: 78716646f4bf5cbba7a66da4cdef88d94d1984aa
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132327"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="f50ac-103">Тип ресурса connectorGroup</span><span class="sxs-lookup"><span data-stu-id="f50ac-103">connectorGroup resource type</span></span>

<span data-ttu-id="f50ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f50ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f50ac-105">Каждый [прокси-сервер приложения Azure AD](https://aka.ms/whyappproxy) всегда является частью группы соединители.</span><span class="sxs-lookup"><span data-stu-id="f50ac-105">Each [Azure AD Application Proxy](https://aka.ms/whyappproxy) connector is always part of a connector group.</span></span> <span data-ttu-id="f50ac-106">Все соединители, принадлежащие одной группе соединитеителей, выступают в качестве отдельной единицы для высокой доступности и балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="f50ac-106">All the connectors that belong to the same connector group act as a separate unit for high-availability and load balancing.</span></span> <span data-ttu-id="f50ac-107">Если группы соединители не создаются, все соединители будут в нее в составе группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f50ac-107">If you don't create connector groups, all your connectors will be part of the default group.</span></span> <span data-ttu-id="f50ac-108">При настройке приложения с помощью прокси приложения необходимо также указать группу соединители, которой необходимо назначить приложение.</span><span class="sxs-lookup"><span data-stu-id="f50ac-108">When configuring an application with Application Proxy, you must also specify which connector group to assign the application to.</span></span>

<span data-ttu-id="f50ac-109">После создания группы соединителю можно добавить или переместить соединители в группу соединителю с помощью [соединителю "Добавить".](../api/connectorgroup-post-members.md)</span><span class="sxs-lookup"><span data-stu-id="f50ac-109">After a connector group is created, you can add or move connectors to the connector group by using [Add connector](../api/connectorgroup-post-members.md).</span></span> <span data-ttu-id="f50ac-110">Вы также можете использовать [приложение "Добавить",](../api/connectorgroup-post-applications.md) чтобы назначить приложение группе соединителю.</span><span class="sxs-lookup"><span data-stu-id="f50ac-110">You can also use [Add application](../api/connectorgroup-post-applications.md) to assign an application to a connector group.</span></span>

## <a name="methods"></a><span data-ttu-id="f50ac-111">Методы</span><span class="sxs-lookup"><span data-stu-id="f50ac-111">Methods</span></span>

| <span data-ttu-id="f50ac-112">Метод</span><span class="sxs-lookup"><span data-stu-id="f50ac-112">Method</span></span>           | <span data-ttu-id="f50ac-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f50ac-113">Return Type</span></span>    |<span data-ttu-id="f50ac-114">Описание</span><span class="sxs-lookup"><span data-stu-id="f50ac-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f50ac-115">List connectorGroup</span><span class="sxs-lookup"><span data-stu-id="f50ac-115">List connectorGroup</span></span>](../api/connectorgroup-list.md) |<span data-ttu-id="f50ac-116">[Коллекция connectorGroup](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="f50ac-116">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="f50ac-117">Получить список объектов connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="f50ac-117">Retrieve a list of connectorGroup objects.</span></span> |
|[<span data-ttu-id="f50ac-118">Создание connectorGroup</span><span class="sxs-lookup"><span data-stu-id="f50ac-118">Create connectorGroup</span></span>](../api/connectorgroup-post.md) |<span data-ttu-id="f50ac-119">[Коллекция connectorGroup](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="f50ac-119">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="f50ac-120">Создание объекта connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="f50ac-120">Create a connectorGroup object.</span></span> |
|[<span data-ttu-id="f50ac-121">Получение connectorGroup</span><span class="sxs-lookup"><span data-stu-id="f50ac-121">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="f50ac-122">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="f50ac-122">connectorGroup</span></span>](connectorgroup.md) | <span data-ttu-id="f50ac-123">Чтение свойств и связей объекта connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="f50ac-123">Read properties and relationships of a connectorGroup object.</span></span> |
|[<span data-ttu-id="f50ac-124">Обновление connectorGroup</span><span class="sxs-lookup"><span data-stu-id="f50ac-124">Update connectorGroup</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="f50ac-125">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="f50ac-125">connectorGroup</span></span>](connectorgroup.md)| <span data-ttu-id="f50ac-126">Обновление объекта connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="f50ac-126">Update a connectorGroup object.</span></span> |
|[<span data-ttu-id="f50ac-127">Удаление connectorGroup</span><span class="sxs-lookup"><span data-stu-id="f50ac-127">Delete connectorGroup</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="f50ac-128">Нет</span><span class="sxs-lookup"><span data-stu-id="f50ac-128">None</span></span> | <span data-ttu-id="f50ac-129">Удаление объекта connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="f50ac-129">Delete a connectorGroup object.</span></span> <span data-ttu-id="f50ac-130">Перед удалением connectorGroup необходимо удалить все соединители из connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="f50ac-130">All connectors must be removed from the connectorGroup before a connectorGroup can be deleted.</span></span> |
|[<span data-ttu-id="f50ac-131">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="f50ac-131">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="f50ac-132">[коллекция соединители](connector.md)</span><span class="sxs-lookup"><span data-stu-id="f50ac-132">[connector](connector.md) collection</span></span>| <span data-ttu-id="f50ac-133">Получите коллекцию объектов соединители.</span><span class="sxs-lookup"><span data-stu-id="f50ac-133">Get a connector object collection.</span></span> |
|[<span data-ttu-id="f50ac-134">Перечисление приложений</span><span class="sxs-lookup"><span data-stu-id="f50ac-134">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="f50ac-135">Коллекция [application](application.md)</span><span class="sxs-lookup"><span data-stu-id="f50ac-135">[application](application.md) collection</span></span>| <span data-ttu-id="f50ac-136">Получение коллекции объектов приложения, связанной с connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="f50ac-136">Get the application object collection associated with the connectorGroup.</span></span> |
|[<span data-ttu-id="f50ac-137">Добавление приложения</span><span class="sxs-lookup"><span data-stu-id="f50ac-137">Add application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="f50ac-138">application</span><span class="sxs-lookup"><span data-stu-id="f50ac-138">application</span></span>](application.md)| <span data-ttu-id="f50ac-139">Связывать приложение с connectorGroup путем публикации в коллекции приложений.</span><span class="sxs-lookup"><span data-stu-id="f50ac-139">Associate an application with the connectorGroup by posting to the applications collection.</span></span> |
|[<span data-ttu-id="f50ac-140">Добавление соединителя</span><span class="sxs-lookup"><span data-stu-id="f50ac-140">Add connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="f50ac-141">connector</span><span class="sxs-lookup"><span data-stu-id="f50ac-141">connector</span></span>](connector.md)| <span data-ttu-id="f50ac-142">Добавление соединителя в connectorGroup путем добавления в коллекцию connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="f50ac-142">Add a connector to the connectorGroup by posting to the connectorGroup collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="f50ac-143">Свойства</span><span class="sxs-lookup"><span data-stu-id="f50ac-143">Properties</span></span>
| <span data-ttu-id="f50ac-144">Свойство</span><span class="sxs-lookup"><span data-stu-id="f50ac-144">Property</span></span>     | <span data-ttu-id="f50ac-145">Тип</span><span class="sxs-lookup"><span data-stu-id="f50ac-145">Type</span></span>   |<span data-ttu-id="f50ac-146">Описание</span><span class="sxs-lookup"><span data-stu-id="f50ac-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f50ac-147">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="f50ac-147">connectorGroupType</span></span>|<span data-ttu-id="f50ac-148">string</span><span class="sxs-lookup"><span data-stu-id="f50ac-148">string</span></span>| <span data-ttu-id="f50ac-149">Указывает тип гибридного агента.</span><span class="sxs-lookup"><span data-stu-id="f50ac-149">Indicates the type of hybrid agent.</span></span> <span data-ttu-id="f50ac-150">Это предварительно заданной системой.</span><span class="sxs-lookup"><span data-stu-id="f50ac-150">This pre-set by the system.</span></span> <span data-ttu-id="f50ac-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f50ac-151">Read-only.</span></span> |
|<span data-ttu-id="f50ac-152">id</span><span class="sxs-lookup"><span data-stu-id="f50ac-152">id</span></span>|<span data-ttu-id="f50ac-153">string</span><span class="sxs-lookup"><span data-stu-id="f50ac-153">string</span></span>| <span data-ttu-id="f50ac-154">Уникальный идентификатор для этого соединителаGroup.</span><span class="sxs-lookup"><span data-stu-id="f50ac-154">Unique identifier for this connectorGroup.</span></span> <span data-ttu-id="f50ac-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f50ac-155">Read-only.</span></span> |
|<span data-ttu-id="f50ac-156">isDefault</span><span class="sxs-lookup"><span data-stu-id="f50ac-156">isDefault</span></span>|<span data-ttu-id="f50ac-157">boolean</span><span class="sxs-lookup"><span data-stu-id="f50ac-157">boolean</span></span>| <span data-ttu-id="f50ac-158">Указывает, является ли connectorGroup соединитетелем по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f50ac-158">Indicates if the connectorGroup is the default connectorGroup.</span></span> <span data-ttu-id="f50ac-159">Только одна группа соединительных соединительных подключений может быть соединитеной группой по умолчанию, которая предварительно заданной системой.</span><span class="sxs-lookup"><span data-stu-id="f50ac-159">Only a single connector group can be the default connectorGroup and this is pre-set by the system.</span></span> <span data-ttu-id="f50ac-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f50ac-160">Read-only.</span></span> |
|<span data-ttu-id="f50ac-161">name</span><span class="sxs-lookup"><span data-stu-id="f50ac-161">name</span></span>|<span data-ttu-id="f50ac-162">string</span><span class="sxs-lookup"><span data-stu-id="f50ac-162">string</span></span>| <span data-ttu-id="f50ac-163">Имя, связанное с соединитетелемGroup.</span><span class="sxs-lookup"><span data-stu-id="f50ac-163">The name associated with the connectorGroup.</span></span> |
|<span data-ttu-id="f50ac-164">region</span><span class="sxs-lookup"><span data-stu-id="f50ac-164">region</span></span>|<span data-ttu-id="f50ac-165">string</span><span class="sxs-lookup"><span data-stu-id="f50ac-165">string</span></span>| <span data-ttu-id="f50ac-166">Регион, для который назначен соединительГрупп и для который будет оптимизирована трафик.</span><span class="sxs-lookup"><span data-stu-id="f50ac-166">The region the connectorGroup is assigned to and will optimize traffic for.</span></span> <span data-ttu-id="f50ac-167">Этот регион можно установить только в **том** случае, если соединители или приложения не назначены соединительной группе.</span><span class="sxs-lookup"><span data-stu-id="f50ac-167">This region can only be set if **no connectors or applications** are assigned to the connectorGroup.</span></span> <span data-ttu-id="f50ac-168">Доступны следующие регионы: Северная Америка, Европа, Австралия, Азия и Индия.</span><span class="sxs-lookup"><span data-stu-id="f50ac-168">The regions available include: North America, Europe, Australia, Asia, and India.</span></span> <span data-ttu-id="f50ac-169">Возможные значения: `nam`, `eur`, `aus`, `asia`, `ind`.</span><span class="sxs-lookup"><span data-stu-id="f50ac-169">Possible values are: `nam`, `eur`, `aus`, `asia`, `ind`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f50ac-170">Связи</span><span class="sxs-lookup"><span data-stu-id="f50ac-170">Relationships</span></span>
| <span data-ttu-id="f50ac-171">Связь</span><span class="sxs-lookup"><span data-stu-id="f50ac-171">Relationship</span></span> | <span data-ttu-id="f50ac-172">Тип</span><span class="sxs-lookup"><span data-stu-id="f50ac-172">Type</span></span>   |<span data-ttu-id="f50ac-173">Описание</span><span class="sxs-lookup"><span data-stu-id="f50ac-173">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f50ac-174">applications</span><span class="sxs-lookup"><span data-stu-id="f50ac-174">applications</span></span>|<span data-ttu-id="f50ac-175">Коллекция [application](application.md)</span><span class="sxs-lookup"><span data-stu-id="f50ac-175">[application](application.md) collection</span></span>| <span data-ttu-id="f50ac-176">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f50ac-176">Read-only.</span></span> <span data-ttu-id="f50ac-177">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f50ac-177">Nullable.</span></span>|
|<span data-ttu-id="f50ac-178">members</span><span class="sxs-lookup"><span data-stu-id="f50ac-178">members</span></span>|<span data-ttu-id="f50ac-179">[коллекция соединители](connector.md)</span><span class="sxs-lookup"><span data-stu-id="f50ac-179">[connector](connector.md) collection</span></span>| <span data-ttu-id="f50ac-p109">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f50ac-p109">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f50ac-182">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f50ac-182">JSON representation</span></span>

<span data-ttu-id="f50ac-183">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f50ac-183">The following is a JSON representation of the resource.</span></span>

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



