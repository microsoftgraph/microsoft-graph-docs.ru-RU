---
title: Тип ресурса directoryRoleTemplate
description: Представляет шаблон роли каталога. Шаблон роли каталога определяет значения свойств, принадлежащих роли каталога (directoryRole). С каждой ролью каталога, которую можно активировать на клиенте, связан объект соответствующего шаблона. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируется только роль каталога администраторов организации. Чтобы активировать другие доступные роли каталога, следует отправить запрос POST в конечную точку  с идентификатором шаблона роли каталога, на базе которого создана роль каталога и который указан в параметре roleTemplateId запроса. После успешного завершения этого запроса можно начинать считывание и назначение членов для роли каталога. Примечание. Шаблон роли каталога отображается вместо роли каталога пользователей. Роль каталога пользователей — неявная и невидимая для клиентов каталога. Каждый пользователь на клиенте назначается для этой роли инфраструктурой. Роль уже активирована. Не используйте этот шаблон.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dd813c9f7676e7190e5aedbb6d9b950e9ffc6aac
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526160"
---
# <a name="directoryroletemplate-resource-type"></a><span data-ttu-id="4264c-114">Тип ресурса directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="4264c-114">directoryRoleTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4264c-p102">Представляет шаблон роли каталога. Шаблон роли каталога определяет значения свойств, принадлежащих роли каталога ([directoryRole](directoryrole.md)). С каждой ролью каталога, которую можно активировать на клиенте, связан объект соответствующего шаблона. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируется только роль каталога администраторов организации. Чтобы активировать другие доступные роли каталога, следует отправить запрос POST в конечную точку `/directoryRoles` с идентификатором шаблона роли каталога, на базе которого создана роль каталога и который указан в параметре **roleTemplateId** запроса. После успешного завершения этого запроса можно начинать считывание и назначение членов для роли каталога. **Примечание.** Шаблон роли каталога отображается вместо роли каталога пользователей. Роль каталога пользователей — неявная и невидимая для клиентов каталога. Каждый пользователь на клиенте назначается для этой роли инфраструктурой. Роль уже активирована. Не используйте этот шаблон.</span><span class="sxs-lookup"><span data-stu-id="4264c-p102">Represents a directory role template. A directory role template specifies the property values of a directory role ([directoryRole](directoryrole.md)). There is an associated directory role template object for each of the directory roles that may be activated in a tenant. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles you send a POST request to the `/directoryRoles` endpoint with the ID of the directory role template on which the directory role is based specified in the **roleTemplateId** parameter of the request. Upon successful completion of this request, you can then start to read and assign members to the directory role. **Note**: A directory role template is exposed for the Users directory role. The Users directory role is implicit and is not visible to directory clients. Every User in the tenant is assigned to this role by the infrastructure. The role is already activated. Do not use this template.</span></span>


## <a name="methods"></a><span data-ttu-id="4264c-127">Методы</span><span class="sxs-lookup"><span data-stu-id="4264c-127">Methods</span></span>

| <span data-ttu-id="4264c-128">Метод</span><span class="sxs-lookup"><span data-stu-id="4264c-128">Method</span></span>       | <span data-ttu-id="4264c-129">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4264c-129">Return Type</span></span>  |<span data-ttu-id="4264c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="4264c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4264c-131">Получение directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="4264c-131">[Get directoryRoleTemplate](../api/directoryroletemplate-get.md)</span></span> | [<span data-ttu-id="4264c-132">directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="4264c-132">directoryRoleTemplate</span></span>](directoryroletemplate.md) |<span data-ttu-id="4264c-133">Считывание свойств и отношений объекта directoryRoleTemplate.</span><span class="sxs-lookup"><span data-stu-id="4264c-133">Read properties and relationships of directoryRoleTemplate object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4264c-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="4264c-134">Properties</span></span>
| <span data-ttu-id="4264c-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="4264c-135">Property</span></span>     | <span data-ttu-id="4264c-136">Тип</span><span class="sxs-lookup"><span data-stu-id="4264c-136">Type</span></span>   |<span data-ttu-id="4264c-137">Описание</span><span class="sxs-lookup"><span data-stu-id="4264c-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4264c-138">description</span><span class="sxs-lookup"><span data-stu-id="4264c-138">description</span></span>|<span data-ttu-id="4264c-139">String</span><span class="sxs-lookup"><span data-stu-id="4264c-139">String</span></span>|<span data-ttu-id="4264c-p103">Описание, которое нужно задать для роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4264c-p103">The description to set for the directory role. Read-only.</span></span>|
|<span data-ttu-id="4264c-142">displayName</span><span class="sxs-lookup"><span data-stu-id="4264c-142">displayName</span></span>|<span data-ttu-id="4264c-143">String</span><span class="sxs-lookup"><span data-stu-id="4264c-143">String</span></span>|<span data-ttu-id="4264c-p104">Отображаемое имя, которое нужно назначить роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4264c-p104">The display name to set for the directory role. Read-only.</span></span> |
|<span data-ttu-id="4264c-146">id</span><span class="sxs-lookup"><span data-stu-id="4264c-146">id</span></span>|<span data-ttu-id="4264c-147">String</span><span class="sxs-lookup"><span data-stu-id="4264c-147">String</span></span>|<span data-ttu-id="4264c-p105">Уникальный идентификатор шаблона. Наследуется из [directoryObject](directoryobject.md). Следует указать свойство **id** для шаблона роли каталога, чтобы свойство **roleTemplateId** в запросе POST активировало [directoryRole](directoryrole.md) на клиенте. Ключ, значение null не допускается. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4264c-p105">The unique identifier for the template. Inherited from [directoryObject](directoryobject.md). You specify the **id** of the directory role template for the **roleTemplateId** property in the POST request activate a [directoryRole](directoryrole.md) in a tenant. Key, Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4264c-153">Отношения</span><span class="sxs-lookup"><span data-stu-id="4264c-153">Relationships</span></span>
<span data-ttu-id="4264c-154">Нет</span><span class="sxs-lookup"><span data-stu-id="4264c-154">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="4264c-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4264c-155">JSON representation</span></span>

<span data-ttu-id="4264c-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4264c-156">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryroletemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
