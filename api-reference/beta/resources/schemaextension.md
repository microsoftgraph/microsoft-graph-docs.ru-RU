---
title: Тип ресурса schemaExtension (расширения схемы)
description: 'С помощью расширений схемы вы можете задать схему, которую необходимо расширить, и добавить строго типизированные пользовательские данные в тип ресурса. В расширенном ресурсе пользовательские данные имеют сложный тип. '
localization_priority: Normal
ms.openlocfilehash: df0b362e87fa0f8cf836c27e89a5fdebd4ab0de8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894504"
---
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="cc253-104">Тип ресурса schemaExtension (расширения схемы)</span><span class="sxs-lookup"><span data-stu-id="cc253-104">schemaExtension resource type (schema extensions)</span></span>

> <span data-ttu-id="cc253-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cc253-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc253-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc253-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cc253-p103">С помощью расширений схемы вы можете задать схему, которую необходимо расширить, и добавить строго типизированные пользовательские данные в тип ресурса. В расширенном ресурсе пользовательские данные имеют сложный тип.</span><span class="sxs-lookup"><span data-stu-id="cc253-p103">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="cc253-109">Расширения схемы поддерживаются в ресурсах указанных ниже типов.</span><span class="sxs-lookup"><span data-stu-id="cc253-109">Schema extensions are supported by the following resource types:</span></span>

 - [<span data-ttu-id="cc253-110">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="cc253-110">administrativeUnit</span></span>](administrativeunit.md)
 - [<span data-ttu-id="cc253-111">contact</span><span class="sxs-lookup"><span data-stu-id="cc253-111">contact</span></span>](contact.md)
 - [<span data-ttu-id="cc253-112">device</span><span class="sxs-lookup"><span data-stu-id="cc253-112">device</span></span>](device.md)
 - <span data-ttu-id="cc253-113">[event](event.md) (для пользователя или календаря группы Office 365)</span><span class="sxs-lookup"><span data-stu-id="cc253-113">[event](event.md) on a user or Office 365 group calendar</span></span>
 - <span data-ttu-id="cc253-114">[post](post.md) (для группы Office 365)</span><span class="sxs-lookup"><span data-stu-id="cc253-114">[post](post.md) of an Office 365 group</span></span>
 - [<span data-ttu-id="cc253-115">group</span><span class="sxs-lookup"><span data-stu-id="cc253-115">group</span></span>](group.md)
 - [<span data-ttu-id="cc253-116">message</span><span class="sxs-lookup"><span data-stu-id="cc253-116">message</span></span>](message.md) 
 - [<span data-ttu-id="cc253-117">organization</span><span class="sxs-lookup"><span data-stu-id="cc253-117">organization</span></span>](organization.md)
 - [<span data-ttu-id="cc253-118">user</span><span class="sxs-lookup"><span data-stu-id="cc253-118">user</span></span>](user.md)

<span data-ttu-id="cc253-119">Сведения о том, как добавлять пользовательские данные в группы, см. в [примере расширения схемы](/graph/extensibility-schema-groups).</span><span class="sxs-lookup"><span data-stu-id="cc253-119">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="cc253-120">Методы</span><span class="sxs-lookup"><span data-stu-id="cc253-120">Methods</span></span>

