---
title: Тип ресурса роли приложения
description: Представляет роль приложения, которое может быть затребованы клиентское приложение вызов другого приложения или, который может использоваться для назначения приложения для пользователей или групп в указанном приложении роли. Свойство **appRoles** servicePrincipal сущности и сущности приложения — это коллекция **роли приложения**.
localization_priority: Normal
ms.openlocfilehash: 6f587c15073cf2ad5f6b9973de8f7ef66c294294
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571256"
---
# <a name="approle-resource-type"></a><span data-ttu-id="4bb93-104">Тип ресурса роли приложения</span><span class="sxs-lookup"><span data-stu-id="4bb93-104">appRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bb93-105">Представляет роль приложения, которое может быть затребованы клиентское приложение вызов другого приложения или, который может использоваться для назначения приложения для пользователей или групп в указанном приложении роли.</span><span class="sxs-lookup"><span data-stu-id="4bb93-105">Represents an application role that may be requested by a client application calling another application or that may be used to assign an application to users or groups in a specified application role.</span></span> <span data-ttu-id="4bb93-106">Свойство **appRoles** [servicePrincipal](serviceprincipal.md) сущности и сущности [приложения](application.md) — это коллекция **роли приложения**.</span><span class="sxs-lookup"><span data-stu-id="4bb93-106">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **appRole**.</span></span>

> <span data-ttu-id="4bb93-107">Важно: Эта функция отключена в текущем выпуске.</span><span class="sxs-lookup"><span data-stu-id="4bb93-107">Important: This functionality is disabled in the current release.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4bb93-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4bb93-108">JSON representation</span></span>

<span data-ttu-id="4bb93-109">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="4bb93-109">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appRole"
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
## <a name="properties"></a><span data-ttu-id="4bb93-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="4bb93-110">Properties</span></span>
| <span data-ttu-id="4bb93-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="4bb93-111">Property</span></span>     | <span data-ttu-id="4bb93-112">Тип</span><span class="sxs-lookup"><span data-stu-id="4bb93-112">Type</span></span>   |<span data-ttu-id="4bb93-113">Описание</span><span class="sxs-lookup"><span data-stu-id="4bb93-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4bb93-114">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="4bb93-114">allowedMemberTypes</span></span>|<span data-ttu-id="4bb93-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4bb93-115">String collection</span></span>|<span data-ttu-id="4bb93-116">Указывает ли определение роли в этом приложении можно назначить пользователям и группам, настройку «User» или другие приложения (которые обращаются к этого приложения в сценариях службы демон), задав для «Приложения» или оба.</span><span class="sxs-lookup"><span data-stu-id="4bb93-116">Specifies whether this app role definition can be assigned to users and groups by setting to “User”, or to other applications (that are accessing this application in daemon service scenarios) by setting to “Application”, or to both.</span></span>|
|<span data-ttu-id="4bb93-117">description</span><span class="sxs-lookup"><span data-stu-id="4bb93-117">description</span></span>|<span data-ttu-id="4bb93-118">Строка</span><span class="sxs-lookup"><span data-stu-id="4bb93-118">String</span></span>|<span data-ttu-id="4bb93-119">Разрешение текст, который отображается в назначении приложения администрирования справки и соглашаетесь каждый раз.</span><span class="sxs-lookup"><span data-stu-id="4bb93-119">Permission help text that appears in the admin app assignment and consent experiences.</span></span>|
|<span data-ttu-id="4bb93-120">displayName</span><span class="sxs-lookup"><span data-stu-id="4bb93-120">displayName</span></span>|<span data-ttu-id="4bb93-121">Строка</span><span class="sxs-lookup"><span data-stu-id="4bb93-121">String</span></span>|<span data-ttu-id="4bb93-122">Отображаемое имя для разрешения, которое отображается в admin согласия и приложение назначения приемы и способы работы.</span><span class="sxs-lookup"><span data-stu-id="4bb93-122">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="4bb93-123">id</span><span class="sxs-lookup"><span data-stu-id="4bb93-123">id</span></span>|<span data-ttu-id="4bb93-124">Guid</span><span class="sxs-lookup"><span data-stu-id="4bb93-124">Guid</span></span>|<span data-ttu-id="4bb93-125">Уникальный идентификатор роли в коллекцию **appRoles** .</span><span class="sxs-lookup"><span data-stu-id="4bb93-125">Unique role identifier inside the **appRoles** collection.</span></span>|
|<span data-ttu-id="4bb93-126">isEnabled</span><span class="sxs-lookup"><span data-stu-id="4bb93-126">isEnabled</span></span>|<span data-ttu-id="4bb93-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="4bb93-127">Boolean</span></span>|<span data-ttu-id="4bb93-128">При создании или обновлении определения роли, это должно быть присвоено **значение true** (по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="4bb93-128">When creating or updating a role definition, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="4bb93-129">Чтобы удалить роль, это необходимо сначала задать значение **false**.</span><span class="sxs-lookup"><span data-stu-id="4bb93-129">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="4bb93-130">На этом этапе в последующих вызовов, с этой ролью может быть удален.</span><span class="sxs-lookup"><span data-stu-id="4bb93-130">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="4bb93-131">value</span><span class="sxs-lookup"><span data-stu-id="4bb93-131">value</span></span>|<span data-ttu-id="4bb93-132">Строка</span><span class="sxs-lookup"><span data-stu-id="4bb93-132">String</span></span>|<span data-ttu-id="4bb93-133">Задает значение утверждения роли, приложение должно привести в маркеры проверки подлинности и доступа.</span><span class="sxs-lookup"><span data-stu-id="4bb93-133">Specifies the value of the roles claim that the application should expect in the authentication and access tokens.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/approle.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
