---
title: тип ресурсов connectorGroup
description: Представляет соединители прокси-приложения.
localization_priority: Normal
ms.prod: applications
author: japere
doc_type: resourcePageType
ms.openlocfilehash: df3a80c6dfd4004daccfe33045c8775c2e2e6e48
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958810"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="7ac8d-103">тип ресурсов connectorGroup</span><span class="sxs-lookup"><span data-stu-id="7ac8d-103">connectorGroup resource type</span></span>

<span data-ttu-id="7ac8d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ac8d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ac8d-105">Каждый [соединитатель прокси-сервера приложения Azure AD](https://aka.ms/whyappproxy) всегда является частью группы соединители.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-105">Each [Azure AD Application Proxy](https://aka.ms/whyappproxy) connector is always part of a connector group.</span></span> <span data-ttu-id="7ac8d-106">Все соединители, принадлежащие к одной группе соединитетелей, выступают в качестве отдельного блока для балансировки высокой доступности и нагрузки.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-106">All the connectors that belong to the same connector group act as a separate unit for high-availability and load balancing.</span></span> <span data-ttu-id="7ac8d-107">Если вы не создаете соединители группы, все соединители будут частью группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-107">If you don't create connector groups, all your connectors will be part of the default group.</span></span> <span data-ttu-id="7ac8d-108">При настройке приложения с помощью прокси-сервера приложения необходимо также указать группу соединители для назначения приложения.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-108">When configuring an application with Application Proxy, you must also specify which connector group to assign the application to.</span></span>

<span data-ttu-id="7ac8d-109">После создания группы соединителю можно добавить или переместить соединители в группу соединителю с помощью [соединитетеля Add.](../api/connectorgroup-post-members.md)</span><span class="sxs-lookup"><span data-stu-id="7ac8d-109">After a connector group is created, you can add or move connectors to the connector group by using [Add connector](../api/connectorgroup-post-members.md).</span></span> <span data-ttu-id="7ac8d-110">Вы также можете использовать [приложение Add для](../api/connectorgroup-post-applications.md) назначения приложения группе соединителю.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-110">You can also use [Add application](../api/connectorgroup-post-applications.md) to assign an application to a connector group.</span></span>

## <a name="methods"></a><span data-ttu-id="7ac8d-111">Методы</span><span class="sxs-lookup"><span data-stu-id="7ac8d-111">Methods</span></span>

| <span data-ttu-id="7ac8d-112">Метод</span><span class="sxs-lookup"><span data-stu-id="7ac8d-112">Method</span></span>           | <span data-ttu-id="7ac8d-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7ac8d-113">Return Type</span></span>    |<span data-ttu-id="7ac8d-114">Описание</span><span class="sxs-lookup"><span data-stu-id="7ac8d-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7ac8d-115">Соединители спискиGroup</span><span class="sxs-lookup"><span data-stu-id="7ac8d-115">List connectorGroup</span></span>](../api/connectorgroup-list.md) |<span data-ttu-id="7ac8d-116">[коллекция connectorGroup](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="7ac8d-116">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="7ac8d-117">Извлечение списка объектов connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-117">Retrieve a list of connectorGroup objects.</span></span> |
|[<span data-ttu-id="7ac8d-118">Создание connectorGroup</span><span class="sxs-lookup"><span data-stu-id="7ac8d-118">Create connectorGroup</span></span>](../api/connectorgroup-post.md) |<span data-ttu-id="7ac8d-119">[коллекция connectorGroup](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="7ac8d-119">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="7ac8d-120">Создание объекта connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-120">Create a connectorGroup object.</span></span> |
|[<span data-ttu-id="7ac8d-121">Получение connectorGroup</span><span class="sxs-lookup"><span data-stu-id="7ac8d-121">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="7ac8d-122">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="7ac8d-122">connectorGroup</span></span>](connectorgroup.md) | <span data-ttu-id="7ac8d-123">Чтение свойств и связей объекта connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-123">Read properties and relationships of a connectorGroup object.</span></span> |
|[<span data-ttu-id="7ac8d-124">Обновление connectorGroup</span><span class="sxs-lookup"><span data-stu-id="7ac8d-124">Update connectorGroup</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="7ac8d-125">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="7ac8d-125">connectorGroup</span></span>](connectorgroup.md)| <span data-ttu-id="7ac8d-126">Обновление объекта connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-126">Update a connectorGroup object.</span></span> |
|[<span data-ttu-id="7ac8d-127">Удаление connectorGroup</span><span class="sxs-lookup"><span data-stu-id="7ac8d-127">Delete connectorGroup</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="7ac8d-128">Нет</span><span class="sxs-lookup"><span data-stu-id="7ac8d-128">None</span></span> | <span data-ttu-id="7ac8d-129">Удаление объекта connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-129">Delete a connectorGroup object.</span></span> <span data-ttu-id="7ac8d-130">Все соединители должны быть удалены из соединителиГруппы, прежде чем соединителиGroup можно удалить.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-130">All connectors must be removed from the connectorGroup before a connectorGroup can be deleted.</span></span> |
|[<span data-ttu-id="7ac8d-131">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="7ac8d-131">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="7ac8d-132">[коллекция соединители](connector.md)</span><span class="sxs-lookup"><span data-stu-id="7ac8d-132">[connector](connector.md) collection</span></span>| <span data-ttu-id="7ac8d-133">Получите коллекцию объектов соединители.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-133">Get a connector object collection.</span></span> |
|[<span data-ttu-id="7ac8d-134">Перечисление приложений</span><span class="sxs-lookup"><span data-stu-id="7ac8d-134">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="7ac8d-135">Коллекция [application](application.md)</span><span class="sxs-lookup"><span data-stu-id="7ac8d-135">[application](application.md) collection</span></span>| <span data-ttu-id="7ac8d-136">Получение коллекции объектов приложения, связанной с соединитетелемGroup.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-136">Get the application object collection associated with the connectorGroup.</span></span> |
|[<span data-ttu-id="7ac8d-137">Добавление приложения</span><span class="sxs-lookup"><span data-stu-id="7ac8d-137">Add application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="7ac8d-138">application</span><span class="sxs-lookup"><span data-stu-id="7ac8d-138">application</span></span>](application.md)| <span data-ttu-id="7ac8d-139">Связать приложение с соединителягруппой, разместив в коллекции приложений.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-139">Associate an application with the connectorGroup by posting to the applications collection.</span></span> |
|[<span data-ttu-id="7ac8d-140">Добавление соединителя</span><span class="sxs-lookup"><span data-stu-id="7ac8d-140">Add connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="7ac8d-141">connector</span><span class="sxs-lookup"><span data-stu-id="7ac8d-141">connector</span></span>](connector.md)| <span data-ttu-id="7ac8d-142">Добавьте соединителю в соединителюGroup, разместив его в коллекции connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-142">Add a connector to the connectorGroup by posting to the connectorGroup collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="7ac8d-143">Свойства</span><span class="sxs-lookup"><span data-stu-id="7ac8d-143">Properties</span></span>
| <span data-ttu-id="7ac8d-144">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ac8d-144">Property</span></span>     | <span data-ttu-id="7ac8d-145">Тип</span><span class="sxs-lookup"><span data-stu-id="7ac8d-145">Type</span></span>   |<span data-ttu-id="7ac8d-146">Описание</span><span class="sxs-lookup"><span data-stu-id="7ac8d-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ac8d-147">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="7ac8d-147">connectorGroupType</span></span>|<span data-ttu-id="7ac8d-148">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="7ac8d-148">connectorGroupType</span></span>| <span data-ttu-id="7ac8d-149">Указывает тип гибридного агента.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-149">Indicates the type of hybrid agent.</span></span> <span data-ttu-id="7ac8d-150">Это заранее заданной системой.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-150">This pre-set by the system.</span></span> <span data-ttu-id="7ac8d-151">Возможные значения: `applicationProxy` .</span><span class="sxs-lookup"><span data-stu-id="7ac8d-151">Possible values are: `applicationProxy`.</span></span> <span data-ttu-id="7ac8d-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-152">Read-only.</span></span> |
|<span data-ttu-id="7ac8d-153">id</span><span class="sxs-lookup"><span data-stu-id="7ac8d-153">id</span></span>|<span data-ttu-id="7ac8d-154">string</span><span class="sxs-lookup"><span data-stu-id="7ac8d-154">string</span></span>| <span data-ttu-id="7ac8d-155">Уникальный идентификатор для этого соединитетеляGroup.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-155">Unique identifier for this connectorGroup.</span></span> <span data-ttu-id="7ac8d-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-156">Read-only.</span></span> |
|<span data-ttu-id="7ac8d-157">isDefault</span><span class="sxs-lookup"><span data-stu-id="7ac8d-157">isDefault</span></span>|<span data-ttu-id="7ac8d-158">boolean</span><span class="sxs-lookup"><span data-stu-id="7ac8d-158">boolean</span></span>| <span data-ttu-id="7ac8d-159">Указывает, является ли соединительщикОм ConnectorGroup по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-159">Indicates if the connectorGroup is the default connectorGroup.</span></span> <span data-ttu-id="7ac8d-160">Соединительщиком по умолчанию может быть только одна группа соединительных групп, и это заранее заданной системой.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-160">Only a single connector group can be the default connectorGroup and this is pre-set by the system.</span></span> <span data-ttu-id="7ac8d-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-161">Read-only.</span></span> |
|<span data-ttu-id="7ac8d-162">name</span><span class="sxs-lookup"><span data-stu-id="7ac8d-162">name</span></span>|<span data-ttu-id="7ac8d-163">string</span><span class="sxs-lookup"><span data-stu-id="7ac8d-163">string</span></span>| <span data-ttu-id="7ac8d-164">Имя, связанное с соединитетелемGroup.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-164">The name associated with the connectorGroup.</span></span> |
|<span data-ttu-id="7ac8d-165">регион</span><span class="sxs-lookup"><span data-stu-id="7ac8d-165">region</span></span>|<span data-ttu-id="7ac8d-166">connectorGroupRegion</span><span class="sxs-lookup"><span data-stu-id="7ac8d-166">connectorGroupRegion</span></span>| <span data-ttu-id="7ac8d-167">Регион, в который назначен connectorGroup, и будет оптимизировать трафик.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-167">The region the connectorGroup is assigned to and will optimize traffic for.</span></span> <span data-ttu-id="7ac8d-168">Этот регион можно установить только в **том** случае, если соединители или приложения не назначены соединительгруппе.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-168">This region can only be set if **no connectors or applications** are assigned to the connectorGroup.</span></span> <span data-ttu-id="7ac8d-169">Возможные значения: (для Северной `nam` **Америки),** `eur` (для Европы), `aus` (для Австралии), `asia` (для Азии), `ind` (для Индии) и `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="7ac8d-169">The possible values are: `nam` (for **North America**), `eur` (for Europe), `aus` (for Australia), `asia` (for Asia), `ind` (for India), and `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ac8d-170">Связи</span><span class="sxs-lookup"><span data-stu-id="7ac8d-170">Relationships</span></span>
| <span data-ttu-id="7ac8d-171">Связь</span><span class="sxs-lookup"><span data-stu-id="7ac8d-171">Relationship</span></span> | <span data-ttu-id="7ac8d-172">Тип</span><span class="sxs-lookup"><span data-stu-id="7ac8d-172">Type</span></span>   |<span data-ttu-id="7ac8d-173">Описание</span><span class="sxs-lookup"><span data-stu-id="7ac8d-173">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ac8d-174">приложения</span><span class="sxs-lookup"><span data-stu-id="7ac8d-174">applications</span></span>|<span data-ttu-id="7ac8d-175">Коллекция [application](application.md)</span><span class="sxs-lookup"><span data-stu-id="7ac8d-175">[application](application.md) collection</span></span>| <span data-ttu-id="7ac8d-176">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-176">Read-only.</span></span> <span data-ttu-id="7ac8d-177">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-177">Nullable.</span></span>|
|<span data-ttu-id="7ac8d-178">members</span><span class="sxs-lookup"><span data-stu-id="7ac8d-178">members</span></span>|<span data-ttu-id="7ac8d-179">[коллекция соединители](connector.md)</span><span class="sxs-lookup"><span data-stu-id="7ac8d-179">[connector](connector.md) collection</span></span>| <span data-ttu-id="7ac8d-p109">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-p109">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7ac8d-182">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7ac8d-182">JSON representation</span></span>

<span data-ttu-id="7ac8d-183">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ac8d-183">The following is a JSON representation of the resource.</span></span>

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



