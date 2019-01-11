---
title: Тип ресурса directoryRoleTemplate
description: 'Представляет шаблон роли каталога. Шаблон роли каталога задает значения свойств роли каталога (directoryRole). Нет объекта связанного directory роли шаблона для каждой роли каталогов, которые может быть активировано клиента. Для чтения роли каталога или обновите его члены, необходимо активировать в клиентов. Только роль directory Администраторы организации активируется по умолчанию. Активация других ролей доступны directory отправить запрос POST для `/directoryRoles` конечная точка с Идентификатором роль шаблона каталога — это каталог роль на основе указанного в параметре **roleTemplateId** запроса. После успешного выполнения этого запроса то затем сможете для чтения и добавления членов в роль directory. **Примечание**: шаблона роли каталога, открытой для роли каталогов пользователей. Роль каталогов пользователей неявных и не отображается на клиентах каталогов. Каждый пользователь клиента назначена эта роль в инфраструктуре. Роль уже активировано. Не используйте этот шаблон.'
localization_priority: Normal
ms.openlocfilehash: bffff81db3416c538031bce58cfc80580c06f48e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821191"
---
# <a name="directoryroletemplate-resource-type"></a><span data-ttu-id="85afa-114">Тип ресурса directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="85afa-114">directoryRoleTemplate resource type</span></span>

> <span data-ttu-id="85afa-115">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="85afa-115">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85afa-116">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85afa-116">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="85afa-p103">Представляет шаблон роли каталога. Шаблон роли каталога определяет значения свойств, принадлежащих роли каталога ([directoryRole](directoryrole.md)). С каждой ролью каталога, которую можно активировать на клиенте, связан объект соответствующего шаблона. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируется только роль каталога администраторов организации. Чтобы активировать другие доступные роли каталога, следует отправить запрос POST в конечную точку `/directoryRoles` с идентификатором шаблона роли каталога, на базе которого создана роль каталога и который указан в параметре **roleTemplateId** запроса. После успешного завершения этого запроса можно начинать считывание и назначение членов для роли каталога. **Примечание.** Шаблон роли каталога отображается вместо роли каталога пользователей. Роль каталога пользователей — неявная и невидимая для клиентов каталога. Каждый пользователь на клиенте назначается для этой роли инфраструктурой. Роль уже активирована. Не используйте этот шаблон.</span><span class="sxs-lookup"><span data-stu-id="85afa-p103">Represents a directory role template. A directory role template specifies the property values of a directory role ([directoryRole](directoryrole.md)). There is an associated directory role template object for each of the directory roles that may be activated in a tenant. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles you send a POST request to the `/directoryRoles` endpoint with the ID of the directory role template on which the directory role is based specified in the **roleTemplateId** parameter of the request. Upon successful completion of this request, you can then start to read and assign members to the directory role. **Note**: A directory role template is exposed for the Users directory role. The Users directory role is implicit and is not visible to directory clients. Every User in the tenant is assigned to this role by the infrastructure. The role is already activated. Do not use this template.</span></span>


## <a name="methods"></a><span data-ttu-id="85afa-129">Методы</span><span class="sxs-lookup"><span data-stu-id="85afa-129">Methods</span></span>

| <span data-ttu-id="85afa-130">Метод</span><span class="sxs-lookup"><span data-stu-id="85afa-130">Method</span></span>       | <span data-ttu-id="85afa-131">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="85afa-131">Return Type</span></span>  |<span data-ttu-id="85afa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="85afa-132">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="85afa-133">Получение directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="85afa-133">Get directoryRoleTemplate</span></span>](../api/directoryroletemplate-get.md) | [<span data-ttu-id="85afa-134">directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="85afa-134">directoryRoleTemplate</span></span>](directoryroletemplate.md) |<span data-ttu-id="85afa-135">Считывание свойств и отношений объекта directoryRoleTemplate.</span><span class="sxs-lookup"><span data-stu-id="85afa-135">Read properties and relationships of directoryRoleTemplate object.</span></span>|

## <a name="properties"></a><span data-ttu-id="85afa-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="85afa-136">Properties</span></span>
| <span data-ttu-id="85afa-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="85afa-137">Property</span></span>     | <span data-ttu-id="85afa-138">Тип</span><span class="sxs-lookup"><span data-stu-id="85afa-138">Type</span></span>   |<span data-ttu-id="85afa-139">Описание</span><span class="sxs-lookup"><span data-stu-id="85afa-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85afa-140">описание</span><span class="sxs-lookup"><span data-stu-id="85afa-140">description</span></span>|<span data-ttu-id="85afa-141">String</span><span class="sxs-lookup"><span data-stu-id="85afa-141">String</span></span>|<span data-ttu-id="85afa-p104">Описание, которое нужно задать для роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="85afa-p104">The description to set for the directory role. Read-only.</span></span>|
|<span data-ttu-id="85afa-144">displayName</span><span class="sxs-lookup"><span data-stu-id="85afa-144">displayName</span></span>|<span data-ttu-id="85afa-145">Строка</span><span class="sxs-lookup"><span data-stu-id="85afa-145">String</span></span>|<span data-ttu-id="85afa-p105">Отображаемое имя, которое нужно назначить роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="85afa-p105">The display name to set for the directory role. Read-only.</span></span> |
|<span data-ttu-id="85afa-148">id</span><span class="sxs-lookup"><span data-stu-id="85afa-148">id</span></span>|<span data-ttu-id="85afa-149">Строка</span><span class="sxs-lookup"><span data-stu-id="85afa-149">String</span></span>|<span data-ttu-id="85afa-p106">Уникальный идентификатор шаблона. Наследуется из [directoryObject](directoryobject.md). Следует указать свойство **id** для шаблона роли каталога, чтобы свойство **roleTemplateId** в запросе POST активировало [directoryRole](directoryrole.md) на клиенте. Ключ, значение null не допускается. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="85afa-p106">The unique identifier for the template. Inherited from [directoryObject](directoryobject.md). You specify the **id** of the directory role template for the **roleTemplateId** property in the POST request activate a [directoryRole](directoryrole.md) in a tenant. Key, Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85afa-155">Связи</span><span class="sxs-lookup"><span data-stu-id="85afa-155">Relationships</span></span>
<span data-ttu-id="85afa-156">Нет</span><span class="sxs-lookup"><span data-stu-id="85afa-156">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="85afa-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="85afa-157">JSON representation</span></span>

<span data-ttu-id="85afa-158">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85afa-158">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "directoryRoleTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
