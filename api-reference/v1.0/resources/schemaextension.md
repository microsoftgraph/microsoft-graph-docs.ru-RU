---
title: Тип ресурса schemaExtension (расширения схемы)
description: 'С помощью расширений схемы вы можете задать схему, которую необходимо расширить, и добавить строго типизированные пользовательские данные в тип ресурса. В расширенном ресурсе пользовательские данные имеют сложный тип. '
ms.openlocfilehash: 885b315897814cc15f83526086edb9cf298995f7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027348"
---
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="425d4-104">Тип ресурса schemaExtension (расширения схемы)</span><span class="sxs-lookup"><span data-stu-id="425d4-104">schemaExtension resource type (schema extensions)</span></span>

<span data-ttu-id="425d4-p102">С помощью расширений схемы вы можете задать схему, которую необходимо расширить, и добавить строго типизированные пользовательские данные в тип ресурса. В расширенном ресурсе пользовательские данные имеют сложный тип.</span><span class="sxs-lookup"><span data-stu-id="425d4-p102">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="425d4-107">Расширения схемы поддерживаются в ресурсах указанных ниже типов.</span><span class="sxs-lookup"><span data-stu-id="425d4-107">Schema extensions are supported by the following resource types:</span></span>

 - [<span data-ttu-id="425d4-108">contact</span><span class="sxs-lookup"><span data-stu-id="425d4-108">contact</span></span>](contact.md)
 - [<span data-ttu-id="425d4-109">device</span><span class="sxs-lookup"><span data-stu-id="425d4-109">device</span></span>](device.md)
 - <span data-ttu-id="425d4-110">[event](event.md) (для пользователя или календаря группы Office 365)</span><span class="sxs-lookup"><span data-stu-id="425d4-110">[event](event.md) on a user or Office 365 group calendar</span></span>
 - <span data-ttu-id="425d4-111">[post](post.md) (для группы Office 365)</span><span class="sxs-lookup"><span data-stu-id="425d4-111">[post](post.md) of an Office 365 group</span></span>
 - [<span data-ttu-id="425d4-112">group</span><span class="sxs-lookup"><span data-stu-id="425d4-112">group</span></span>](group.md)
 - [<span data-ttu-id="425d4-113">message</span><span class="sxs-lookup"><span data-stu-id="425d4-113">message</span></span>](message.md) 
 - [<span data-ttu-id="425d4-114">organization</span><span class="sxs-lookup"><span data-stu-id="425d4-114">organization</span></span>](organization.md)
 - [<span data-ttu-id="425d4-115">user</span><span class="sxs-lookup"><span data-stu-id="425d4-115">user</span></span>](user.md)

<span data-ttu-id="425d4-116">Сведения о том, как добавлять пользовательские данные в группы, см. в [примере расширения схемы](/graph/extensibility-schema-groups).</span><span class="sxs-lookup"><span data-stu-id="425d4-116">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="425d4-117">Методы</span><span class="sxs-lookup"><span data-stu-id="425d4-117">Methods</span></span>

