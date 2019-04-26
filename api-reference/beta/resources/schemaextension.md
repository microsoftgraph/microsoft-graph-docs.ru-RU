---
title: Тип ресурса schemaExtension (расширения схемы)
description: 'С помощью расширений схемы вы можете задать схему, которую необходимо расширить, и добавить строго типизированные пользовательские данные в тип ресурса. В расширенном ресурсе пользовательские данные имеют сложный тип. '
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: a6d7ed28b1fedefe1b4172bb780e3a014e4d3ff7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343472"
---
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="58a7d-104">Тип ресурса schemaExtension (расширения схемы)</span><span class="sxs-lookup"><span data-stu-id="58a7d-104">schemaExtension resource type (schema extensions)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58a7d-p102">С помощью расширений схемы вы можете задать схему, которую необходимо расширить, и добавить строго типизированные пользовательские данные в тип ресурса. В расширенном ресурсе пользовательские данные имеют сложный тип.</span><span class="sxs-lookup"><span data-stu-id="58a7d-p102">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="58a7d-107">Расширения схемы поддерживаются в ресурсах указанных ниже типов.</span><span class="sxs-lookup"><span data-stu-id="58a7d-107">Schema extensions are supported by the following resource types:</span></span>

 - [<span data-ttu-id="58a7d-108">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="58a7d-108">administrativeUnit</span></span>](administrativeunit.md)
 - [<span data-ttu-id="58a7d-109">contact</span><span class="sxs-lookup"><span data-stu-id="58a7d-109">contact</span></span>](contact.md)
 - [<span data-ttu-id="58a7d-110">device</span><span class="sxs-lookup"><span data-stu-id="58a7d-110">device</span></span>](device.md)
 - <span data-ttu-id="58a7d-111">[event](event.md) (для пользователя или календаря группы Office 365)</span><span class="sxs-lookup"><span data-stu-id="58a7d-111">[event](event.md) on a user or Office 365 group calendar</span></span>
 - <span data-ttu-id="58a7d-112">[post](post.md) (для группы Office 365)</span><span class="sxs-lookup"><span data-stu-id="58a7d-112">[post](post.md) of an Office 365 group</span></span>
 - [<span data-ttu-id="58a7d-113">group</span><span class="sxs-lookup"><span data-stu-id="58a7d-113">group</span></span>](group.md)
 - [<span data-ttu-id="58a7d-114">message</span><span class="sxs-lookup"><span data-stu-id="58a7d-114">message</span></span>](message.md) 
 - [<span data-ttu-id="58a7d-115">organization</span><span class="sxs-lookup"><span data-stu-id="58a7d-115">organization</span></span>](organization.md)
 - [<span data-ttu-id="58a7d-116">user</span><span class="sxs-lookup"><span data-stu-id="58a7d-116">user</span></span>](user.md)

<span data-ttu-id="58a7d-117">Сведения о том, как добавлять пользовательские данные в группы, см. в [примере расширения схемы](/graph/extensibility-schema-groups).</span><span class="sxs-lookup"><span data-stu-id="58a7d-117">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="58a7d-118">Методы</span><span class="sxs-lookup"><span data-stu-id="58a7d-118">Methods</span></span>