| <span data-ttu-id="cc253-121">Метод</span><span class="sxs-lookup"><span data-stu-id="cc253-121">Method</span></span>           | <span data-ttu-id="cc253-122">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cc253-122">Return Type</span></span>    |<span data-ttu-id="cc253-123">Описание</span><span class="sxs-lookup"><span data-stu-id="cc253-123">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cc253-124">Создание</span><span class="sxs-lookup"><span data-stu-id="cc253-124">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="cc253-125">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="cc253-125">schemaExtension</span></span> |<span data-ttu-id="cc253-126">Создание определения расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="cc253-126">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="cc253-127">Перечисление</span><span class="sxs-lookup"><span data-stu-id="cc253-127">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="cc253-128">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="cc253-128">schemaExtension</span></span> |<span data-ttu-id="cc253-129">Список файлов определения schemaExtension avaialbe и их свойства.</span><span class="sxs-lookup"><span data-stu-id="cc253-129">List the avaialbe schemaExtension defintions and their properties.</span></span>|
|[<span data-ttu-id="cc253-130">Получение</span><span class="sxs-lookup"><span data-stu-id="cc253-130">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="cc253-131">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="cc253-131">schemaExtension</span></span> |<span data-ttu-id="cc253-132">Получение свойств указанного определения schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="cc253-132">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="cc253-133">Обновление</span><span class="sxs-lookup"><span data-stu-id="cc253-133">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="cc253-134">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="cc253-134">schemaExtension</span></span>   |<span data-ttu-id="cc253-135">Обновление определения schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="cc253-135">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="cc253-136">Удаление</span><span class="sxs-lookup"><span data-stu-id="cc253-136">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="cc253-137">Нет</span><span class="sxs-lookup"><span data-stu-id="cc253-137">None</span></span> |<span data-ttu-id="cc253-138">Удаление определения schemaExtension.</span><span class="sxs-lookup"><span data-stu-id="cc253-138">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="cc253-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="cc253-139">Properties</span></span>
| <span data-ttu-id="cc253-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc253-140">Property</span></span>     | <span data-ttu-id="cc253-141">Тип</span><span class="sxs-lookup"><span data-stu-id="cc253-141">Type</span></span>   |<span data-ttu-id="cc253-142">Описание</span><span class="sxs-lookup"><span data-stu-id="cc253-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc253-143">описание</span><span class="sxs-lookup"><span data-stu-id="cc253-143">description</span></span>|<span data-ttu-id="cc253-144">String</span><span class="sxs-lookup"><span data-stu-id="cc253-144">String</span></span>|<span data-ttu-id="cc253-145">Описание расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="cc253-145">Description for the schema extension.</span></span>|
|<span data-ttu-id="cc253-146">id</span><span class="sxs-lookup"><span data-stu-id="cc253-146">id</span></span>|<span data-ttu-id="cc253-147">String</span><span class="sxs-lookup"><span data-stu-id="cc253-147">String</span></span>|<span data-ttu-id="cc253-148">Уникальный идентификатор для определения расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="cc253-148">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="cc253-149">Значение можно присвоить одним из двух способов:</span><span class="sxs-lookup"><span data-stu-id="cc253-149">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="cc253-p104">Сцепите имя одного из ваших проверенных доменов с именем расширения схемы, чтобы создать уникальную строку такого формата: \{_&#65279;доменноеИмя_\}\_\{_&#65279;имяСхемы_\}. Например, `contoso_mySchema`. </span><span class="sxs-lookup"><span data-stu-id="cc253-p104">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="cc253-p105">Укажите имя схемы и предоставьте Microsoft Graph возможность использовать его для назначения **id** в таком формате: ext\{_&#65279;8-случайных-букв-или-цифр_\}\_\{_&#65279;имя-схемы_\}. Например, `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="cc253-p105">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="cc253-154">После создания это свойство невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="cc253-154">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="cc253-155">owner</span><span class="sxs-lookup"><span data-stu-id="cc253-155">owner</span></span>|<span data-ttu-id="cc253-156">String</span><span class="sxs-lookup"><span data-stu-id="cc253-156">String</span></span>|<span data-ttu-id="cc253-157">Идентификатор `appId` приложения, которое является владельцем расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="cc253-157">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="cc253-158">Это свойство можно указать при создании, чтобы задать владельца.</span><span class="sxs-lookup"><span data-stu-id="cc253-158">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="cc253-159">Если оно не указано, то в качестве владельца будет задано вызывающее приложение `appId`.</span><span class="sxs-lookup"><span data-stu-id="cc253-159">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="cc253-160">В любом случае, пользователь, выполнивший вход в систему, должен быть владельцем приложения.</span><span class="sxs-lookup"><span data-stu-id="cc253-160">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="cc253-161">После задания свойства оно будет доступно только для чтения, и вам не удастся изменить его.</span><span class="sxs-lookup"><span data-stu-id="cc253-161">Once set, this property is read-only and cannot be changed.</span></span>|
|<span data-ttu-id="cc253-162">свойства</span><span class="sxs-lookup"><span data-stu-id="cc253-162">properties</span></span>|<span data-ttu-id="cc253-163">Коллекция [extensionSchemaProperty](extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="cc253-163">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="cc253-164">Коллекция имен и типов свойств, составляющих определение расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="cc253-164">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="cc253-165">status</span><span class="sxs-lookup"><span data-stu-id="cc253-165">status</span></span>|<span data-ttu-id="cc253-166">Строка</span><span class="sxs-lookup"><span data-stu-id="cc253-166">String</span></span>|<span data-ttu-id="cc253-p107">Состояние жизненного цикла расширения схемы. Возможные состояния: **InDevelopment**, **Available** и **Deprecated**. При создании свойство автоматически получает значение **InDevelopment**. [Расширения схемы](/graph/extensibility-overview#schema-extensions) предоставляют дополнительные сведения о возможных переходах из одного состояния в другое и об их поведении.</span><span class="sxs-lookup"><span data-stu-id="cc253-p107">The lifecycle state of the schema extension. Possible states are **InDevelopment**, **Available**, and **Deprecated**. Automatically set to **InDevelopment** on creation. [Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span>|
|<span data-ttu-id="cc253-171">targetTypes</span><span class="sxs-lookup"><span data-stu-id="cc253-171">targetTypes</span></span>|<span data-ttu-id="cc253-172">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cc253-172">String collection</span></span>|<span data-ttu-id="cc253-173">Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы.</span><span class="sxs-lookup"><span data-stu-id="cc253-173">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span> <span data-ttu-id="cc253-174">Выберите из **administrativeUnit**, **контактов**, **устройства**, **события**, **группы**, **сообщения**, **организации**, **Публикация**или **пользователя**.</span><span class="sxs-lookup"><span data-stu-id="cc253-174">Select from **administrativeUnit**, **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cc253-175">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cc253-175">JSON representation</span></span>

<span data-ttu-id="cc253-176">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc253-176">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "schemaExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
