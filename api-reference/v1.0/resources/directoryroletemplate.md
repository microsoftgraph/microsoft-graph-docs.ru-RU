---
title: Тип ресурса directoryRoleTemplate
description: 'Представляет шаблон роли каталога. Шаблон роли каталога определяет значения свойств роли каталога (directoryRole). Существует связанный объект шаблона роли каталога для каждой роли каталога, которая может быть активирована в клиенте. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируется только роль каталога администраторов организации. Чтобы активировать другие доступные роли каталога, вы отправляете запрос POST в `/directoryRoles` конечную точку с идентификатором шаблона роли каталога, на котором основана роль каталога, указанной в параметре **ролетемплатеид** запроса. После успешного завершения этого запроса можно начать чтение и назначить роль каталога. **Note**: шаблон роли каталога предоставляется для роли каталога Users. Роль каталога Users является неявной и невидимой для клиентов службы каталогов. Все пользователи в клиенте назначают эту роль инфраструктурой. Роль уже активирована. Не используйте этот шаблон.'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fdacca1f601485e48767364ef99911d061be17e0
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34658003"
---
# <a name="directoryroletemplate-resource-type"></a><span data-ttu-id="c6ccb-114">Тип ресурса directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="c6ccb-114">directoryRoleTemplate resource type</span></span>

<span data-ttu-id="c6ccb-p102">Представляет шаблон роли каталога. Шаблон роли каталога определяет значения свойств, принадлежащих роли каталога ([directoryRole](directoryrole.md)). С каждой ролью каталога, которую можно активировать на клиенте, связан объект соответствующего шаблона. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируется только роль каталога администраторов организации. Чтобы активировать другие доступные роли каталога, следует отправить запрос POST в конечную точку `/directoryRoles` с идентификатором шаблона роли каталога, на базе которого создана роль каталога и который указан в параметре **roleTemplateId** запроса. После успешного завершения этого запроса можно начинать считывание и назначение членов для роли каталога. **Примечание.** Шаблон роли каталога отображается вместо роли каталога пользователей. Роль каталога пользователей — неявная и невидимая для клиентов каталога. Каждый пользователь на клиенте назначается для этой роли инфраструктурой. Роль уже активирована. Не используйте этот шаблон.</span><span class="sxs-lookup"><span data-stu-id="c6ccb-p102">Represents a directory role template. A directory role template specifies the property values of a directory role ([directoryRole](directoryrole.md)). There is an associated directory role template object for each of the directory roles that may be activated in a tenant. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles you send a POST request to the `/directoryRoles` endpoint with the ID of the directory role template on which the directory role is based specified in the **roleTemplateId** parameter of the request. Upon successful completion of this request, you can then start to read and assign members to the directory role. **Note**: A directory role template is exposed for the Users directory role. The Users directory role is implicit and is not visible to directory clients. Every User in the tenant is assigned to this role by the infrastructure. The role is already activated. Do not use this template.</span></span>


## <a name="methods"></a><span data-ttu-id="c6ccb-127">Методы</span><span class="sxs-lookup"><span data-stu-id="c6ccb-127">Methods</span></span>

| <span data-ttu-id="c6ccb-128">Метод</span><span class="sxs-lookup"><span data-stu-id="c6ccb-128">Method</span></span>       | <span data-ttu-id="c6ccb-129">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c6ccb-129">Return Type</span></span>  |<span data-ttu-id="c6ccb-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c6ccb-130">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c6ccb-131">Получение directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="c6ccb-131">Get directoryRoleTemplate</span></span>](../api/directoryroletemplate-get.md) | [<span data-ttu-id="c6ccb-132">directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="c6ccb-132">directoryRoleTemplate</span></span>](directoryroletemplate.md) |<span data-ttu-id="c6ccb-133">Считывание свойств и отношений объекта directoryRoleTemplate.</span><span class="sxs-lookup"><span data-stu-id="c6ccb-133">Read properties and relationships of directoryRoleTemplate object.</span></span>|
|[<span data-ttu-id="c6ccb-134">Список объектов directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="c6ccb-134">List directoryRoleTemplate</span></span>](../api/directoryroletemplate-list.md) | <span data-ttu-id="c6ccb-135">Коллекция объектов [directoryRoleTemplate](directoryroletemplate.md)</span><span class="sxs-lookup"><span data-stu-id="c6ccb-135">[directoryRoleTemplate](directoryroletemplate.md) collection</span></span> |<span data-ttu-id="c6ccb-136">Получение списка объектов directoryRoleTemplate.</span><span class="sxs-lookup"><span data-stu-id="c6ccb-136">Retrieve a list of directoryRoleTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="c6ccb-137">Свойства</span><span class="sxs-lookup"><span data-stu-id="c6ccb-137">Properties</span></span>
| <span data-ttu-id="c6ccb-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="c6ccb-138">Property</span></span>     | <span data-ttu-id="c6ccb-139">Тип</span><span class="sxs-lookup"><span data-stu-id="c6ccb-139">Type</span></span>   |<span data-ttu-id="c6ccb-140">Описание</span><span class="sxs-lookup"><span data-stu-id="c6ccb-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6ccb-141">description</span><span class="sxs-lookup"><span data-stu-id="c6ccb-141">description</span></span>|<span data-ttu-id="c6ccb-142">String</span><span class="sxs-lookup"><span data-stu-id="c6ccb-142">String</span></span>|<span data-ttu-id="c6ccb-p103">Описание, которое нужно задать для роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c6ccb-p103">The description to set for the directory role. Read-only.</span></span>|
|<span data-ttu-id="c6ccb-145">displayName</span><span class="sxs-lookup"><span data-stu-id="c6ccb-145">displayName</span></span>|<span data-ttu-id="c6ccb-146">Строка</span><span class="sxs-lookup"><span data-stu-id="c6ccb-146">String</span></span>|<span data-ttu-id="c6ccb-p104">Отображаемое имя, которое нужно назначить роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c6ccb-p104">The display name to set for the directory role. Read-only.</span></span> |
|<span data-ttu-id="c6ccb-149">id</span><span class="sxs-lookup"><span data-stu-id="c6ccb-149">id</span></span>|<span data-ttu-id="c6ccb-150">String</span><span class="sxs-lookup"><span data-stu-id="c6ccb-150">String</span></span>|<span data-ttu-id="c6ccb-p105">Уникальный идентификатор шаблона. Наследуется из [directoryObject](directoryobject.md). Следует указать свойство **id** для шаблона роли каталога, чтобы свойство **roleTemplateId** в запросе POST активировало [directoryRole](directoryrole.md) на клиенте. Ключ, значение null не допускается. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c6ccb-p105">The unique identifier for the template. Inherited from [directoryObject](directoryobject.md). You specify the **id** of the directory role template for the **roleTemplateId** property in the POST request activate a [directoryRole](directoryrole.md) in a tenant. Key, Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6ccb-156">Отношения</span><span class="sxs-lookup"><span data-stu-id="c6ccb-156">Relationships</span></span>
<span data-ttu-id="c6ccb-157">Нет</span><span class="sxs-lookup"><span data-stu-id="c6ccb-157">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="c6ccb-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c6ccb-158">JSON representation</span></span>

<span data-ttu-id="c6ccb-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c6ccb-159">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.directoryRoleTemplate",
  "@odata.annotations": [
    {
      "capabilities": {
        "toppable": false
      }
    }
  ]
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRoleTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
