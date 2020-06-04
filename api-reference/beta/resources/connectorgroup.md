---
title: Тип ресурса Коннекторграуп
description: Представляет прокси приложения Коннекторграуп.
localization_priority: Normal
ms.prod: microsoft-identity-platform
author: japere
doc_type: resourcePageType
ms.openlocfilehash: 446dae5e78878ba9648d532d2696b0bfde496601
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556172"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="48218-103">Тип ресурса Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="48218-103">connectorGroup resource type</span></span>

<span data-ttu-id="48218-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48218-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48218-105">Каждый соединитель [прокси приложения Azure AD](https://aka.ms/whyappproxy) всегда является частью группы соединителей.</span><span class="sxs-lookup"><span data-stu-id="48218-105">Each [Azure AD Application Proxy](https://aka.ms/whyappproxy) connector is always part of a connector group.</span></span> <span data-ttu-id="48218-106">Все соединители, принадлежащие одной и той же группе соединителей, действуют как отдельные единицы для обеспечения высокого уровня доступности и балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="48218-106">All the connectors that belong to the same connector group act as a separate unit for high-availability and load balancing.</span></span> <span data-ttu-id="48218-107">Если вы не создадите группы соединителей, все соединители будут входить в группу по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="48218-107">If you don't create connector groups, all your connectors will be part of the default group.</span></span> <span data-ttu-id="48218-108">При настройке приложения с помощью прокси для приложения также необходимо указать группу соединителей, которой необходимо назначить приложение.</span><span class="sxs-lookup"><span data-stu-id="48218-108">When configuring an application with Application Proxy, you must also specify which connector group to assign the application to.</span></span>

<span data-ttu-id="48218-109">После создания группы соединителей можно добавить или переместить соединители в группу соединителей с помощью [Add Connector](../api/connectorgroup-post-members.md).</span><span class="sxs-lookup"><span data-stu-id="48218-109">After a connector group is created, you can add or move connectors to the connector group by using [Add connector](../api/connectorgroup-post-members.md).</span></span> <span data-ttu-id="48218-110">Вы также можете использовать [Add Application](../api/connectorgroup-post-applications.md) , чтобы назначить приложение для группы соединителей.</span><span class="sxs-lookup"><span data-stu-id="48218-110">You can also use [Add application](../api/connectorgroup-post-applications.md) to assign an application to a connector group.</span></span>

## <a name="methods"></a><span data-ttu-id="48218-111">Методы</span><span class="sxs-lookup"><span data-stu-id="48218-111">Methods</span></span>

| <span data-ttu-id="48218-112">Метод</span><span class="sxs-lookup"><span data-stu-id="48218-112">Method</span></span>           | <span data-ttu-id="48218-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="48218-113">Return Type</span></span>    |<span data-ttu-id="48218-114">Описание</span><span class="sxs-lookup"><span data-stu-id="48218-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="48218-115">Список Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="48218-115">List connectorGroup</span></span>](../api/connectorgroup-list.md) |<span data-ttu-id="48218-116">Коллекция [коннекторграуп](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="48218-116">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="48218-117">Получение списка объектов Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="48218-117">Retrieve a list of connectorGroup objects.</span></span> |
|[<span data-ttu-id="48218-118">Получение Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="48218-118">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="48218-119">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="48218-119">connectorGroup</span></span>](connectorgroup.md) | <span data-ttu-id="48218-120">Чтение свойств и связей объекта Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="48218-120">Read properties and relationships of a connectorGroup object.</span></span> |
|[<span data-ttu-id="48218-121">Обновление Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="48218-121">Update connectorGroup</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="48218-122">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="48218-122">connectorGroup</span></span>](connectorgroup.md)| <span data-ttu-id="48218-123">Обновление объекта Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="48218-123">Update a connectorGroup object.</span></span> |
|[<span data-ttu-id="48218-124">Удаление Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="48218-124">Delete connectorGroup</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="48218-125">Нет</span><span class="sxs-lookup"><span data-stu-id="48218-125">None</span></span> | <span data-ttu-id="48218-126">Удаление объекта Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="48218-126">Delete a connectorGroup object.</span></span> <span data-ttu-id="48218-127">Прежде чем Коннекторграуп можно будет удалить, необходимо удалить все соединители из Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="48218-127">All connectors must be removed from the connectorGroup before a connectorGroup can be deleted.</span></span> |
|[<span data-ttu-id="48218-128">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="48218-128">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="48218-129">Коллекция [соединителей](connector.md)</span><span class="sxs-lookup"><span data-stu-id="48218-129">[connector](connector.md) collection</span></span>| <span data-ttu-id="48218-130">Получение коллекции объектов Connector.</span><span class="sxs-lookup"><span data-stu-id="48218-130">Get a connector object collection.</span></span> |
|[<span data-ttu-id="48218-131">Перечисление приложений</span><span class="sxs-lookup"><span data-stu-id="48218-131">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="48218-132">Коллекция [application](application.md)</span><span class="sxs-lookup"><span data-stu-id="48218-132">[application](application.md) collection</span></span>| <span data-ttu-id="48218-133">Получение коллекции объектов Application, связанной с Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="48218-133">Get the application object collection associated with the connectorGroup.</span></span> |
|[<span data-ttu-id="48218-134">Добавление приложения</span><span class="sxs-lookup"><span data-stu-id="48218-134">Add application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="48218-135">application</span><span class="sxs-lookup"><span data-stu-id="48218-135">application</span></span>](application.md)| <span data-ttu-id="48218-136">Свяжите приложение с Коннекторграуп, размещая в коллекции Applications.</span><span class="sxs-lookup"><span data-stu-id="48218-136">Associate an application with the connectorGroup by posting to the applications collection.</span></span> |
|[<span data-ttu-id="48218-137">Добавить соединитель</span><span class="sxs-lookup"><span data-stu-id="48218-137">Add connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="48218-138">PDIF</span><span class="sxs-lookup"><span data-stu-id="48218-138">connector</span></span>](connector.md)| <span data-ttu-id="48218-139">Добавление соединителя в Коннекторграуп путем публикации в коллекции Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="48218-139">Add a connector to the connectorGroup by posting to the connectorGroup collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="48218-140">Свойства</span><span class="sxs-lookup"><span data-stu-id="48218-140">Properties</span></span>
| <span data-ttu-id="48218-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="48218-141">Property</span></span>     | <span data-ttu-id="48218-142">Тип</span><span class="sxs-lookup"><span data-stu-id="48218-142">Type</span></span>   |<span data-ttu-id="48218-143">Описание</span><span class="sxs-lookup"><span data-stu-id="48218-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48218-144">коннекторграуптипе</span><span class="sxs-lookup"><span data-stu-id="48218-144">connectorGroupType</span></span>|<span data-ttu-id="48218-145">string</span><span class="sxs-lookup"><span data-stu-id="48218-145">string</span></span>| <span data-ttu-id="48218-146">Указывает тип гибридного агента.</span><span class="sxs-lookup"><span data-stu-id="48218-146">Indicates the type of hybrid agent.</span></span> <span data-ttu-id="48218-147">Это предварительно заданное системой.</span><span class="sxs-lookup"><span data-stu-id="48218-147">This pre-set by the system.</span></span> <span data-ttu-id="48218-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="48218-148">Read-only.</span></span> |
|<span data-ttu-id="48218-149">id</span><span class="sxs-lookup"><span data-stu-id="48218-149">id</span></span>|<span data-ttu-id="48218-150">строка</span><span class="sxs-lookup"><span data-stu-id="48218-150">string</span></span>| <span data-ttu-id="48218-151">Уникальный идентификатор для этого Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="48218-151">Unique identifier for this connectorGroup.</span></span> <span data-ttu-id="48218-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="48218-152">Read-only.</span></span> |
|<span data-ttu-id="48218-153">isDefault</span><span class="sxs-lookup"><span data-stu-id="48218-153">isDefault</span></span>|<span data-ttu-id="48218-154">boolean</span><span class="sxs-lookup"><span data-stu-id="48218-154">boolean</span></span>| <span data-ttu-id="48218-155">Указывает, является ли Коннекторграуп Коннекторграуп по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="48218-155">Indicates if the connectorGroup is the default connectorGroup.</span></span> <span data-ttu-id="48218-156">Только одна группа соединителей может быть Коннекторграуп по умолчанию, и она предопределена системой.</span><span class="sxs-lookup"><span data-stu-id="48218-156">Only a single connector group can be the default connectorGroup and this is pre-set by the system.</span></span> <span data-ttu-id="48218-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="48218-157">Read-only.</span></span> |
|<span data-ttu-id="48218-158">name</span><span class="sxs-lookup"><span data-stu-id="48218-158">name</span></span>|<span data-ttu-id="48218-159">string</span><span class="sxs-lookup"><span data-stu-id="48218-159">string</span></span>| <span data-ttu-id="48218-160">Имя, связанное с Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="48218-160">The name associated with the connectorGroup.</span></span> |
|<span data-ttu-id="48218-161">региональных</span><span class="sxs-lookup"><span data-stu-id="48218-161">region</span></span>|<span data-ttu-id="48218-162">string</span><span class="sxs-lookup"><span data-stu-id="48218-162">string</span></span>| <span data-ttu-id="48218-163">Регион, которому назначена Коннекторграуп, и который оптимизирует трафик для.</span><span class="sxs-lookup"><span data-stu-id="48218-163">The region the connectorGroup is assigned to and will optimize traffic for.</span></span> <span data-ttu-id="48218-164">Эту область можно задать только в том случае, если Коннекторграуп **не назначен ни один из соединителей или приложений** .</span><span class="sxs-lookup"><span data-stu-id="48218-164">This region can only be set if **no connectors or applications** are assigned to the connectorGroup.</span></span> <span data-ttu-id="48218-165">Доступны следующие регионы: Северная Америка, Европа, Австралия, Азия и Индии.</span><span class="sxs-lookup"><span data-stu-id="48218-165">The regions available include: North America, Europe, Australia, Asia, and India.</span></span> <span data-ttu-id="48218-166">Возможные значения: `nam`, `eur`, `aus`, `asia`, `ind`.</span><span class="sxs-lookup"><span data-stu-id="48218-166">Possible values are: `nam`, `eur`, `aus`, `asia`, `ind`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48218-167">Связи</span><span class="sxs-lookup"><span data-stu-id="48218-167">Relationships</span></span>
| <span data-ttu-id="48218-168">Связь</span><span class="sxs-lookup"><span data-stu-id="48218-168">Relationship</span></span> | <span data-ttu-id="48218-169">Тип</span><span class="sxs-lookup"><span data-stu-id="48218-169">Type</span></span>   |<span data-ttu-id="48218-170">Описание</span><span class="sxs-lookup"><span data-stu-id="48218-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48218-171">заявлен</span><span class="sxs-lookup"><span data-stu-id="48218-171">applications</span></span>|<span data-ttu-id="48218-172">Коллекция [application](application.md)</span><span class="sxs-lookup"><span data-stu-id="48218-172">[application](application.md) collection</span></span>| <span data-ttu-id="48218-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="48218-173">Read-only.</span></span> <span data-ttu-id="48218-174">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="48218-174">Nullable.</span></span>|
|<span data-ttu-id="48218-175">members</span><span class="sxs-lookup"><span data-stu-id="48218-175">members</span></span>|<span data-ttu-id="48218-176">Коллекция [соединителей](connector.md)</span><span class="sxs-lookup"><span data-stu-id="48218-176">[connector](connector.md) collection</span></span>| <span data-ttu-id="48218-p109">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="48218-p109">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="48218-179">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="48218-179">JSON representation</span></span>

<span data-ttu-id="48218-180">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48218-180">The following is a JSON representation of the resource.</span></span>

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