| <span data-ttu-id="58a7d-119">Метод</span><span class="sxs-lookup"><span data-stu-id="58a7d-119">Method</span></span>           | <span data-ttu-id="58a7d-120">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="58a7d-120">Return Type</span></span>    |<span data-ttu-id="58a7d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="58a7d-121">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="58a7d-122">Создание</span><span class="sxs-lookup"><span data-stu-id="58a7d-122">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="58a7d-123">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="58a7d-123">schemaExtension</span></span> |<span data-ttu-id="58a7d-124">Создание определения расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="58a7d-124">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="58a7d-125">Перечисление</span><span class="sxs-lookup"><span data-stu-id="58a7d-125">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="58a7d-126">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="58a7d-126">schemaExtension</span></span> |<span data-ttu-id="58a7d-127">ПереЧислите аваиалбе schemaExtension дефинтионс и их свойства.</span><span class="sxs-lookup"><span data-stu-id="58a7d-127">List the avaialbe schemaExtension defintions and their properties.</span></span>|
|[<span data-ttu-id="58a7d-128">Получение</span><span class="sxs-lookup"><span data-stu-id="58a7d-128">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="58a7d-129">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="58a7d-129">schemaExtension</span></span> |<span data-ttu-id="58a7d-130">Получение свойств указанного определения schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="58a7d-130">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="58a7d-131">Обновление</span><span class="sxs-lookup"><span data-stu-id="58a7d-131">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="58a7d-132">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="58a7d-132">schemaExtension</span></span>   |<span data-ttu-id="58a7d-133">Обновление определения schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="58a7d-133">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="58a7d-134">Удаление</span><span class="sxs-lookup"><span data-stu-id="58a7d-134">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="58a7d-135">Нет</span><span class="sxs-lookup"><span data-stu-id="58a7d-135">None</span></span> |<span data-ttu-id="58a7d-136">Удаление определения schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="58a7d-136">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="58a7d-137">Свойства</span><span class="sxs-lookup"><span data-stu-id="58a7d-137">Properties</span></span>
| <span data-ttu-id="58a7d-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="58a7d-138">Property</span></span>     | <span data-ttu-id="58a7d-139">Тип</span><span class="sxs-lookup"><span data-stu-id="58a7d-139">Type</span></span>   |<span data-ttu-id="58a7d-140">Описание</span><span class="sxs-lookup"><span data-stu-id="58a7d-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58a7d-141">description</span><span class="sxs-lookup"><span data-stu-id="58a7d-141">description</span></span>|<span data-ttu-id="58a7d-142">String</span><span class="sxs-lookup"><span data-stu-id="58a7d-142">String</span></span>|<span data-ttu-id="58a7d-143">Описание расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="58a7d-143">Description for the schema extension.</span></span>|
|<span data-ttu-id="58a7d-144">id</span><span class="sxs-lookup"><span data-stu-id="58a7d-144">id</span></span>|<span data-ttu-id="58a7d-145">Строка</span><span class="sxs-lookup"><span data-stu-id="58a7d-145">String</span></span>|<span data-ttu-id="58a7d-146">Уникальный идентификатор для определения расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="58a7d-146">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="58a7d-147">Значение можно присвоить одним из двух способов:</span><span class="sxs-lookup"><span data-stu-id="58a7d-147">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="58a7d-p103">Сцепите имя одного из ваших проверенных доменов с именем расширения схемы, чтобы создать уникальную строку такого формата: \{_&#65279;доменноеИмя_\}\_\{_&#65279;имяСхемы_\}. Например, `contoso_mySchema`. </span><span class="sxs-lookup"><span data-stu-id="58a7d-p103">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="58a7d-p104">Укажите имя схемы и предоставьте Microsoft Graph возможность использовать его для назначения **id** в таком формате: ext\{_&#65279;8-случайных-букв-или-цифр_\}\_\{_&#65279;имя-схемы_\}. Например, `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="58a7d-p104">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="58a7d-152">После создания это свойство невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="58a7d-152">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="58a7d-153">owner</span><span class="sxs-lookup"><span data-stu-id="58a7d-153">owner</span></span>|<span data-ttu-id="58a7d-154">String</span><span class="sxs-lookup"><span data-stu-id="58a7d-154">String</span></span>|<span data-ttu-id="58a7d-155">Идентификатор `appId` приложения, которое является владельцем расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="58a7d-155">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="58a7d-156">Это свойство можно указать при создании, чтобы задать владельца.</span><span class="sxs-lookup"><span data-stu-id="58a7d-156">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="58a7d-157">Если оно не указано, то в качестве владельца будет задано вызывающее приложение `appId`.</span><span class="sxs-lookup"><span data-stu-id="58a7d-157">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="58a7d-158">В любом случае, пользователь, выполнивший вход в систему, должен быть владельцем приложения.</span><span class="sxs-lookup"><span data-stu-id="58a7d-158">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="58a7d-159">После задания свойства оно будет доступно только для чтения, и вам не удастся изменить его.</span><span class="sxs-lookup"><span data-stu-id="58a7d-159">Once set, this property is read-only and cannot be changed.</span></span>|
|<span data-ttu-id="58a7d-160">properties</span><span class="sxs-lookup"><span data-stu-id="58a7d-160">properties</span></span>|<span data-ttu-id="58a7d-161">Коллекция [extensionSchemaProperty](extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="58a7d-161">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="58a7d-162">Коллекция имен и типов свойств, составляющих определение расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="58a7d-162">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="58a7d-163">status</span><span class="sxs-lookup"><span data-stu-id="58a7d-163">status</span></span>|<span data-ttu-id="58a7d-164">String</span><span class="sxs-lookup"><span data-stu-id="58a7d-164">String</span></span>|<span data-ttu-id="58a7d-165">Состояние жизненного цикла расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="58a7d-165">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="58a7d-166">Возможные состояния: **InDevelopment**, **Available** и **Deprecated**.</span><span class="sxs-lookup"><span data-stu-id="58a7d-166">Possible states are **InDevelopment**, **Available**, and **Deprecated**.</span></span> <span data-ttu-id="58a7d-167">При создании свойство автоматически получает значение **InDevelopment**.</span><span class="sxs-lookup"><span data-stu-id="58a7d-167">Automatically set to **InDevelopment** on creation.</span></span> <span data-ttu-id="58a7d-168">[Расширения схемы](/graph/extensibility-overview#schema-extensions) предоставляют дополнительные сведения о возможных переходах из одного состояния в другое и о поведении.</span><span class="sxs-lookup"><span data-stu-id="58a7d-168">[Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span>|
|<span data-ttu-id="58a7d-169">targetTypes</span><span class="sxs-lookup"><span data-stu-id="58a7d-169">targetTypes</span></span>|<span data-ttu-id="58a7d-170">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="58a7d-170">String collection</span></span>|<span data-ttu-id="58a7d-171">Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы.</span><span class="sxs-lookup"><span data-stu-id="58a7d-171">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span> <span data-ttu-id="58a7d-172">Выберите из **administrativeUnit**, **контакта**, **устройства**, **события**, **группы**, **сообщения**, **Организации**, **записи**или **пользователя**.</span><span class="sxs-lookup"><span data-stu-id="58a7d-172">Select from **administrativeUnit**, **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="58a7d-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="58a7d-173">JSON representation</span></span>

<span data-ttu-id="58a7d-174">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58a7d-174">Here is a JSON representation of the resource.</span></span>

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
