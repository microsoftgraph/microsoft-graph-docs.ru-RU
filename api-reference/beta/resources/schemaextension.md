---
title: Тип ресурса schemaExtension (расширения схемы)
description: 'С помощью расширений схемы вы можете задать схему, которую необходимо расширить, и добавить строго типизированные пользовательские данные в тип ресурса. В расширенном ресурсе пользовательские данные имеют сложный тип. '
localization_priority: Normal
author: dkershaw10
doc_type: resourcePageType
ms.prod: extensions
ms.openlocfilehash: 63cd126a37e1f21ff8020937d60eb769622aa1b6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083955"
---
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="f47b0-104">Тип ресурса schemaExtension (расширения схемы)</span><span class="sxs-lookup"><span data-stu-id="f47b0-104">schemaExtension resource type (schema extensions)</span></span>

<span data-ttu-id="f47b0-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f47b0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f47b0-p102">С помощью расширений схемы вы можете задать схему, которую необходимо расширить, и добавить строго типизированные пользовательские данные в тип ресурса. В расширенном ресурсе пользовательские данные имеют сложный тип.</span><span class="sxs-lookup"><span data-stu-id="f47b0-p102">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="f47b0-108">Расширения схемы поддерживаются в ресурсах указанных ниже типов.</span><span class="sxs-lookup"><span data-stu-id="f47b0-108">Schema extensions are supported by the following resource types:</span></span>

- [<span data-ttu-id="f47b0-109">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="f47b0-109">administrativeUnit</span></span>](administrativeunit.md)
- [<span data-ttu-id="f47b0-110">contact</span><span class="sxs-lookup"><span data-stu-id="f47b0-110">contact</span></span>](contact.md)
- [<span data-ttu-id="f47b0-111">device</span><span class="sxs-lookup"><span data-stu-id="f47b0-111">device</span></span>](device.md)
- <span data-ttu-id="f47b0-112">[event](event.md) (для пользователя или календаря группы Microsoft 365)</span><span class="sxs-lookup"><span data-stu-id="f47b0-112">[event](event.md) on a user or Microsoft 365 group calendar</span></span>
- <span data-ttu-id="f47b0-113">[post](post.md) (для группы Microsoft 365)</span><span class="sxs-lookup"><span data-stu-id="f47b0-113">[post](post.md) of a Microsoft 365 group</span></span>
- [<span data-ttu-id="f47b0-114">group</span><span class="sxs-lookup"><span data-stu-id="f47b0-114">group</span></span>](group.md)
- [<span data-ttu-id="f47b0-115">message</span><span class="sxs-lookup"><span data-stu-id="f47b0-115">message</span></span>](message.md) 
- [<span data-ttu-id="f47b0-116">organization</span><span class="sxs-lookup"><span data-stu-id="f47b0-116">organization</span></span>](organization.md)
- [<span data-ttu-id="f47b0-117">user</span><span class="sxs-lookup"><span data-stu-id="f47b0-117">user</span></span>](user.md)

<span data-ttu-id="f47b0-118">Сведения о том, как добавлять пользовательские данные в группы, см. в [примере расширения схемы](/graph/extensibility-schema-groups).</span><span class="sxs-lookup"><span data-stu-id="f47b0-118">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="f47b0-119">Методы</span><span class="sxs-lookup"><span data-stu-id="f47b0-119">Methods</span></span>

