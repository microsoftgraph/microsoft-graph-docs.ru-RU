---
title: Тип ресурса Аппроле
description: Представляет роль приложения, которая может быть запрошена клиентским приложением, вызывающей другое приложение, или которая может использоваться для назначения приложения пользователям или группам в указанной роли приложения. Свойство **appRoles** объекта servicePrincipal и сущности приложения является коллекцией **аппроле**.
localization_priority: Normal
ms.openlocfilehash: 0ff9c2195b8a1abe52ff505c1a01c86244e332c7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328534"
---
# <a name="approle-resource-type"></a><span data-ttu-id="897f4-104">Тип ресурса Аппроле</span><span class="sxs-lookup"><span data-stu-id="897f4-104">appRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="897f4-105">Представляет роль приложения, которая может быть запрошена клиентским приложением, вызывающей другое приложение, или которая может использоваться для назначения приложения пользователям или группам в указанной роли приложения.</span><span class="sxs-lookup"><span data-stu-id="897f4-105">Represents an application role that may be requested by a client application calling another application or that may be used to assign an application to users or groups in a specified application role.</span></span> <span data-ttu-id="897f4-106">Свойство **appRoles** объекта [servicePrincipal](serviceprincipal.md) и сущности [приложения](application.md) является коллекцией **аппроле**.</span><span class="sxs-lookup"><span data-stu-id="897f4-106">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **appRole**.</span></span>

> <span data-ttu-id="897f4-107">Важно! эта функция отключена в текущем выпуске.</span><span class="sxs-lookup"><span data-stu-id="897f4-107">Important: This functionality is disabled in the current release.</span></span>

## <a name="json-representation"></a><span data-ttu-id="897f4-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="897f4-108">JSON representation</span></span>

<span data-ttu-id="897f4-109">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="897f4-109">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="897f4-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="897f4-110">Properties</span></span>
| <span data-ttu-id="897f4-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="897f4-111">Property</span></span>     | <span data-ttu-id="897f4-112">Тип</span><span class="sxs-lookup"><span data-stu-id="897f4-112">Type</span></span>   |<span data-ttu-id="897f4-113">Описание</span><span class="sxs-lookup"><span data-stu-id="897f4-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="897f4-114">Алловедмембертипес</span><span class="sxs-lookup"><span data-stu-id="897f4-114">allowedMemberTypes</span></span>|<span data-ttu-id="897f4-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="897f4-115">String collection</span></span>|<span data-ttu-id="897f4-116">Указывает, можно ли назначить это определение роли приложения пользователям и группам, задав для параметра значение "пользователь" или другие приложения (которые обращаются к этому приложению в сценариях службы демона), задав значение "Application" или как то, и другое.</span><span class="sxs-lookup"><span data-stu-id="897f4-116">Specifies whether this app role definition can be assigned to users and groups by setting to “User”, or to other applications (that are accessing this application in daemon service scenarios) by setting to “Application”, or to both.</span></span>|
|<span data-ttu-id="897f4-117">description</span><span class="sxs-lookup"><span data-stu-id="897f4-117">description</span></span>|<span data-ttu-id="897f4-118">String</span><span class="sxs-lookup"><span data-stu-id="897f4-118">String</span></span>|<span data-ttu-id="897f4-119">Текст справки по разРешениям, который отображается при назначении и согласии приложения администрирования.</span><span class="sxs-lookup"><span data-stu-id="897f4-119">Permission help text that appears in the admin app assignment and consent experiences.</span></span>|
|<span data-ttu-id="897f4-120">displayName</span><span class="sxs-lookup"><span data-stu-id="897f4-120">displayName</span></span>|<span data-ttu-id="897f4-121">String</span><span class="sxs-lookup"><span data-stu-id="897f4-121">String</span></span>|<span data-ttu-id="897f4-122">Отображаемое имя разрешения, которое отображается в качестве согласия администратора и взаимодействия с назначением приложений.</span><span class="sxs-lookup"><span data-stu-id="897f4-122">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="897f4-123">id</span><span class="sxs-lookup"><span data-stu-id="897f4-123">id</span></span>|<span data-ttu-id="897f4-124">GUID</span><span class="sxs-lookup"><span data-stu-id="897f4-124">Guid</span></span>|<span data-ttu-id="897f4-125">Уникальный идентификатор роли в семействе **appRoles** .</span><span class="sxs-lookup"><span data-stu-id="897f4-125">Unique role identifier inside the **appRoles** collection.</span></span>|
|<span data-ttu-id="897f4-126">isEnabled</span><span class="sxs-lookup"><span data-stu-id="897f4-126">isEnabled</span></span>|<span data-ttu-id="897f4-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="897f4-127">Boolean</span></span>|<span data-ttu-id="897f4-128">При создании или обновлении определения роли должно быть задано **значение true** (значение по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="897f4-128">When creating or updating a role definition, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="897f4-129">Чтобы удалить роль, необходимо сначала задать значение **false**.</span><span class="sxs-lookup"><span data-stu-id="897f4-129">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="897f4-130">В этот момент эта роль может быть удалена в последующих вызовах.</span><span class="sxs-lookup"><span data-stu-id="897f4-130">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="897f4-131">value</span><span class="sxs-lookup"><span data-stu-id="897f4-131">value</span></span>|<span data-ttu-id="897f4-132">String</span><span class="sxs-lookup"><span data-stu-id="897f4-132">String</span></span>|<span data-ttu-id="897f4-133">Указывает значение утверждения ролей, которое должно ожидать приложение в маркерах проверки подлинности и доступа.</span><span class="sxs-lookup"><span data-stu-id="897f4-133">Specifies the value of the roles claim that the application should expect in the authentication and access tokens.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
