---
title: Тип ресурса schemaExtension (расширения схемы)
description: 'Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource. '
localization_priority: Normal
author: dkershaw10
doc_type: resourcePageType
ms.prod: extensions
ms.openlocfilehash: 6959a21d2341c9868c8a3e20e39098c1fe048277
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896968"
---
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="51e9e-104">Тип ресурса schemaExtension (расширения схемы)</span><span class="sxs-lookup"><span data-stu-id="51e9e-104">schemaExtension resource type (schema extensions)</span></span>

<span data-ttu-id="51e9e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51e9e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51e9e-106">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type.</span><span class="sxs-lookup"><span data-stu-id="51e9e-106">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type.</span></span> <span data-ttu-id="51e9e-107">The custom data appears as a complex type on the extended resource.</span><span class="sxs-lookup"><span data-stu-id="51e9e-107">The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="51e9e-108">Расширения схемы поддерживаются в ресурсах указанных ниже типов.</span><span class="sxs-lookup"><span data-stu-id="51e9e-108">Schema extensions are supported by the following resource types:</span></span>

- [<span data-ttu-id="51e9e-109">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="51e9e-109">administrativeUnit</span></span>](administrativeunit.md)
- [<span data-ttu-id="51e9e-110">contact</span><span class="sxs-lookup"><span data-stu-id="51e9e-110">contact</span></span>](contact.md)
- [<span data-ttu-id="51e9e-111">device</span><span class="sxs-lookup"><span data-stu-id="51e9e-111">device</span></span>](device.md)
- <span data-ttu-id="51e9e-112">[событие](event.md) для пользователя или календаря группы Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="51e9e-112">[event](event.md) on a user or Microsoft 365 group calendar</span></span>
- <span data-ttu-id="51e9e-113">[Публикация](post.md) группы Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="51e9e-113">[post](post.md) of a Microsoft 365 group</span></span>
- [<span data-ttu-id="51e9e-114">group</span><span class="sxs-lookup"><span data-stu-id="51e9e-114">group</span></span>](group.md)
- [<span data-ttu-id="51e9e-115">message</span><span class="sxs-lookup"><span data-stu-id="51e9e-115">message</span></span>](message.md) 
- [<span data-ttu-id="51e9e-116">organization</span><span class="sxs-lookup"><span data-stu-id="51e9e-116">organization</span></span>](organization.md)
- [<span data-ttu-id="51e9e-117">user</span><span class="sxs-lookup"><span data-stu-id="51e9e-117">user</span></span>](user.md)

<span data-ttu-id="51e9e-118">Сведения о том, как добавлять пользовательские данные в группы, см. в [примере расширения схемы](/graph/extensibility-schema-groups).</span><span class="sxs-lookup"><span data-stu-id="51e9e-118">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="51e9e-119">Методы</span><span class="sxs-lookup"><span data-stu-id="51e9e-119">Methods</span></span>

