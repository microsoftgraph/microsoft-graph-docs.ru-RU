---
title: Тип ресурса schemaExtension (расширения схемы)
description: 'С помощью расширений схемы вы можете задать схему, которую необходимо расширить, и добавить строго типизированные пользовательские данные в тип ресурса. В расширенном ресурсе пользовательские данные имеют сложный тип. '
localization_priority: Priority
author: dkershaw10
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 38bb2d34347f253d114d549b32d6db98c12aa831
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446956"
---
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="265a4-104">Тип ресурса schemaExtension (расширения схемы)</span><span class="sxs-lookup"><span data-stu-id="265a4-104">schemaExtension resource type (schema extensions)</span></span>

<span data-ttu-id="265a4-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="265a4-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="265a4-p102">С помощью расширений схемы вы можете задать схему, которую необходимо расширить, и добавить строго типизированные пользовательские данные в тип ресурса. В расширенном ресурсе пользовательские данные имеют сложный тип.</span><span class="sxs-lookup"><span data-stu-id="265a4-p102">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="265a4-108">Расширения схемы поддерживаются в ресурсах указанных ниже типов.</span><span class="sxs-lookup"><span data-stu-id="265a4-108">Schema extensions are supported by the following resource types:</span></span>

- [<span data-ttu-id="265a4-109">contact</span><span class="sxs-lookup"><span data-stu-id="265a4-109">contact</span></span>](contact.md)
- [<span data-ttu-id="265a4-110">device</span><span class="sxs-lookup"><span data-stu-id="265a4-110">device</span></span>](device.md)
- <span data-ttu-id="265a4-111">[event](event.md) (для пользователя или календаря группы Office 365)</span><span class="sxs-lookup"><span data-stu-id="265a4-111">[event](event.md) on a user or Office 365 group calendar</span></span>
- <span data-ttu-id="265a4-112">[post](post.md) (для группы Office 365)</span><span class="sxs-lookup"><span data-stu-id="265a4-112">[post](post.md) of an Office 365 group</span></span>
- [<span data-ttu-id="265a4-113">group</span><span class="sxs-lookup"><span data-stu-id="265a4-113">group</span></span>](group.md)
- [<span data-ttu-id="265a4-114">message</span><span class="sxs-lookup"><span data-stu-id="265a4-114">message</span></span>](message.md) 
- [<span data-ttu-id="265a4-115">organization</span><span class="sxs-lookup"><span data-stu-id="265a4-115">organization</span></span>](organization.md)
- [<span data-ttu-id="265a4-116">user</span><span class="sxs-lookup"><span data-stu-id="265a4-116">user</span></span>](user.md)

<span data-ttu-id="265a4-117">Сведения о том, как добавлять пользовательские данные в группы, см. в [примере расширения схемы](/graph/extensibility-schema-groups).</span><span class="sxs-lookup"><span data-stu-id="265a4-117">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="265a4-118">Методы</span><span class="sxs-lookup"><span data-stu-id="265a4-118">Methods</span></span>

