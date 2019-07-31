---
title: Тип ресурса oAuth2Permission
description: Представляет область делегированного разрешения OAuth 2,0. Указанные делегированные области разрешений OAuth 2,0 могут запрашиваться клиентскими приложениями (через коллекцию **рекуиредресаурцеакцесс** для объекта Application) при вызове приложения-ресурса. Свойство **appRoles** объекта servicePrincipal и сущности приложения является коллекцией **oAuth2Permission**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 16dfa93d13127d585cd5b56a56987bb22ab39d8f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009575"
---
# <a name="oauth2permission-resource-type"></a><span data-ttu-id="4604c-105">Тип ресурса oAuth2Permission</span><span class="sxs-lookup"><span data-stu-id="4604c-105">oAuth2Permission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4604c-106">Представляет область делегированного разрешения OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="4604c-106">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="4604c-107">Указанные делегированные области разрешений OAuth 2,0 могут запрашиваться клиентскими приложениями (через коллекцию **рекуиредресаурцеакцесс** для объекта [Application](application.md) ) при вызове приложения-ресурса.</span><span class="sxs-lookup"><span data-stu-id="4604c-107">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="4604c-108">Свойство **appRoles** объекта [servicePrincipal](serviceprincipal.md) и сущности [приложения](application.md) является коллекцией **oAuth2Permission**.</span><span class="sxs-lookup"><span data-stu-id="4604c-108">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **oAuth2Permission**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="4604c-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4604c-109">JSON representation</span></span>

<span data-ttu-id="4604c-110">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="4604c-110">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2Permission"
}-->

```json
{
  "adminConsentDescription": "string",
  "adminConsentDisplayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "type": "string",
  "userConsentDescription": "string",
  "userConsentDisplayName": "string",
  "value": "string"
}

```
## <a name="properties"></a><span data-ttu-id="4604c-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="4604c-111">Properties</span></span>
| <span data-ttu-id="4604c-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="4604c-112">Property</span></span>     | <span data-ttu-id="4604c-113">Тип</span><span class="sxs-lookup"><span data-stu-id="4604c-113">Type</span></span>   |<span data-ttu-id="4604c-114">Описание</span><span class="sxs-lookup"><span data-stu-id="4604c-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4604c-115">Админконсентдескриптион</span><span class="sxs-lookup"><span data-stu-id="4604c-115">adminConsentDescription</span></span>|<span data-ttu-id="4604c-116">String</span><span class="sxs-lookup"><span data-stu-id="4604c-116">String</span></span>|<span data-ttu-id="4604c-117">Текст справки по разрешениям, который отображается в качестве согласия администратора и взаимодействия с назначением приложений.</span><span class="sxs-lookup"><span data-stu-id="4604c-117">Permission help text that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="4604c-118">Админконсентдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="4604c-118">adminConsentDisplayName</span></span>|<span data-ttu-id="4604c-119">String</span><span class="sxs-lookup"><span data-stu-id="4604c-119">String</span></span>|<span data-ttu-id="4604c-120">Отображаемое имя разрешения, которое отображается в качестве согласия администратора и взаимодействия с назначением приложений.</span><span class="sxs-lookup"><span data-stu-id="4604c-120">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="4604c-121">id</span><span class="sxs-lookup"><span data-stu-id="4604c-121">id</span></span>|<span data-ttu-id="4604c-122">GUID</span><span class="sxs-lookup"><span data-stu-id="4604c-122">Guid</span></span>|<span data-ttu-id="4604c-123">Уникальный идентификатор разрешения области в коллекции oauth2Permissions.</span><span class="sxs-lookup"><span data-stu-id="4604c-123">Unique scope permission identifier inside the oauth2Permissions collection.</span></span>|
|<span data-ttu-id="4604c-124">isEnabled</span><span class="sxs-lookup"><span data-stu-id="4604c-124">isEnabled</span></span>|<span data-ttu-id="4604c-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="4604c-125">Boolean</span></span>|<span data-ttu-id="4604c-126">При создании или обновлении разрешения для этого свойства должно быть задано **значение true** (значение по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="4604c-126">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="4604c-127">Чтобы удалить разрешение, необходимо сначала задать для этого свойства значение **false**.</span><span class="sxs-lookup"><span data-stu-id="4604c-127">To delete a permission, this property must first be set to **false**.</span></span>  <span data-ttu-id="4604c-128">В этот момент разрешение может быть удалено из последующего вызова.</span><span class="sxs-lookup"><span data-stu-id="4604c-128">At that point, in a subsequent call, the permission may be removed.</span></span>|
|<span data-ttu-id="4604c-129">type</span><span class="sxs-lookup"><span data-stu-id="4604c-129">type</span></span>|<span data-ttu-id="4604c-130">String</span><span class="sxs-lookup"><span data-stu-id="4604c-130">String</span></span>|<span data-ttu-id="4604c-131">Указывает, может ли пользователь иметь разрешение на доступ к области, а также о том, является ли оно разрешением, которое должно быть отослано администратором компании.</span><span class="sxs-lookup"><span data-stu-id="4604c-131">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a Company Administrator.</span></span>  <span data-ttu-id="4604c-132">Возможные значения: "User" или "admin".</span><span class="sxs-lookup"><span data-stu-id="4604c-132">Possible values are "User" or "Admin".</span></span>|
|<span data-ttu-id="4604c-133">Усерконсентдескриптион</span><span class="sxs-lookup"><span data-stu-id="4604c-133">userConsentDescription</span></span>|<span data-ttu-id="4604c-134">String</span><span class="sxs-lookup"><span data-stu-id="4604c-134">String</span></span>|<span data-ttu-id="4604c-135">Текст справки по разрешениям, который отображается в диалоговом окне согласия конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="4604c-135">Permission help text that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="4604c-136">Усерконсентдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="4604c-136">userConsentDisplayName</span></span>|<span data-ttu-id="4604c-137">String</span><span class="sxs-lookup"><span data-stu-id="4604c-137">String</span></span>|<span data-ttu-id="4604c-138">Отображаемое имя разрешения, которое отображается в диалоговом окне согласия конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="4604c-138">Display name for the permission that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="4604c-139">value</span><span class="sxs-lookup"><span data-stu-id="4604c-139">value</span></span>|<span data-ttu-id="4604c-140">String</span><span class="sxs-lookup"><span data-stu-id="4604c-140">String</span></span>|<span data-ttu-id="4604c-141">Значение утверждения области, которое должно ожидать приложение ресурсов в маркере доступа OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="4604c-141">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
