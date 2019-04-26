---
title: Тип ресурса directoryRoleTemplate
description: 'Представляет шаблон роли каталога. Шаблон роли каталога определяет значения свойств роли каталога (directoryRole). Существует связанный объект шаблона роли каталога для каждой роли каталога, которая может быть активирована в клиенте. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активирована только роль каталога администраторов компании. Чтобы активировать другие доступные роли каталога, вы отправляете запрос POST в `/directoryRoles` конечную точку с идентификатором шаблона роли каталога, на котором основана роль каталога, указанной в параметре **ролетемплатеид** запроса. После успешного завершения этого запроса можно начать чтение и назначить роль каталога. **Note**: шаблон роли каталога предоставляется для роли каталога Users. Роль каталога Users является неявной и невидимой для клиентов службы каталогов. Все пользователи в клиенте назначают эту роль инфраструктурой. Роль уже активирована. Не используйте этот шаблон.'
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6ec01338159e2b0345437035b2a79cd3f2fb6b4b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340737"
---
# <a name="directoryroletemplate-resource-type"></a><span data-ttu-id="0843a-114">Тип ресурса directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="0843a-114">directoryRoleTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0843a-p102">Представляет шаблон роли каталога. Шаблон роли каталога определяет значения свойств, принадлежащих роли каталога ([directoryRole](directoryrole.md)). С каждой ролью каталога, которую можно активировать на клиенте, связан объект соответствующего шаблона. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируется только роль каталога администраторов организации. Чтобы активировать другие доступные роли каталога, следует отправить запрос POST в конечную точку `/directoryRoles` с идентификатором шаблона роли каталога, на базе которого создана роль каталога и который указан в параметре **roleTemplateId** запроса. После успешного завершения этого запроса можно начинать считывание и назначение членов для роли каталога. **Примечание.** Шаблон роли каталога отображается вместо роли каталога пользователей. Роль каталога пользователей — неявная и невидимая для клиентов каталога. Каждый пользователь на клиенте назначается для этой роли инфраструктурой. Роль уже активирована. Не используйте этот шаблон.</span><span class="sxs-lookup"><span data-stu-id="0843a-p102">Represents a directory role template. A directory role template specifies the property values of a directory role ([directoryRole](directoryrole.md)). There is an associated directory role template object for each of the directory roles that may be activated in a tenant. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles you send a POST request to the `/directoryRoles` endpoint with the ID of the directory role template on which the directory role is based specified in the **roleTemplateId** parameter of the request. Upon successful completion of this request, you can then start to read and assign members to the directory role. **Note**: A directory role template is exposed for the Users directory role. The Users directory role is implicit and is not visible to directory clients. Every User in the tenant is assigned to this role by the infrastructure. The role is already activated. Do not use this template.</span></span>


## <a name="methods"></a><span data-ttu-id="0843a-127">Методы</span><span class="sxs-lookup"><span data-stu-id="0843a-127">Methods</span></span>

| <span data-ttu-id="0843a-128">Метод</span><span class="sxs-lookup"><span data-stu-id="0843a-128">Method</span></span>       | <span data-ttu-id="0843a-129">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0843a-129">Return Type</span></span>  |<span data-ttu-id="0843a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0843a-130">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0843a-131">Получение directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="0843a-131">Get directoryRoleTemplate</span></span>](../api/directoryroletemplate-get.md) | [<span data-ttu-id="0843a-132">directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="0843a-132">directoryRoleTemplate</span></span>](directoryroletemplate.md) |<span data-ttu-id="0843a-133">Считывание свойств и отношений объекта directoryRoleTemplate.</span><span class="sxs-lookup"><span data-stu-id="0843a-133">Read properties and relationships of directoryRoleTemplate object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0843a-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="0843a-134">Properties</span></span>
| <span data-ttu-id="0843a-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="0843a-135">Property</span></span>     | <span data-ttu-id="0843a-136">Тип</span><span class="sxs-lookup"><span data-stu-id="0843a-136">Type</span></span>   |<span data-ttu-id="0843a-137">Описание</span><span class="sxs-lookup"><span data-stu-id="0843a-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0843a-138">description</span><span class="sxs-lookup"><span data-stu-id="0843a-138">description</span></span>|<span data-ttu-id="0843a-139">String</span><span class="sxs-lookup"><span data-stu-id="0843a-139">String</span></span>|<span data-ttu-id="0843a-p103">Описание, которое нужно задать для роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0843a-p103">The description to set for the directory role. Read-only.</span></span>|
|<span data-ttu-id="0843a-142">displayName</span><span class="sxs-lookup"><span data-stu-id="0843a-142">displayName</span></span>|<span data-ttu-id="0843a-143">Строка</span><span class="sxs-lookup"><span data-stu-id="0843a-143">String</span></span>|<span data-ttu-id="0843a-p104">Отображаемое имя, которое нужно назначить роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0843a-p104">The display name to set for the directory role. Read-only.</span></span> |
|<span data-ttu-id="0843a-146">id</span><span class="sxs-lookup"><span data-stu-id="0843a-146">id</span></span>|<span data-ttu-id="0843a-147">Строка</span><span class="sxs-lookup"><span data-stu-id="0843a-147">String</span></span>|<span data-ttu-id="0843a-p105">Уникальный идентификатор шаблона. Наследуется из [directoryObject](directoryobject.md). Следует указать свойство **id** для шаблона роли каталога, чтобы свойство **roleTemplateId** в запросе POST активировало [directoryRole](directoryrole.md) на клиенте. Ключ, значение null не допускается. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0843a-p105">The unique identifier for the template. Inherited from [directoryObject](directoryobject.md). You specify the **id** of the directory role template for the **roleTemplateId** property in the POST request activate a [directoryRole](directoryrole.md) in a tenant. Key, Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0843a-153">Отношения</span><span class="sxs-lookup"><span data-stu-id="0843a-153">Relationships</span></span>
<span data-ttu-id="0843a-154">Нет</span><span class="sxs-lookup"><span data-stu-id="0843a-154">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="0843a-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0843a-155">JSON representation</span></span>

<span data-ttu-id="0843a-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0843a-156">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRoleTemplate"
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
<!--
{
  "type": "#page.annotation",
  "description": "directoryRoleTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
