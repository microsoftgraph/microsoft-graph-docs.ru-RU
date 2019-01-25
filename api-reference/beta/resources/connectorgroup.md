---
title: Тип ресурса connectorGroup
description: Ниже показано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: de405d2f0cbe0417271ab54e66c5c30073d8ee7f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517500"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="4243e-103">Тип ресурса connectorGroup</span><span class="sxs-lookup"><span data-stu-id="4243e-103">connectorGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a><span data-ttu-id="4243e-104">Методы</span><span class="sxs-lookup"><span data-stu-id="4243e-104">Methods</span></span>

| <span data-ttu-id="4243e-105">Метод</span><span class="sxs-lookup"><span data-stu-id="4243e-105">Method</span></span>           | <span data-ttu-id="4243e-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4243e-106">Return Type</span></span>    |<span data-ttu-id="4243e-107">Описание</span><span class="sxs-lookup"><span data-stu-id="4243e-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4243e-108">Получение connectorGroup</span><span class="sxs-lookup"><span data-stu-id="4243e-108">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="4243e-109">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="4243e-109">connectorGroup</span></span>](connectorgroup.md) |<span data-ttu-id="4243e-110">Чтение свойства и связи объекта connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="4243e-110">Read properties and relationships of connectorGroup object.</span></span>|
|[<span data-ttu-id="4243e-111">Создание приложения</span><span class="sxs-lookup"><span data-stu-id="4243e-111">Create application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="4243e-112">application</span><span class="sxs-lookup"><span data-stu-id="4243e-112">application</span></span>](application.md)| <span data-ttu-id="4243e-113">Свяжите приложение с группой соединителя с учета в коллекцию приложений.</span><span class="sxs-lookup"><span data-stu-id="4243e-113">Associate an application with the connector group by posting to the applications collection.</span></span>|
|[<span data-ttu-id="4243e-114">Список приложений</span><span class="sxs-lookup"><span data-stu-id="4243e-114">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="4243e-115">коллекции [приложения](application.md)</span><span class="sxs-lookup"><span data-stu-id="4243e-115">[application](application.md) collection</span></span>| <span data-ttu-id="4243e-116">Получение коллекции объектов связанного приложения.</span><span class="sxs-lookup"><span data-stu-id="4243e-116">Get the associated application object collection.</span></span>|
|[<span data-ttu-id="4243e-117">Создание соединителя</span><span class="sxs-lookup"><span data-stu-id="4243e-117">Create connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="4243e-118">Connector</span><span class="sxs-lookup"><span data-stu-id="4243e-118">connector</span></span>](connector.md)| <span data-ttu-id="4243e-119">Добавьте соединитель для соединителя группы, отправку сообщений в коллекцию элементов.</span><span class="sxs-lookup"><span data-stu-id="4243e-119">Add a connector to the connector Group by posting to the members collection.</span></span>|
|[<span data-ttu-id="4243e-120">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="4243e-120">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="4243e-121">Коллекция [соединителей](connector.md)</span><span class="sxs-lookup"><span data-stu-id="4243e-121">[connector](connector.md) collection</span></span>| <span data-ttu-id="4243e-122">Получите соединитель коллекции объектов.</span><span class="sxs-lookup"><span data-stu-id="4243e-122">Get a connector object collection.</span></span>|
|[<span data-ttu-id="4243e-123">Update</span><span class="sxs-lookup"><span data-stu-id="4243e-123">Update</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="4243e-124">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="4243e-124">connectorGroup</span></span>](connectorgroup.md)    |<span data-ttu-id="4243e-125">Обновление объекта connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="4243e-125">Update connectorGroup object.</span></span> |
|[<span data-ttu-id="4243e-126">Delete</span><span class="sxs-lookup"><span data-stu-id="4243e-126">Delete</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="4243e-127">Нет</span><span class="sxs-lookup"><span data-stu-id="4243e-127">None</span></span> |<span data-ttu-id="4243e-128">Удалите объект connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="4243e-128">Delete connectorGroup object.</span></span> <span data-ttu-id="4243e-129">Все соединители должны быть Удаление соединителя группы могут быть удалены.</span><span class="sxs-lookup"><span data-stu-id="4243e-129">All connectors must be remove before a conector group can be deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="4243e-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="4243e-130">Properties</span></span>
| <span data-ttu-id="4243e-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="4243e-131">Property</span></span>     | <span data-ttu-id="4243e-132">Тип</span><span class="sxs-lookup"><span data-stu-id="4243e-132">Type</span></span>   |<span data-ttu-id="4243e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="4243e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4243e-134">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="4243e-134">connectorGroupType</span></span>|<span data-ttu-id="4243e-135">string</span><span class="sxs-lookup"><span data-stu-id="4243e-135">string</span></span>| <span data-ttu-id="4243e-136">Тип соединителей, которые будут использоваться с этой группой.</span><span class="sxs-lookup"><span data-stu-id="4243e-136">The type of connectors that will be used with the group.</span></span> <span data-ttu-id="4243e-137">Возможные значения: `applicationProxy`.</span><span class="sxs-lookup"><span data-stu-id="4243e-137">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="4243e-138">id</span><span class="sxs-lookup"><span data-stu-id="4243e-138">id</span></span>|<span data-ttu-id="4243e-139">String</span><span class="sxs-lookup"><span data-stu-id="4243e-139">String</span></span>| <span data-ttu-id="4243e-140">Идентификатор объекта connectorGroup</span><span class="sxs-lookup"><span data-stu-id="4243e-140">The object id of the connectorGroup</span></span>|
|<span data-ttu-id="4243e-141">isDefault</span><span class="sxs-lookup"><span data-stu-id="4243e-141">isDefault</span></span>|<span data-ttu-id="4243e-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="4243e-142">Boolean</span></span>| <span data-ttu-id="4243e-143">Указывает, является ли connectorGroup соединителя группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4243e-143">Indicates if the connectorGroup is the default connector group.</span></span> <span data-ttu-id="4243e-144">Только один соединитель группы могут быть connectorGroup по умолчанию и устанавливается системой.</span><span class="sxs-lookup"><span data-stu-id="4243e-144">Only a single connector Group can be the default connectorGroup and is set by the system.</span></span>|
|<span data-ttu-id="4243e-145">name</span><span class="sxs-lookup"><span data-stu-id="4243e-145">name</span></span>|<span data-ttu-id="4243e-146">String</span><span class="sxs-lookup"><span data-stu-id="4243e-146">String</span></span>| <span data-ttu-id="4243e-147">Имя, связанное с connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="4243e-147">The name associated with the connectorGroup.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4243e-148">Отношения</span><span class="sxs-lookup"><span data-stu-id="4243e-148">Relationships</span></span>
| <span data-ttu-id="4243e-149">Связь</span><span class="sxs-lookup"><span data-stu-id="4243e-149">Relationship</span></span> | <span data-ttu-id="4243e-150">Тип</span><span class="sxs-lookup"><span data-stu-id="4243e-150">Type</span></span>   |<span data-ttu-id="4243e-151">Описание</span><span class="sxs-lookup"><span data-stu-id="4243e-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4243e-152">приложения</span><span class="sxs-lookup"><span data-stu-id="4243e-152">applications</span></span>|<span data-ttu-id="4243e-153">коллекции [приложения](application.md)</span><span class="sxs-lookup"><span data-stu-id="4243e-153">[application](application.md) collection</span></span>| <span data-ttu-id="4243e-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4243e-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="4243e-156">members</span><span class="sxs-lookup"><span data-stu-id="4243e-156">members</span></span>|<span data-ttu-id="4243e-157">Коллекция [соединителей](connector.md)</span><span class="sxs-lookup"><span data-stu-id="4243e-157">[connector](connector.md) collection</span></span>| <span data-ttu-id="4243e-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4243e-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4243e-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4243e-160">JSON representation</span></span>

<span data-ttu-id="4243e-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4243e-161">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "connectorGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/connectorgroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
