---
title: Тип ресурса connectorGroup
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 211efe5d8caae57457a6a5cc4fa95d145cd176f3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823193"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="63157-103">Тип ресурса connectorGroup</span><span class="sxs-lookup"><span data-stu-id="63157-103">connectorGroup resource type</span></span>

> <span data-ttu-id="63157-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="63157-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63157-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63157-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="methods"></a><span data-ttu-id="63157-106">Методы</span><span class="sxs-lookup"><span data-stu-id="63157-106">Methods</span></span>

| <span data-ttu-id="63157-107">Метод</span><span class="sxs-lookup"><span data-stu-id="63157-107">Method</span></span>           | <span data-ttu-id="63157-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="63157-108">Return Type</span></span>    |<span data-ttu-id="63157-109">Описание</span><span class="sxs-lookup"><span data-stu-id="63157-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="63157-110">Получение connectorGroup</span><span class="sxs-lookup"><span data-stu-id="63157-110">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="63157-111">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="63157-111">connectorGroup</span></span>](connectorgroup.md) |<span data-ttu-id="63157-112">Чтение свойства и связи объекта connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="63157-112">Read properties and relationships of connectorGroup object.</span></span>|
|[<span data-ttu-id="63157-113">Создание приложения</span><span class="sxs-lookup"><span data-stu-id="63157-113">Create application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="63157-114">application</span><span class="sxs-lookup"><span data-stu-id="63157-114">application</span></span>](application.md)| <span data-ttu-id="63157-115">Свяжите приложение с группой соединителя с учета в коллекцию приложений.</span><span class="sxs-lookup"><span data-stu-id="63157-115">Associate an application with the connector group by posting to the applications collection.</span></span>|
|[<span data-ttu-id="63157-116">Список приложений</span><span class="sxs-lookup"><span data-stu-id="63157-116">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="63157-117">коллекции [приложения](application.md)</span><span class="sxs-lookup"><span data-stu-id="63157-117">[application](application.md) collection</span></span>| <span data-ttu-id="63157-118">Получение коллекции объектов связанного приложения.</span><span class="sxs-lookup"><span data-stu-id="63157-118">Get the associated application object collection.</span></span>|
|[<span data-ttu-id="63157-119">Создание соединителя</span><span class="sxs-lookup"><span data-stu-id="63157-119">Create connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="63157-120">Соединитель</span><span class="sxs-lookup"><span data-stu-id="63157-120">connector</span></span>](connector.md)| <span data-ttu-id="63157-121">Добавьте соединитель для соединителя группы, отправку сообщений в коллекцию элементов.</span><span class="sxs-lookup"><span data-stu-id="63157-121">Add a connector to the connector Group by posting to the members collection.</span></span>|
|[<span data-ttu-id="63157-122">Список членов</span><span class="sxs-lookup"><span data-stu-id="63157-122">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="63157-123">Коллекция [соединителей](connector.md)</span><span class="sxs-lookup"><span data-stu-id="63157-123">[connector](connector.md) collection</span></span>| <span data-ttu-id="63157-124">Получите соединитель коллекции объектов.</span><span class="sxs-lookup"><span data-stu-id="63157-124">Get a connector object collection.</span></span>|
|<span data-ttu-id="63157-125">[обновление](../api/connectorgroup-update.md).</span><span class="sxs-lookup"><span data-stu-id="63157-125">[Update](../api/connectorgroup-update.md)</span></span> | [<span data-ttu-id="63157-126">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="63157-126">connectorGroup</span></span>](connectorgroup.md)    |<span data-ttu-id="63157-127">Обновление объекта connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="63157-127">Update connectorGroup object.</span></span> |
|[<span data-ttu-id="63157-128">Delete</span><span class="sxs-lookup"><span data-stu-id="63157-128">Delete</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="63157-129">Нет</span><span class="sxs-lookup"><span data-stu-id="63157-129">None</span></span> |<span data-ttu-id="63157-130">Удалите объект connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="63157-130">Delete connectorGroup object.</span></span> <span data-ttu-id="63157-131">Все соединители должны быть Удаление соединителя группы могут быть удалены.</span><span class="sxs-lookup"><span data-stu-id="63157-131">All connectors must be remove before a conector group can be deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="63157-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="63157-132">Properties</span></span>
| <span data-ttu-id="63157-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="63157-133">Property</span></span>     | <span data-ttu-id="63157-134">Тип</span><span class="sxs-lookup"><span data-stu-id="63157-134">Type</span></span>   |<span data-ttu-id="63157-135">Описание</span><span class="sxs-lookup"><span data-stu-id="63157-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63157-136">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="63157-136">connectorGroupType</span></span>|<span data-ttu-id="63157-137">string</span><span class="sxs-lookup"><span data-stu-id="63157-137">string</span></span>| <span data-ttu-id="63157-138">Тип соединителей, которые будут использоваться с этой группой.</span><span class="sxs-lookup"><span data-stu-id="63157-138">The type of connectors that will be used with the group.</span></span> <span data-ttu-id="63157-139">Возможные значения: `applicationProxy`.</span><span class="sxs-lookup"><span data-stu-id="63157-139">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="63157-140">id</span><span class="sxs-lookup"><span data-stu-id="63157-140">id</span></span>|<span data-ttu-id="63157-141">Строка</span><span class="sxs-lookup"><span data-stu-id="63157-141">String</span></span>| <span data-ttu-id="63157-142">Идентификатор объекта connectorGroup</span><span class="sxs-lookup"><span data-stu-id="63157-142">The object id of the connectorGroup</span></span>|
|<span data-ttu-id="63157-143">isDefault</span><span class="sxs-lookup"><span data-stu-id="63157-143">isDefault</span></span>|<span data-ttu-id="63157-144">Логический</span><span class="sxs-lookup"><span data-stu-id="63157-144">Boolean</span></span>| <span data-ttu-id="63157-145">Указывает, является ли connectorGroup соединителя группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="63157-145">Indicates if the connectorGroup is the default connector group.</span></span> <span data-ttu-id="63157-146">Только один соединитель группы могут быть connectorGroup по умолчанию и устанавливается системой.</span><span class="sxs-lookup"><span data-stu-id="63157-146">Only a single connector Group can be the default connectorGroup and is set by the system.</span></span>|
|<span data-ttu-id="63157-147">name</span><span class="sxs-lookup"><span data-stu-id="63157-147">name</span></span>|<span data-ttu-id="63157-148">Строка</span><span class="sxs-lookup"><span data-stu-id="63157-148">String</span></span>| <span data-ttu-id="63157-149">Имя, связанное с connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="63157-149">The name associated with the connectorGroup.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63157-150">Связи</span><span class="sxs-lookup"><span data-stu-id="63157-150">Relationships</span></span>
| <span data-ttu-id="63157-151">Связь</span><span class="sxs-lookup"><span data-stu-id="63157-151">Relationship</span></span> | <span data-ttu-id="63157-152">Тип</span><span class="sxs-lookup"><span data-stu-id="63157-152">Type</span></span>   |<span data-ttu-id="63157-153">Описание</span><span class="sxs-lookup"><span data-stu-id="63157-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63157-154">приложения</span><span class="sxs-lookup"><span data-stu-id="63157-154">applications</span></span>|<span data-ttu-id="63157-155">коллекции [приложения](application.md)</span><span class="sxs-lookup"><span data-stu-id="63157-155">[application](application.md) collection</span></span>| <span data-ttu-id="63157-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="63157-p105">Read-only. Nullable.</span></span>|
|<span data-ttu-id="63157-158">members</span><span class="sxs-lookup"><span data-stu-id="63157-158">members</span></span>|<span data-ttu-id="63157-159">Коллекция [соединителей](connector.md)</span><span class="sxs-lookup"><span data-stu-id="63157-159">[connector](connector.md) collection</span></span>| <span data-ttu-id="63157-p106">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="63157-p106">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="63157-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="63157-162">JSON representation</span></span>

<span data-ttu-id="63157-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63157-163">Here is a JSON representation of the resource.</span></span>

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
