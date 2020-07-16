---
title: Тип ресурса schemaExtension (расширения схемы)
description: 'С помощью расширений схемы вы можете задать схему, которую необходимо расширить, и добавить строго типизированные пользовательские данные в тип ресурса. В расширенном ресурсе пользовательские данные имеют сложный тип. '
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
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="13852-104">Тип ресурса schemaExtension (расширения схемы)</span><span class="sxs-lookup"><span data-stu-id="13852-104">schemaExtension resource type (schema extensions)</span></span>

<span data-ttu-id="13852-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13852-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13852-p102">С помощью расширений схемы вы можете задать схему, которую необходимо расширить, и добавить строго типизированные пользовательские данные в тип ресурса. В расширенном ресурсе пользовательские данные имеют сложный тип.</span><span class="sxs-lookup"><span data-stu-id="13852-p102">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="13852-108">Расширения схемы поддерживаются в ресурсах указанных ниже типов.</span><span class="sxs-lookup"><span data-stu-id="13852-108">Schema extensions are supported by the following resource types:</span></span>

- [<span data-ttu-id="13852-109">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="13852-109">administrativeUnit</span></span>](administrativeunit.md)
- [<span data-ttu-id="13852-110">contact</span><span class="sxs-lookup"><span data-stu-id="13852-110">contact</span></span>](contact.md)
- [<span data-ttu-id="13852-111">device</span><span class="sxs-lookup"><span data-stu-id="13852-111">device</span></span>](device.md)
- <span data-ttu-id="13852-112">[событие](event.md) для пользователя или календаря группы Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="13852-112">[event](event.md) on a user or Microsoft 365 group calendar</span></span>
- <span data-ttu-id="13852-113">[Публикация](post.md) группы Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="13852-113">[post](post.md) of a Microsoft 365 group</span></span>
- [<span data-ttu-id="13852-114">group</span><span class="sxs-lookup"><span data-stu-id="13852-114">group</span></span>](group.md)
- [<span data-ttu-id="13852-115">message</span><span class="sxs-lookup"><span data-stu-id="13852-115">message</span></span>](message.md) 
- [<span data-ttu-id="13852-116">organization</span><span class="sxs-lookup"><span data-stu-id="13852-116">organization</span></span>](organization.md)
- [<span data-ttu-id="13852-117">user</span><span class="sxs-lookup"><span data-stu-id="13852-117">user</span></span>](user.md)

<span data-ttu-id="13852-118">Сведения о том, как добавлять пользовательские данные в группы, см. в [примере расширения схемы](/graph/extensibility-schema-groups).</span><span class="sxs-lookup"><span data-stu-id="13852-118">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="13852-119">Методы</span><span class="sxs-lookup"><span data-stu-id="13852-119">Methods</span></span>