| <span data-ttu-id="f47b0-120">Метод</span><span class="sxs-lookup"><span data-stu-id="f47b0-120">Method</span></span>           | <span data-ttu-id="f47b0-121">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f47b0-121">Return Type</span></span>    |<span data-ttu-id="f47b0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f47b0-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f47b0-123">Создание</span><span class="sxs-lookup"><span data-stu-id="f47b0-123">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="f47b0-124">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="f47b0-124">schemaExtension</span></span> |<span data-ttu-id="f47b0-125">Создание определения расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="f47b0-125">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="f47b0-126">Перечисление</span><span class="sxs-lookup"><span data-stu-id="f47b0-126">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="f47b0-127">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="f47b0-127">schemaExtension</span></span> |<span data-ttu-id="f47b0-128">Перечислите аваиалбе schemaExtension дефинтионс и их свойства.</span><span class="sxs-lookup"><span data-stu-id="f47b0-128">List the avaialbe schemaExtension defintions and their properties.</span></span>|
|[<span data-ttu-id="f47b0-129">Получение</span><span class="sxs-lookup"><span data-stu-id="f47b0-129">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="f47b0-130">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="f47b0-130">schemaExtension</span></span> |<span data-ttu-id="f47b0-131">Получение свойств указанного определения schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="f47b0-131">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="f47b0-132">Обновление</span><span class="sxs-lookup"><span data-stu-id="f47b0-132">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="f47b0-133">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="f47b0-133">schemaExtension</span></span>   |<span data-ttu-id="f47b0-134">Обновление определения schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="f47b0-134">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="f47b0-135">Удаление</span><span class="sxs-lookup"><span data-stu-id="f47b0-135">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="f47b0-136">Нет</span><span class="sxs-lookup"><span data-stu-id="f47b0-136">None</span></span> |<span data-ttu-id="f47b0-137">Удаление определения schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="f47b0-137">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="f47b0-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="f47b0-138">Properties</span></span>
| <span data-ttu-id="f47b0-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="f47b0-139">Property</span></span>     | <span data-ttu-id="f47b0-140">Тип</span><span class="sxs-lookup"><span data-stu-id="f47b0-140">Type</span></span>   |<span data-ttu-id="f47b0-141">Описание</span><span class="sxs-lookup"><span data-stu-id="f47b0-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f47b0-142">description</span><span class="sxs-lookup"><span data-stu-id="f47b0-142">description</span></span>|<span data-ttu-id="f47b0-143">String</span><span class="sxs-lookup"><span data-stu-id="f47b0-143">String</span></span>|<span data-ttu-id="f47b0-144">Описание расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="f47b0-144">Description for the schema extension.</span></span>|
|<span data-ttu-id="f47b0-145">id</span><span class="sxs-lookup"><span data-stu-id="f47b0-145">id</span></span>|<span data-ttu-id="f47b0-146">String</span><span class="sxs-lookup"><span data-stu-id="f47b0-146">String</span></span>|<span data-ttu-id="f47b0-147">Уникальный идентификатор для определения расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="f47b0-147">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="f47b0-148">Значение можно присвоить одним из двух способов:</span><span class="sxs-lookup"><span data-stu-id="f47b0-148">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="f47b0-p103">Сцепите имя одного из ваших проверенных доменов с именем расширения схемы, чтобы создать уникальную строку такого формата: \{_&#65279;доменноеИмя_\}\_\{_&#65279;имяСхемы_\}. Например, `contoso_mySchema`. </span><span class="sxs-lookup"><span data-stu-id="f47b0-p103">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="f47b0-p104">Укажите имя схемы и предоставьте Microsoft Graph возможность использовать его для назначения **id** в таком формате: ext\{_&#65279;8-случайных-букв-или-цифр_\}\_\{_&#65279;имя-схемы_\}. Например, `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="f47b0-p104">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="f47b0-153">После создания это свойство невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="f47b0-153">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="f47b0-154">owner</span><span class="sxs-lookup"><span data-stu-id="f47b0-154">owner</span></span>|<span data-ttu-id="f47b0-155">String</span><span class="sxs-lookup"><span data-stu-id="f47b0-155">String</span></span>|<span data-ttu-id="f47b0-156">Идентификатор `appId` приложения, которое является владельцем расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="f47b0-156">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="f47b0-157">Это свойство можно указать при создании, чтобы задать владельца.</span><span class="sxs-lookup"><span data-stu-id="f47b0-157">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="f47b0-158">Если оно не указано, то в качестве владельца будет задано вызывающее приложение `appId`.</span><span class="sxs-lookup"><span data-stu-id="f47b0-158">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="f47b0-159">В любом случае, пользователь, выполнивший вход в систему, должен быть владельцем приложения.</span><span class="sxs-lookup"><span data-stu-id="f47b0-159">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="f47b0-160">После задания свойства оно будет доступно только для чтения, и вам не удастся изменить его.</span><span class="sxs-lookup"><span data-stu-id="f47b0-160">Once set, this property is read-only and cannot be changed.</span></span>|
|<span data-ttu-id="f47b0-161">properties</span><span class="sxs-lookup"><span data-stu-id="f47b0-161">properties</span></span>|<span data-ttu-id="f47b0-162">Коллекция [extensionSchemaProperty](extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="f47b0-162">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="f47b0-163">Коллекция имен и типов свойств, составляющих определение расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="f47b0-163">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="f47b0-164">status</span><span class="sxs-lookup"><span data-stu-id="f47b0-164">status</span></span>|<span data-ttu-id="f47b0-165">String</span><span class="sxs-lookup"><span data-stu-id="f47b0-165">String</span></span>|<span data-ttu-id="f47b0-166">Состояние жизненного цикла расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="f47b0-166">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="f47b0-167">Возможные состояния: **InDevelopment**, **Available** и **Deprecated**.</span><span class="sxs-lookup"><span data-stu-id="f47b0-167">Possible states are **InDevelopment**, **Available**, and **Deprecated**.</span></span> <span data-ttu-id="f47b0-168">При создании свойство автоматически получает значение **InDevelopment**.</span><span class="sxs-lookup"><span data-stu-id="f47b0-168">Automatically set to **InDevelopment** on creation.</span></span> <span data-ttu-id="f47b0-169">[Расширения схемы](/graph/extensibility-overview#schema-extensions) предоставляют дополнительные сведения о возможных переходах из одного состояния в другое и о поведении.</span><span class="sxs-lookup"><span data-stu-id="f47b0-169">[Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span>|
|<span data-ttu-id="f47b0-170">targetTypes</span><span class="sxs-lookup"><span data-stu-id="f47b0-170">targetTypes</span></span>|<span data-ttu-id="f47b0-171">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f47b0-171">String collection</span></span>|<span data-ttu-id="f47b0-172">Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы.</span><span class="sxs-lookup"><span data-stu-id="f47b0-172">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span> <span data-ttu-id="f47b0-173">Выберите из **administrativeUnit**, **контакта**, **устройства**, **события**, **группы**, **сообщения**, **Организации**, **записи**или **пользователя**.</span><span class="sxs-lookup"><span data-stu-id="f47b0-173">Select from **administrativeUnit**, **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f47b0-174">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f47b0-174">JSON representation</span></span>

<span data-ttu-id="f47b0-175">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f47b0-175">Here is a JSON representation of the resource.</span></span>

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


