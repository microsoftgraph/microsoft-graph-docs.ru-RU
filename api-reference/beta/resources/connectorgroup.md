---
title: Тип ресурса connectorGroup
description: Ниже представлено описание ресурса в формате JSON.
ms.openlocfilehash: a3131b887216f1f400f70ed8d607477f65793cc7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079875"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="545b2-103">Тип ресурса connectorGroup</span><span class="sxs-lookup"><span data-stu-id="545b2-103">connectorGroup resource type</span></span>

> <span data-ttu-id="545b2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="545b2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="545b2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="545b2-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="methods"></a><span data-ttu-id="545b2-106">Методы</span><span class="sxs-lookup"><span data-stu-id="545b2-106">Methods</span></span>

| <span data-ttu-id="545b2-107">Метод</span><span class="sxs-lookup"><span data-stu-id="545b2-107">Method</span></span>           | <span data-ttu-id="545b2-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="545b2-108">Return Type</span></span>    |<span data-ttu-id="545b2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="545b2-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="545b2-110">Получение connectorGroup</span><span class="sxs-lookup"><span data-stu-id="545b2-110">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="545b2-111">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="545b2-111">connectorGroup</span></span>](connectorgroup.md) |<span data-ttu-id="545b2-112">Чтение свойства и связи объекта connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="545b2-112">Read properties and relationships of connectorGroup object.</span></span>|
|[<span data-ttu-id="545b2-113">Создание приложения</span><span class="sxs-lookup"><span data-stu-id="545b2-113">Create application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="545b2-114">application</span><span class="sxs-lookup"><span data-stu-id="545b2-114">application</span></span>](application.md)| <span data-ttu-id="545b2-115">Свяжите приложение с группой соединителя с учета в коллекцию приложений.</span><span class="sxs-lookup"><span data-stu-id="545b2-115">Associate an application with the connector group by posting to the applications collection.</span></span>|
|[<span data-ttu-id="545b2-116">Список приложений</span><span class="sxs-lookup"><span data-stu-id="545b2-116">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="545b2-117">коллекции [приложения](application.md)</span><span class="sxs-lookup"><span data-stu-id="545b2-117">[application](application.md) collection</span></span>| <span data-ttu-id="545b2-118">Получение коллекции объектов связанного приложения.</span><span class="sxs-lookup"><span data-stu-id="545b2-118">Get the associated application object collection.</span></span>|
|[<span data-ttu-id="545b2-119">Создание соединителя</span><span class="sxs-lookup"><span data-stu-id="545b2-119">Create connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="545b2-120">Соединитель</span><span class="sxs-lookup"><span data-stu-id="545b2-120">connector</span></span>](connector.md)| <span data-ttu-id="545b2-121">Добавьте соединитель для соединителя группы, отправку сообщений в коллекцию элементов.</span><span class="sxs-lookup"><span data-stu-id="545b2-121">Add a connector to the connector Group by posting to the members collection.</span></span>|
|[<span data-ttu-id="545b2-122">Список членов</span><span class="sxs-lookup"><span data-stu-id="545b2-122">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="545b2-123">Коллекция [соединителей](connector.md)</span><span class="sxs-lookup"><span data-stu-id="545b2-123">[connector](connector.md) collection</span></span>| <span data-ttu-id="545b2-124">Получите соединитель коллекции объектов.</span><span class="sxs-lookup"><span data-stu-id="545b2-124">Get a connector object collection.</span></span>|
|[<span data-ttu-id="545b2-125">Update</span><span class="sxs-lookup"><span data-stu-id="545b2-125">Update</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="545b2-126">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="545b2-126">connectorGroup</span></span>](connectorgroup.md)    |<span data-ttu-id="545b2-127">Обновление объекта connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="545b2-127">Update connectorGroup object.</span></span> |
|[<span data-ttu-id="545b2-128">Delete</span><span class="sxs-lookup"><span data-stu-id="545b2-128">Delete</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="545b2-129">Нет</span><span class="sxs-lookup"><span data-stu-id="545b2-129">None</span></span> |<span data-ttu-id="545b2-130">Удалите объект connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="545b2-130">Delete connectorGroup object.</span></span> <span data-ttu-id="545b2-131">Все соединители должны быть Удаление соединителя группы могут быть удалены.</span><span class="sxs-lookup"><span data-stu-id="545b2-131">All connectors must be remove before a conector group can be deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="545b2-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="545b2-132">Properties</span></span>
| <span data-ttu-id="545b2-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="545b2-133">Property</span></span>     | <span data-ttu-id="545b2-134">Тип</span><span class="sxs-lookup"><span data-stu-id="545b2-134">Type</span></span>   |<span data-ttu-id="545b2-135">Description</span><span class="sxs-lookup"><span data-stu-id="545b2-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="545b2-136">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="545b2-136">connectorGroupType</span></span>|<span data-ttu-id="545b2-137">string</span><span class="sxs-lookup"><span data-stu-id="545b2-137">string</span></span>| <span data-ttu-id="545b2-138">Тип соединителей, которые будут использоваться с этой группой.</span><span class="sxs-lookup"><span data-stu-id="545b2-138">The type of connectors that will be used with the group.</span></span> <span data-ttu-id="545b2-139">Возможные значения: `applicationProxy`.</span><span class="sxs-lookup"><span data-stu-id="545b2-139">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="545b2-140">id</span><span class="sxs-lookup"><span data-stu-id="545b2-140">id</span></span>|<span data-ttu-id="545b2-141">String</span><span class="sxs-lookup"><span data-stu-id="545b2-141">String</span></span>| <span data-ttu-id="545b2-142">Идентификатор объекта connectorGroup</span><span class="sxs-lookup"><span data-stu-id="545b2-142">The object id of the connectorGroup</span></span>|
|<span data-ttu-id="545b2-143">isDefault</span><span class="sxs-lookup"><span data-stu-id="545b2-143">isDefault</span></span>|<span data-ttu-id="545b2-144">Логический</span><span class="sxs-lookup"><span data-stu-id="545b2-144">Boolean</span></span>| <span data-ttu-id="545b2-145">Указывает, является ли connectorGroup соединителя группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="545b2-145">Indicates if the connectorGroup is the default connector group.</span></span> <span data-ttu-id="545b2-146">Только один соединитель группы могут быть connectorGroup по умолчанию и устанавливается системой.</span><span class="sxs-lookup"><span data-stu-id="545b2-146">Only a single connector Group can be the default connectorGroup and is set by the system.</span></span>|
|<span data-ttu-id="545b2-147">name</span><span class="sxs-lookup"><span data-stu-id="545b2-147">name</span></span>|<span data-ttu-id="545b2-148">String</span><span class="sxs-lookup"><span data-stu-id="545b2-148">String</span></span>| <span data-ttu-id="545b2-149">Имя, связанное с connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="545b2-149">The name associated with the connectorGroup.</span></span>|

## <a name="relationships"></a><span data-ttu-id="545b2-150">Связи</span><span class="sxs-lookup"><span data-stu-id="545b2-150">Relationships</span></span>
| <span data-ttu-id="545b2-151">Связь</span><span class="sxs-lookup"><span data-stu-id="545b2-151">Relationship</span></span> | <span data-ttu-id="545b2-152">Тип</span><span class="sxs-lookup"><span data-stu-id="545b2-152">Type</span></span>   |<span data-ttu-id="545b2-153">Description</span><span class="sxs-lookup"><span data-stu-id="545b2-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="545b2-154">приложения</span><span class="sxs-lookup"><span data-stu-id="545b2-154">applications</span></span>|<span data-ttu-id="545b2-155">коллекции [приложения](application.md)</span><span class="sxs-lookup"><span data-stu-id="545b2-155">[application](application.md) collection</span></span>| <span data-ttu-id="545b2-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="545b2-p105">Read-only. Nullable.</span></span>|
|<span data-ttu-id="545b2-158">members</span><span class="sxs-lookup"><span data-stu-id="545b2-158">members</span></span>|<span data-ttu-id="545b2-159">Коллекция [соединителей](connector.md)</span><span class="sxs-lookup"><span data-stu-id="545b2-159">[connector](connector.md) collection</span></span>| <span data-ttu-id="545b2-p106">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="545b2-p106">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="545b2-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="545b2-162">JSON representation</span></span>

<span data-ttu-id="545b2-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="545b2-163">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectorGroup"
}-->

```json
{
  "connectorGroupType": "string",
  "id": "String (identifier)",
  "isDefault": true,
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connectorGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