| <span data-ttu-id="265a4-119">Метод</span><span class="sxs-lookup"><span data-stu-id="265a4-119">Method</span></span>           | <span data-ttu-id="265a4-120">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="265a4-120">Return Type</span></span>    |<span data-ttu-id="265a4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="265a4-121">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="265a4-122">Создание</span><span class="sxs-lookup"><span data-stu-id="265a4-122">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="265a4-123">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="265a4-123">schemaExtension</span></span> |<span data-ttu-id="265a4-124">Создание определения расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="265a4-124">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="265a4-125">Перечисление</span><span class="sxs-lookup"><span data-stu-id="265a4-125">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="265a4-126">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="265a4-126">schemaExtension</span></span> |<span data-ttu-id="265a4-127">Создание списка доступных определений schemaExtension и их свойств.</span><span class="sxs-lookup"><span data-stu-id="265a4-127">List the available schemaExtension definitions and their properties.</span></span>|
|[<span data-ttu-id="265a4-128">Получение</span><span class="sxs-lookup"><span data-stu-id="265a4-128">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="265a4-129">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="265a4-129">schemaExtension</span></span> |<span data-ttu-id="265a4-130">Получение свойств указанного определения schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="265a4-130">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="265a4-131">Обновление</span><span class="sxs-lookup"><span data-stu-id="265a4-131">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="265a4-132">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="265a4-132">schemaExtension</span></span>   |<span data-ttu-id="265a4-133">Обновление определения schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="265a4-133">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="265a4-134">Удаление</span><span class="sxs-lookup"><span data-stu-id="265a4-134">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="265a4-135">Нет</span><span class="sxs-lookup"><span data-stu-id="265a4-135">None</span></span> |<span data-ttu-id="265a4-136">Удаление определения schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="265a4-136">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="265a4-137">Свойства</span><span class="sxs-lookup"><span data-stu-id="265a4-137">Properties</span></span>
| <span data-ttu-id="265a4-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="265a4-138">Property</span></span>     | <span data-ttu-id="265a4-139">Тип</span><span class="sxs-lookup"><span data-stu-id="265a4-139">Type</span></span>   |<span data-ttu-id="265a4-140">Описание</span><span class="sxs-lookup"><span data-stu-id="265a4-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="265a4-141">description</span><span class="sxs-lookup"><span data-stu-id="265a4-141">description</span></span>|<span data-ttu-id="265a4-142">String</span><span class="sxs-lookup"><span data-stu-id="265a4-142">String</span></span>|<span data-ttu-id="265a4-143">Описание расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="265a4-143">Description for the schema extension.</span></span>|
|<span data-ttu-id="265a4-144">id</span><span class="sxs-lookup"><span data-stu-id="265a4-144">id</span></span>|<span data-ttu-id="265a4-145">String</span><span class="sxs-lookup"><span data-stu-id="265a4-145">String</span></span>|<span data-ttu-id="265a4-146">Уникальный идентификатор для определения расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="265a4-146">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="265a4-147">Значение можно присвоить одним из двух способов:</span><span class="sxs-lookup"><span data-stu-id="265a4-147">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="265a4-p103">Сцепите имя одного из ваших проверенных доменов с именем расширения схемы, чтобы создать уникальную строку такого формата: \{_&#65279;доменноеИмя_\}\_\{_&#65279;имяСхемы_\}. Например, `contoso_mySchema`. </span><span class="sxs-lookup"><span data-stu-id="265a4-p103">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="265a4-p104">Укажите имя схемы и предоставьте Microsoft Graph возможность использовать его для назначения **id** в таком формате: ext\{_&#65279;8-случайных-букв-или-цифр_\}\_\{_&#65279;имя-схемы_\}. Например, `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="265a4-p104">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="265a4-152">После создания это свойство невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="265a4-152">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="265a4-153">owner</span><span class="sxs-lookup"><span data-stu-id="265a4-153">owner</span></span>|<span data-ttu-id="265a4-154">String</span><span class="sxs-lookup"><span data-stu-id="265a4-154">String</span></span>|<span data-ttu-id="265a4-155">Идентификатор `appId` приложения, которое является владельцем расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="265a4-155">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="265a4-156">Это свойство можно указать при создании, чтобы задать владельца.</span><span class="sxs-lookup"><span data-stu-id="265a4-156">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="265a4-157">Если оно не указано, то в качестве владельца будет задано вызывающее приложение `appId`.</span><span class="sxs-lookup"><span data-stu-id="265a4-157">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="265a4-158">В любом случае, пользователь, выполнивший вход в систему, должен быть владельцем приложения.</span><span class="sxs-lookup"><span data-stu-id="265a4-158">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="265a4-159">После задания свойства оно будет доступно только для чтения, и вам не удастся изменить его.</span><span class="sxs-lookup"><span data-stu-id="265a4-159">Once set, this property is read-only and cannot be changed.</span></span>| 
|<span data-ttu-id="265a4-160">properties</span><span class="sxs-lookup"><span data-stu-id="265a4-160">properties</span></span>|<span data-ttu-id="265a4-161">Коллекция [extensionSchemaProperty](extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="265a4-161">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="265a4-162">Коллекция имен и типов свойств, составляющих определение расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="265a4-162">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="265a4-163">status</span><span class="sxs-lookup"><span data-stu-id="265a4-163">status</span></span>|<span data-ttu-id="265a4-164">String</span><span class="sxs-lookup"><span data-stu-id="265a4-164">String</span></span>|<span data-ttu-id="265a4-165">Состояние жизненного цикла расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="265a4-165">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="265a4-166">Возможные состояния: **InDevelopment**, **Available** и **Deprecated**.</span><span class="sxs-lookup"><span data-stu-id="265a4-166">Possible states are **InDevelopment**, **Available**, and **Deprecated**.</span></span> <span data-ttu-id="265a4-167">При создании свойство автоматически получает значение **InDevelopment**.</span><span class="sxs-lookup"><span data-stu-id="265a4-167">Automatically set to **InDevelopment** on creation.</span></span> <span data-ttu-id="265a4-168">[Расширения схемы](/graph/extensibility-overview#schema-extensions) предоставляют дополнительные сведения о возможных переходах из одного состояния в другое и о поведении.</span><span class="sxs-lookup"><span data-stu-id="265a4-168">[Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span>|
|<span data-ttu-id="265a4-169">targetTypes</span><span class="sxs-lookup"><span data-stu-id="265a4-169">targetTypes</span></span>|<span data-ttu-id="265a4-170">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="265a4-170">String collection</span></span>|<span data-ttu-id="265a4-171">Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы.</span><span class="sxs-lookup"><span data-stu-id="265a4-171">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span> <span data-ttu-id="265a4-172">Возможные варианты: **contact**, **device**, **event**, **group**, **message**, **organization**, **post** или **user**.</span><span class="sxs-lookup"><span data-stu-id="265a4-172">Select from **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="265a4-173">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="265a4-173">JSON representation</span></span>

<span data-ttu-id="265a4-174">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="265a4-174">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.schemaExtension"
}-->

```json
{
  "description": "String",
  "id": "String (identifier)",
  "owner": "String",
  "properties": [{"@odata.type": "microsoft.graph.extensionSchemaProperty"}],
  "status": "String",
  "targetTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "schemaExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