| <span data-ttu-id="425d4-118">Метод</span><span class="sxs-lookup"><span data-stu-id="425d4-118">Method</span></span>           | <span data-ttu-id="425d4-119">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="425d4-119">Return Type</span></span>    |<span data-ttu-id="425d4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="425d4-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="425d4-121">Создание</span><span class="sxs-lookup"><span data-stu-id="425d4-121">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="425d4-122">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="425d4-122">schemaExtension</span></span> |<span data-ttu-id="425d4-123">Создание определения расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="425d4-123">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="425d4-124">Перечисление</span><span class="sxs-lookup"><span data-stu-id="425d4-124">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="425d4-125">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="425d4-125">schemaExtension</span></span> |<span data-ttu-id="425d4-126">Создание списка доступных определений schemaExtension и их свойств.</span><span class="sxs-lookup"><span data-stu-id="425d4-126">List the available schemaExtension definitions and their properties.</span></span>|
|[<span data-ttu-id="425d4-127">Получение</span><span class="sxs-lookup"><span data-stu-id="425d4-127">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="425d4-128">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="425d4-128">schemaExtension</span></span> |<span data-ttu-id="425d4-129">Получение свойств указанного определения schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="425d4-129">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="425d4-130">Обновление</span><span class="sxs-lookup"><span data-stu-id="425d4-130">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="425d4-131">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="425d4-131">schemaExtension</span></span>   |<span data-ttu-id="425d4-132">Обновление определения schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="425d4-132">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="425d4-133">Удаление</span><span class="sxs-lookup"><span data-stu-id="425d4-133">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="425d4-134">Нет</span><span class="sxs-lookup"><span data-stu-id="425d4-134">None</span></span> |<span data-ttu-id="425d4-135">Удаление определения schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="425d4-135">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="425d4-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="425d4-136">Properties</span></span>
| <span data-ttu-id="425d4-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="425d4-137">Property</span></span>     | <span data-ttu-id="425d4-138">Тип</span><span class="sxs-lookup"><span data-stu-id="425d4-138">Type</span></span>   |<span data-ttu-id="425d4-139">Описание</span><span class="sxs-lookup"><span data-stu-id="425d4-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="425d4-140">описание</span><span class="sxs-lookup"><span data-stu-id="425d4-140">description</span></span>|<span data-ttu-id="425d4-141">String</span><span class="sxs-lookup"><span data-stu-id="425d4-141">String</span></span>|<span data-ttu-id="425d4-142">Описание расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="425d4-142">Description for the schema extension.</span></span>|
|<span data-ttu-id="425d4-143">id</span><span class="sxs-lookup"><span data-stu-id="425d4-143">id</span></span>|<span data-ttu-id="425d4-144">String</span><span class="sxs-lookup"><span data-stu-id="425d4-144">String</span></span>|<span data-ttu-id="425d4-145">Уникальный идентификатор для определения расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="425d4-145">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="425d4-146">Значение можно присвоить одним из двух способов:</span><span class="sxs-lookup"><span data-stu-id="425d4-146">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="425d4-p103">Сцепите имя одного из ваших проверенных доменов с именем расширения схемы, чтобы создать уникальную строку такого формата: \{_&#65279;доменноеИмя_\}\_\{_&#65279;имяСхемы_\}. Например, `contoso_mySchema`. </span><span class="sxs-lookup"><span data-stu-id="425d4-p103">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="425d4-p104">Укажите имя схемы и предоставьте Microsoft Graph возможность использовать его для назначения **id** в таком формате: ext\{_&#65279;8-случайных-букв-или-цифр_\}\_\{_&#65279;имя-схемы_\}. Например, `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="425d4-p104">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="425d4-151">После создания это свойство невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="425d4-151">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="425d4-152">owner</span><span class="sxs-lookup"><span data-stu-id="425d4-152">owner</span></span>|<span data-ttu-id="425d4-153">String</span><span class="sxs-lookup"><span data-stu-id="425d4-153">String</span></span>|<span data-ttu-id="425d4-154">Идентификатор `appId` приложения, которое является владельцем расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="425d4-154">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="425d4-155">Это свойство можно указать при создании, чтобы задать владельца.</span><span class="sxs-lookup"><span data-stu-id="425d4-155">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="425d4-156">Если оно не указано, то в качестве владельца будет задано вызывающее приложение `appId`.</span><span class="sxs-lookup"><span data-stu-id="425d4-156">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="425d4-157">В любом случае, пользователь, выполнивший вход в систему, должен быть владельцем приложения.</span><span class="sxs-lookup"><span data-stu-id="425d4-157">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="425d4-158">После задания свойства оно будет доступно только для чтения, и вам не удастся изменить его.</span><span class="sxs-lookup"><span data-stu-id="425d4-158">Once set, this property is read-only and cannot be changed.</span></span>| 
|<span data-ttu-id="425d4-159">свойства</span><span class="sxs-lookup"><span data-stu-id="425d4-159">properties</span></span>|<span data-ttu-id="425d4-160">Коллекция [extensionSchemaProperty](extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="425d4-160">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="425d4-161">Коллекция имен и типов свойств, составляющих определение расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="425d4-161">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="425d4-162">status</span><span class="sxs-lookup"><span data-stu-id="425d4-162">status</span></span>|<span data-ttu-id="425d4-163">String</span><span class="sxs-lookup"><span data-stu-id="425d4-163">String</span></span>|<span data-ttu-id="425d4-p106">Состояние жизненного цикла расширения схемы. Возможные состояния: **InDevelopment**, **Available** и **Deprecated**. При создании свойство автоматически получает значение **InDevelopment**. [Расширения схемы](/graph/extensibility-overview#schema-extensions) предоставляют дополнительные сведения о возможных переходах из одного состояния в другое и об их поведении.</span><span class="sxs-lookup"><span data-stu-id="425d4-p106">The lifecycle state of the schema extension. Possible states are **InDevelopment**, **Available**, and **Deprecated**. Automatically set to **InDevelopment** on creation. [Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span>|
|<span data-ttu-id="425d4-168">targetTypes</span><span class="sxs-lookup"><span data-stu-id="425d4-168">targetTypes</span></span>|<span data-ttu-id="425d4-169">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="425d4-169">String collection</span></span>|<span data-ttu-id="425d4-p107">Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы. Возможные варианты: **contact**, **device**, **event**, **group**, **message**, **organization**, **post** или **user**.</span><span class="sxs-lookup"><span data-stu-id="425d4-p107">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to. Select from **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="425d4-172">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="425d4-172">JSON representation</span></span>

<span data-ttu-id="425d4-173">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="425d4-173">Here is a JSON representation of the resource.</span></span>

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