| <span data-ttu-id="13852-120">Метод</span><span class="sxs-lookup"><span data-stu-id="13852-120">Method</span></span>           | <span data-ttu-id="13852-121">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="13852-121">Return Type</span></span>    |<span data-ttu-id="13852-122">Описание</span><span class="sxs-lookup"><span data-stu-id="13852-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="13852-123">Создание</span><span class="sxs-lookup"><span data-stu-id="13852-123">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="13852-124">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="13852-124">schemaExtension</span></span> |<span data-ttu-id="13852-125">Создание определения расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="13852-125">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="13852-126">Перечисление</span><span class="sxs-lookup"><span data-stu-id="13852-126">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="13852-127">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="13852-127">schemaExtension</span></span> |<span data-ttu-id="13852-128">Перечислите аваиалбе schemaExtension дефинтионс и их свойства.</span><span class="sxs-lookup"><span data-stu-id="13852-128">List the avaialbe schemaExtension defintions and their properties.</span></span>|
|[<span data-ttu-id="13852-129">Получение</span><span class="sxs-lookup"><span data-stu-id="13852-129">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="13852-130">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="13852-130">schemaExtension</span></span> |<span data-ttu-id="13852-131">Получение свойств указанного определения schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="13852-131">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="13852-132">Обновление</span><span class="sxs-lookup"><span data-stu-id="13852-132">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="13852-133">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="13852-133">schemaExtension</span></span>   |<span data-ttu-id="13852-134">Обновление определения schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="13852-134">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="13852-135">Удаление</span><span class="sxs-lookup"><span data-stu-id="13852-135">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="13852-136">Нет</span><span class="sxs-lookup"><span data-stu-id="13852-136">None</span></span> |<span data-ttu-id="13852-137">Удаление определения schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="13852-137">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="13852-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="13852-138">Properties</span></span>
| <span data-ttu-id="13852-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="13852-139">Property</span></span>     | <span data-ttu-id="13852-140">Тип</span><span class="sxs-lookup"><span data-stu-id="13852-140">Type</span></span>   |<span data-ttu-id="13852-141">Описание</span><span class="sxs-lookup"><span data-stu-id="13852-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13852-142">description</span><span class="sxs-lookup"><span data-stu-id="13852-142">description</span></span>|<span data-ttu-id="13852-143">String</span><span class="sxs-lookup"><span data-stu-id="13852-143">String</span></span>|<span data-ttu-id="13852-144">Описание расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="13852-144">Description for the schema extension.</span></span>|
|<span data-ttu-id="13852-145">id</span><span class="sxs-lookup"><span data-stu-id="13852-145">id</span></span>|<span data-ttu-id="13852-146">Строка</span><span class="sxs-lookup"><span data-stu-id="13852-146">String</span></span>|<span data-ttu-id="13852-147">Уникальный идентификатор для определения расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="13852-147">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="13852-148">Значение можно присвоить одним из двух способов:</span><span class="sxs-lookup"><span data-stu-id="13852-148">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="13852-p103">Сцепите имя одного из ваших проверенных доменов с именем расширения схемы, чтобы создать уникальную строку такого формата: \{_&#65279;доменноеИмя_\}\_\{_&#65279;имяСхемы_\}. Например, `contoso_mySchema`. </span><span class="sxs-lookup"><span data-stu-id="13852-p103">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="13852-p104">Укажите имя схемы и предоставьте Microsoft Graph возможность использовать его для назначения **id** в таком формате: ext\{_&#65279;8-случайных-букв-или-цифр_\}\_\{_&#65279;имя-схемы_\}. Например, `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="13852-p104">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="13852-153">После создания это свойство невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="13852-153">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="13852-154">owner</span><span class="sxs-lookup"><span data-stu-id="13852-154">owner</span></span>|<span data-ttu-id="13852-155">String</span><span class="sxs-lookup"><span data-stu-id="13852-155">String</span></span>|<span data-ttu-id="13852-156">Идентификатор `appId` приложения, которое является владельцем расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="13852-156">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="13852-157">Это свойство можно указать при создании, чтобы задать владельца.</span><span class="sxs-lookup"><span data-stu-id="13852-157">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="13852-158">Если оно не указано, то в качестве владельца будет задано вызывающее приложение `appId`.</span><span class="sxs-lookup"><span data-stu-id="13852-158">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="13852-159">В любом случае, пользователь, выполнивший вход в систему, должен быть владельцем приложения.</span><span class="sxs-lookup"><span data-stu-id="13852-159">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="13852-160">После задания свойства оно будет доступно только для чтения, и вам не удастся изменить его.</span><span class="sxs-lookup"><span data-stu-id="13852-160">Once set, this property is read-only and cannot be changed.</span></span>|
|<span data-ttu-id="13852-161">properties</span><span class="sxs-lookup"><span data-stu-id="13852-161">properties</span></span>|<span data-ttu-id="13852-162">Коллекция [extensionSchemaProperty](extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="13852-162">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="13852-163">Коллекция имен и типов свойств, составляющих определение расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="13852-163">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="13852-164">status</span><span class="sxs-lookup"><span data-stu-id="13852-164">status</span></span>|<span data-ttu-id="13852-165">String</span><span class="sxs-lookup"><span data-stu-id="13852-165">String</span></span>|<span data-ttu-id="13852-166">Состояние жизненного цикла расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="13852-166">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="13852-167">Возможные состояния: **InDevelopment**, **Available** и **Deprecated**.</span><span class="sxs-lookup"><span data-stu-id="13852-167">Possible states are **InDevelopment**, **Available**, and **Deprecated**.</span></span> <span data-ttu-id="13852-168">При создании свойство автоматически получает значение **InDevelopment**.</span><span class="sxs-lookup"><span data-stu-id="13852-168">Automatically set to **InDevelopment** on creation.</span></span> <span data-ttu-id="13852-169">[Расширения схемы](/graph/extensibility-overview#schema-extensions) предоставляют дополнительные сведения о возможных переходах из одного состояния в другое и о поведении.</span><span class="sxs-lookup"><span data-stu-id="13852-169">[Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span>|
|<span data-ttu-id="13852-170">targetTypes</span><span class="sxs-lookup"><span data-stu-id="13852-170">targetTypes</span></span>|<span data-ttu-id="13852-171">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="13852-171">String collection</span></span>|<span data-ttu-id="13852-172">Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы.</span><span class="sxs-lookup"><span data-stu-id="13852-172">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span> <span data-ttu-id="13852-173">Выберите из **administrativeUnit**, **контакта**, **устройства**, **события**, **группы**, **сообщения**, **Организации**, **записи**или **пользователя**.</span><span class="sxs-lookup"><span data-stu-id="13852-173">Select from **administrativeUnit**, **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13852-174">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="13852-174">JSON representation</span></span>

<span data-ttu-id="13852-175">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13852-175">Here is a JSON representation of the resource.</span></span>

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
