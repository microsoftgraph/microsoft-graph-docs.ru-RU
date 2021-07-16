---
title: Тип ресурса schemaExtension (расширения схемы)
description: 'С помощью расширений схемы вы можете задать схему, которую необходимо расширить, и добавить строго типизированные пользовательские данные в тип ресурса. В расширенном ресурсе пользовательские данные имеют сложный тип. '
localization_priority: Normal
author: dkershaw10
doc_type: resourcePageType
ms.prod: extensions
ms.openlocfilehash: 43e5600ea7e8fb8a484216e8068c9ac3f29ac90d
ms.sourcegitcommit: 73bbf84e6f5dbc8c3db8ed2c48cc5ab9ae3cff78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2021
ms.locfileid: "53456417"
---
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="db009-104">Тип ресурса schemaExtension (расширения схемы)</span><span class="sxs-lookup"><span data-stu-id="db009-104">schemaExtension resource type (schema extensions)</span></span>

<span data-ttu-id="db009-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db009-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db009-p102">С помощью расширений схемы вы можете задать схему, которую необходимо расширить, и добавить строго типизированные пользовательские данные в тип ресурса. В расширенном ресурсе пользовательские данные имеют сложный тип.</span><span class="sxs-lookup"><span data-stu-id="db009-p102">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="db009-108">Расширения схемы поддерживаются в ресурсах указанных ниже типов.</span><span class="sxs-lookup"><span data-stu-id="db009-108">Schema extensions are supported by the following resource types:</span></span>

- [<span data-ttu-id="db009-109">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="db009-109">administrativeUnit</span></span>](administrativeunit.md)
- [<span data-ttu-id="db009-110">contact</span><span class="sxs-lookup"><span data-stu-id="db009-110">contact</span></span>](contact.md)
- [<span data-ttu-id="db009-111">device</span><span class="sxs-lookup"><span data-stu-id="db009-111">device</span></span>](device.md)
- <span data-ttu-id="db009-112">[event](event.md) (для пользователя или календаря группы Microsoft 365)</span><span class="sxs-lookup"><span data-stu-id="db009-112">[event](event.md) on a user or Microsoft 365 group calendar</span></span>
- <span data-ttu-id="db009-113">[post](post.md) (для группы Microsoft 365)</span><span class="sxs-lookup"><span data-stu-id="db009-113">[post](post.md) of a Microsoft 365 group</span></span>
- [<span data-ttu-id="db009-114">group</span><span class="sxs-lookup"><span data-stu-id="db009-114">group</span></span>](group.md)
- [<span data-ttu-id="db009-115">message</span><span class="sxs-lookup"><span data-stu-id="db009-115">message</span></span>](message.md) 
- [<span data-ttu-id="db009-116">organization</span><span class="sxs-lookup"><span data-stu-id="db009-116">organization</span></span>](organization.md)
- [<span data-ttu-id="db009-117">user</span><span class="sxs-lookup"><span data-stu-id="db009-117">user</span></span>](user.md)

<span data-ttu-id="db009-118">Сведения о том, как добавлять пользовательские данные в группы, см. в [примере расширения схемы](/graph/extensibility-schema-groups).</span><span class="sxs-lookup"><span data-stu-id="db009-118">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="db009-119">Методы</span><span class="sxs-lookup"><span data-stu-id="db009-119">Methods</span></span>