| <span data-ttu-id="51e9e-120">Метод</span><span class="sxs-lookup"><span data-stu-id="51e9e-120">Method</span></span>           | <span data-ttu-id="51e9e-121">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="51e9e-121">Return Type</span></span>    |<span data-ttu-id="51e9e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="51e9e-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="51e9e-123">Создание</span><span class="sxs-lookup"><span data-stu-id="51e9e-123">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="51e9e-124">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="51e9e-124">schemaExtension</span></span> |<span data-ttu-id="51e9e-125">Создание определения расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="51e9e-125">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="51e9e-126">Перечисление</span><span class="sxs-lookup"><span data-stu-id="51e9e-126">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="51e9e-127">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="51e9e-127">schemaExtension</span></span> |<span data-ttu-id="51e9e-128">Перечислите аваиалбе schemaExtension дефинтионс и их свойства.</span><span class="sxs-lookup"><span data-stu-id="51e9e-128">List the avaialbe schemaExtension defintions and their properties.</span></span>|
|[<span data-ttu-id="51e9e-129">Получение</span><span class="sxs-lookup"><span data-stu-id="51e9e-129">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="51e9e-130">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="51e9e-130">schemaExtension</span></span> |<span data-ttu-id="51e9e-131">Получение свойств указанного определения schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="51e9e-131">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="51e9e-132">Обновление</span><span class="sxs-lookup"><span data-stu-id="51e9e-132">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="51e9e-133">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="51e9e-133">schemaExtension</span></span>   |<span data-ttu-id="51e9e-134">Обновление определения schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="51e9e-134">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="51e9e-135">Удаление</span><span class="sxs-lookup"><span data-stu-id="51e9e-135">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="51e9e-136">Нет</span><span class="sxs-lookup"><span data-stu-id="51e9e-136">None</span></span> |<span data-ttu-id="51e9e-137">Удаление определения schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="51e9e-137">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="51e9e-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="51e9e-138">Properties</span></span>
| <span data-ttu-id="51e9e-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="51e9e-139">Property</span></span>     | <span data-ttu-id="51e9e-140">Тип</span><span class="sxs-lookup"><span data-stu-id="51e9e-140">Type</span></span>   |<span data-ttu-id="51e9e-141">Описание</span><span class="sxs-lookup"><span data-stu-id="51e9e-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51e9e-142">description</span><span class="sxs-lookup"><span data-stu-id="51e9e-142">description</span></span>|<span data-ttu-id="51e9e-143">String</span><span class="sxs-lookup"><span data-stu-id="51e9e-143">String</span></span>|<span data-ttu-id="51e9e-144">Описание расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="51e9e-144">Description for the schema extension.</span></span>|
|<span data-ttu-id="51e9e-145">id</span><span class="sxs-lookup"><span data-stu-id="51e9e-145">id</span></span>|<span data-ttu-id="51e9e-146">Строка</span><span class="sxs-lookup"><span data-stu-id="51e9e-146">String</span></span>|<span data-ttu-id="51e9e-147">Уникальный идентификатор для определения расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="51e9e-147">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="51e9e-148">Значение можно присвоить одним из двух способов:</span><span class="sxs-lookup"><span data-stu-id="51e9e-148">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="51e9e-149">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span><span class="sxs-lookup"><span data-stu-id="51e9e-149">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span></span> <span data-ttu-id="51e9e-150">As an example, `contoso_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="51e9e-150">As an example, `contoso_mySchema`.</span></span> </li><li><span data-ttu-id="51e9e-151">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}.</span><span class="sxs-lookup"><span data-stu-id="51e9e-151">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}.</span></span> <span data-ttu-id="51e9e-152">An example would be `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="51e9e-152">An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="51e9e-153">После создания это свойство невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="51e9e-153">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="51e9e-154">owner</span><span class="sxs-lookup"><span data-stu-id="51e9e-154">owner</span></span>|<span data-ttu-id="51e9e-155">String</span><span class="sxs-lookup"><span data-stu-id="51e9e-155">String</span></span>|<span data-ttu-id="51e9e-156">Идентификатор `appId` приложения, которое является владельцем расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="51e9e-156">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="51e9e-157">Это свойство можно указать при создании, чтобы задать владельца.</span><span class="sxs-lookup"><span data-stu-id="51e9e-157">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="51e9e-158">Если оно не указано, то в качестве владельца будет задано вызывающее приложение `appId`.</span><span class="sxs-lookup"><span data-stu-id="51e9e-158">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="51e9e-159">В любом случае, пользователь, выполнивший вход в систему, должен быть владельцем приложения.</span><span class="sxs-lookup"><span data-stu-id="51e9e-159">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="51e9e-160">После задания свойства оно будет доступно только для чтения, и вам не удастся изменить его.</span><span class="sxs-lookup"><span data-stu-id="51e9e-160">Once set, this property is read-only and cannot be changed.</span></span>|
|<span data-ttu-id="51e9e-161">properties</span><span class="sxs-lookup"><span data-stu-id="51e9e-161">properties</span></span>|<span data-ttu-id="51e9e-162">Коллекция [extensionSchemaProperty](extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="51e9e-162">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="51e9e-163">Коллекция имен и типов свойств, составляющих определение расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="51e9e-163">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="51e9e-164">status</span><span class="sxs-lookup"><span data-stu-id="51e9e-164">status</span></span>|<span data-ttu-id="51e9e-165">String</span><span class="sxs-lookup"><span data-stu-id="51e9e-165">String</span></span>|<span data-ttu-id="51e9e-166">Состояние жизненного цикла расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="51e9e-166">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="51e9e-167">Возможные состояния: **InDevelopment**, **Available** и **Deprecated**.</span><span class="sxs-lookup"><span data-stu-id="51e9e-167">Possible states are **InDevelopment**, **Available**, and **Deprecated**.</span></span> <span data-ttu-id="51e9e-168">При создании свойство автоматически получает значение **InDevelopment**.</span><span class="sxs-lookup"><span data-stu-id="51e9e-168">Automatically set to **InDevelopment** on creation.</span></span> <span data-ttu-id="51e9e-169">[Расширения схемы](/graph/extensibility-overview#schema-extensions) предоставляют дополнительные сведения о возможных переходах из одного состояния в другое и о поведении.</span><span class="sxs-lookup"><span data-stu-id="51e9e-169">[Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span>|
|<span data-ttu-id="51e9e-170">targetTypes</span><span class="sxs-lookup"><span data-stu-id="51e9e-170">targetTypes</span></span>|<span data-ttu-id="51e9e-171">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="51e9e-171">String collection</span></span>|<span data-ttu-id="51e9e-172">Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы.</span><span class="sxs-lookup"><span data-stu-id="51e9e-172">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span> <span data-ttu-id="51e9e-173">Выберите из **administrativeUnit**, **контакта**, **устройства**, **события**, **группы**, **сообщения**, **Организации**, **записи**или **пользователя**.</span><span class="sxs-lookup"><span data-stu-id="51e9e-173">Select from **administrativeUnit**, **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="51e9e-174">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="51e9e-174">JSON representation</span></span>

<span data-ttu-id="51e9e-175">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51e9e-175">Here is a JSON representation of the resource.</span></span>

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
