---
title: Тип ресурса роли приложения
description: Представляет роль приложения, которое может быть затребованы клиентское приложение вызов другого приложения или, который может использоваться для назначения приложения для пользователей или групп в указанном приложении роли. Свойство **appRoles** servicePrincipal сущности и сущности приложения — это коллекция **роли приложения**.
localization_priority: Normal
ms.openlocfilehash: 26fe11fc4f0c362de002c205c7e3b95a6ec4a314
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891548"
---
# <a name="approle-resource-type"></a><span data-ttu-id="57374-104">Тип ресурса роли приложения</span><span class="sxs-lookup"><span data-stu-id="57374-104">appRole resource type</span></span>

> <span data-ttu-id="57374-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="57374-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57374-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57374-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="57374-107">Представляет роль приложения, которое может быть затребованы клиентское приложение вызов другого приложения или, который может использоваться для назначения приложения для пользователей или групп в указанном приложении роли.</span><span class="sxs-lookup"><span data-stu-id="57374-107">Represents an application role that may be requested by a client application calling another application or that may be used to assign an application to users or groups in a specified application role.</span></span> <span data-ttu-id="57374-108">Свойство **appRoles** [servicePrincipal](serviceprincipal.md) сущности и сущности [приложения](application.md) — это коллекция **роли приложения**.</span><span class="sxs-lookup"><span data-stu-id="57374-108">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **appRole**.</span></span>

> <span data-ttu-id="57374-109">Важно: Эта функция отключена в текущем выпуске.</span><span class="sxs-lookup"><span data-stu-id="57374-109">Important: This functionality is disabled in the current release.</span></span>

## <a name="json-representation"></a><span data-ttu-id="57374-110">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="57374-110">JSON representation</span></span>

<span data-ttu-id="57374-111">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="57374-111">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approle"
}-->

```json
{
  "allowedMemberTypes": ["string"],
  "description": "string",
  "displayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "value": "string"
}

```
## <a name="properties"></a><span data-ttu-id="57374-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="57374-112">Properties</span></span>
| <span data-ttu-id="57374-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="57374-113">Property</span></span>     | <span data-ttu-id="57374-114">Тип</span><span class="sxs-lookup"><span data-stu-id="57374-114">Type</span></span>   |<span data-ttu-id="57374-115">Описание</span><span class="sxs-lookup"><span data-stu-id="57374-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57374-116">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="57374-116">allowedMemberTypes</span></span>|<span data-ttu-id="57374-117">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="57374-117">String collection</span></span>|<span data-ttu-id="57374-118">Указывает ли определение роли в этом приложении можно назначить пользователям и группам, настройку «User» или другие приложения (которые обращаются к этого приложения в сценариях службы демон), задав для «Приложения» или оба.</span><span class="sxs-lookup"><span data-stu-id="57374-118">Specifies whether this app role definition can be assigned to users and groups by setting to “User”, or to other applications (that are accessing this application in daemon service scenarios) by setting to “Application”, or to both.</span></span>|
|<span data-ttu-id="57374-119">описание</span><span class="sxs-lookup"><span data-stu-id="57374-119">description</span></span>|<span data-ttu-id="57374-120">Строка</span><span class="sxs-lookup"><span data-stu-id="57374-120">String</span></span>|<span data-ttu-id="57374-121">Разрешение текст, который отображается в назначении приложения администрирования справки и соглашаетесь каждый раз.</span><span class="sxs-lookup"><span data-stu-id="57374-121">Permission help text that appears in the admin app assignment and consent experiences.</span></span>|
|<span data-ttu-id="57374-122">displayName</span><span class="sxs-lookup"><span data-stu-id="57374-122">displayName</span></span>|<span data-ttu-id="57374-123">Строка</span><span class="sxs-lookup"><span data-stu-id="57374-123">String</span></span>|<span data-ttu-id="57374-124">Отображаемое имя для разрешения, которое отображается в admin согласия и приложение назначения приемы и способы работы.</span><span class="sxs-lookup"><span data-stu-id="57374-124">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="57374-125">id</span><span class="sxs-lookup"><span data-stu-id="57374-125">id</span></span>|<span data-ttu-id="57374-126">Guid</span><span class="sxs-lookup"><span data-stu-id="57374-126">Guid</span></span>|<span data-ttu-id="57374-127">Уникальный идентификатор роли в коллекцию **appRoles** .</span><span class="sxs-lookup"><span data-stu-id="57374-127">Unique role identifier inside the **appRoles** collection.</span></span>|
|<span data-ttu-id="57374-128">isEnabled</span><span class="sxs-lookup"><span data-stu-id="57374-128">isEnabled</span></span>|<span data-ttu-id="57374-129">Логический</span><span class="sxs-lookup"><span data-stu-id="57374-129">Boolean</span></span>|<span data-ttu-id="57374-130">При создании или обновлении определения роли, это должно быть присвоено **значение true** (по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="57374-130">When creating or updating a role definition, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="57374-131">Чтобы удалить роль, это необходимо сначала задать значение **false**.</span><span class="sxs-lookup"><span data-stu-id="57374-131">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="57374-132">На этом этапе в последующих вызовов, с этой ролью может быть удален.</span><span class="sxs-lookup"><span data-stu-id="57374-132">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="57374-133">value</span><span class="sxs-lookup"><span data-stu-id="57374-133">value</span></span>|<span data-ttu-id="57374-134">Строка</span><span class="sxs-lookup"><span data-stu-id="57374-134">String</span></span>|<span data-ttu-id="57374-135">Задает значение утверждения роли, приложение должно привести в маркеры проверки подлинности и доступа.</span><span class="sxs-lookup"><span data-stu-id="57374-135">Specifies the value of the roles claim that the application should expect in the authentication and access tokens.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