| <span data-ttu-id="db009-120">Метод</span><span class="sxs-lookup"><span data-stu-id="db009-120">Method</span></span>           | <span data-ttu-id="db009-121">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="db009-121">Return Type</span></span>    |<span data-ttu-id="db009-122">Описание</span><span class="sxs-lookup"><span data-stu-id="db009-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="db009-123">Создание</span><span class="sxs-lookup"><span data-stu-id="db009-123">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="db009-124">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="db009-124">schemaExtension</span></span> |<span data-ttu-id="db009-125">Создание определения расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="db009-125">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="db009-126">Перечисление</span><span class="sxs-lookup"><span data-stu-id="db009-126">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="db009-127">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="db009-127">schemaExtension</span></span> |<span data-ttu-id="db009-128">Перечислите схему avaialbeExtension defintions и их свойства.</span><span class="sxs-lookup"><span data-stu-id="db009-128">List the avaialbe schemaExtension defintions and their properties.</span></span>|
|[<span data-ttu-id="db009-129">Получение</span><span class="sxs-lookup"><span data-stu-id="db009-129">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="db009-130">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="db009-130">schemaExtension</span></span> |<span data-ttu-id="db009-131">Получение свойств указанного определения schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="db009-131">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="db009-132">Обновление</span><span class="sxs-lookup"><span data-stu-id="db009-132">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="db009-133">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="db009-133">schemaExtension</span></span>   |<span data-ttu-id="db009-134">Обновление определения schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="db009-134">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="db009-135">Удаление</span><span class="sxs-lookup"><span data-stu-id="db009-135">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="db009-136">Нет</span><span class="sxs-lookup"><span data-stu-id="db009-136">None</span></span> |<span data-ttu-id="db009-137">Удаление определения schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="db009-137">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="db009-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="db009-138">Properties</span></span>
| <span data-ttu-id="db009-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="db009-139">Property</span></span>     | <span data-ttu-id="db009-140">Тип</span><span class="sxs-lookup"><span data-stu-id="db009-140">Type</span></span>   |<span data-ttu-id="db009-141">Описание</span><span class="sxs-lookup"><span data-stu-id="db009-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db009-142">description</span><span class="sxs-lookup"><span data-stu-id="db009-142">description</span></span>|<span data-ttu-id="db009-143">String</span><span class="sxs-lookup"><span data-stu-id="db009-143">String</span></span>|<span data-ttu-id="db009-144">Описание расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="db009-144">Description for the schema extension.</span></span> <span data-ttu-id="db009-145">Поддерживает `$filter` (`eq`).</span><span class="sxs-lookup"><span data-stu-id="db009-145">Supports `$filter` (`eq`).</span></span>|
|<span data-ttu-id="db009-146">id</span><span class="sxs-lookup"><span data-stu-id="db009-146">id</span></span>|<span data-ttu-id="db009-147">String</span><span class="sxs-lookup"><span data-stu-id="db009-147">String</span></span>|<span data-ttu-id="db009-148">Уникальный идентификатор для определения расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="db009-148">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="db009-149">Значение можно присвоить одним из двух способов:</span><span class="sxs-lookup"><span data-stu-id="db009-149">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="db009-p104">Сцепите имя одного из ваших проверенных доменов с именем расширения схемы, чтобы создать уникальную строку такого формата: \{_&#65279;доменноеИмя_\}\_\{_&#65279;имяСхемы_\}. Например, `contoso_mySchema`. </span><span class="sxs-lookup"><span data-stu-id="db009-p104">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="db009-p105">Укажите имя схемы и предоставьте Microsoft Graph возможность использовать его для назначения **id** в таком формате: ext\{_&#65279;8-случайных-букв-или-цифр_\}\_\{_&#65279;имя-схемы_\}. Например, `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="db009-p105">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="db009-154">После создания это свойство невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="db009-154">This property cannot be changed after creation.</span></span> <span data-ttu-id="db009-155">Поддерживает `$filter` (`eq`).</span><span class="sxs-lookup"><span data-stu-id="db009-155">Supports `$filter` (`eq`).</span></span> |
|<span data-ttu-id="db009-156">owner</span><span class="sxs-lookup"><span data-stu-id="db009-156">owner</span></span>|<span data-ttu-id="db009-157">String</span><span class="sxs-lookup"><span data-stu-id="db009-157">String</span></span>| <span data-ttu-id="db009-158">Идентификатор `appId` приложения, которое является владельцем расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="db009-158">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="db009-159">Это свойство можно указать при создании, чтобы задать владельца.</span><span class="sxs-lookup"><span data-stu-id="db009-159">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="db009-160">Если оно не указано, то в качестве владельца будет задано вызывающее приложение `appId`.</span><span class="sxs-lookup"><span data-stu-id="db009-160">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="db009-161">В любом случае, пользователь, выполнивший вход в систему, должен быть владельцем приложения.</span><span class="sxs-lookup"><span data-stu-id="db009-161">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="db009-162">Таким образом, например, при создании определения расширения схемы с помощью песочницы Graph вам **потребуется** указать свойство владельца.</span><span class="sxs-lookup"><span data-stu-id="db009-162">So, for example, if creating a new schema extension definition using Graph Explorer, you **must** supply the owner property.</span></span> <span data-ttu-id="db009-163">После задания свойства оно будет доступно только для чтения, и вам не удастся изменить его.</span><span class="sxs-lookup"><span data-stu-id="db009-163">Once set, this property is read-only and cannot be changed.</span></span> <span data-ttu-id="db009-164">Поддерживает `$filter` (`eq`).</span><span class="sxs-lookup"><span data-stu-id="db009-164">Supports `$filter` (`eq`).</span></span>|
|<span data-ttu-id="db009-165">properties</span><span class="sxs-lookup"><span data-stu-id="db009-165">properties</span></span>|<span data-ttu-id="db009-166">Коллекция [extensionSchemaProperty](extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="db009-166">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="db009-167">Коллекция имен и типов свойств, составляющих определение расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="db009-167">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="db009-168">status</span><span class="sxs-lookup"><span data-stu-id="db009-168">status</span></span>|<span data-ttu-id="db009-169">String</span><span class="sxs-lookup"><span data-stu-id="db009-169">String</span></span>|<span data-ttu-id="db009-170">Состояние жизненного цикла расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="db009-170">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="db009-171">Возможные состояния: **InDevelopment**, **Available** и **Deprecated**.</span><span class="sxs-lookup"><span data-stu-id="db009-171">Possible states are **InDevelopment**, **Available**, and **Deprecated**.</span></span> <span data-ttu-id="db009-172">При создании свойство автоматически получает значение **InDevelopment**.</span><span class="sxs-lookup"><span data-stu-id="db009-172">Automatically set to **InDevelopment** on creation.</span></span> <span data-ttu-id="db009-173">[Расширения схемы](/graph/extensibility-overview#schema-extensions) предоставляют дополнительные сведения о возможных переходах из одного состояния в другое и о поведении.</span><span class="sxs-lookup"><span data-stu-id="db009-173">[Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span> <span data-ttu-id="db009-174">Поддерживает `$filter` (`eq`).</span><span class="sxs-lookup"><span data-stu-id="db009-174">Supports `$filter` (`eq`).</span></span>|
|<span data-ttu-id="db009-175">targetTypes</span><span class="sxs-lookup"><span data-stu-id="db009-175">targetTypes</span></span>|<span data-ttu-id="db009-176">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="db009-176">String collection</span></span>|<span data-ttu-id="db009-177">Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы.</span><span class="sxs-lookup"><span data-stu-id="db009-177">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span> <span data-ttu-id="db009-178">Выберите из **administrativeUnit**, **контакт**, **устройство**, **событие**, **группа**, **сообщение**, **организация**, **сообщение**, **или пользователь**.</span><span class="sxs-lookup"><span data-stu-id="db009-178">Select from **administrativeUnit**, **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="db009-179">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db009-179">JSON representation</span></span>

<span data-ttu-id="db009-180">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db009-180">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "schemaExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


