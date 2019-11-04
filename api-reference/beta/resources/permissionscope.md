---
title: Тип ресурса permissionScope
description: Представляет область делегированного разрешения OAuth 2,0.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 53e777d3a545ed95c5a6010db7abc965d3b9cad5
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939343"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="9dea6-103">Тип ресурса permissionScope</span><span class="sxs-lookup"><span data-stu-id="9dea6-103">permissionScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9dea6-104">Представляет область делегированного разрешения OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="9dea6-104">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="9dea6-105">Указанные делегированные области разрешений OAuth 2,0 могут запрашиваться клиентскими приложениями (через коллекцию **рекуиредресаурцеакцесс** для объекта [Application](application.md) ) при вызове приложения-ресурса.</span><span class="sxs-lookup"><span data-stu-id="9dea6-105">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="9dea6-106">Свойство **oauth2Permissions** объекта [ServicePrincipal](serviceprincipal.md) и сущности [приложения](application.md) является коллекцией **permissionScope**.</span><span class="sxs-lookup"><span data-stu-id="9dea6-106">The **oauth2Permissions** property of the [servicePrincipal](serviceprincipal.md) entity and of the [Application](application.md) entity is a collection of **permissionScope**.</span></span>

## <a name="properties"></a><span data-ttu-id="9dea6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9dea6-107">Properties</span></span>

| <span data-ttu-id="9dea6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9dea6-108">Property</span></span> | <span data-ttu-id="9dea6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9dea6-109">Type</span></span> | <span data-ttu-id="9dea6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9dea6-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9dea6-111">админконсентдескриптион</span><span class="sxs-lookup"><span data-stu-id="9dea6-111">adminConsentDescription</span></span>|<span data-ttu-id="9dea6-112">Строка</span><span class="sxs-lookup"><span data-stu-id="9dea6-112">String</span></span>| <span data-ttu-id="9dea6-113">Текст справки по разрешениям, который отображается в качестве согласия администратора и взаимодействия с назначением приложений.</span><span class="sxs-lookup"><span data-stu-id="9dea6-113">Permission help text that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="9dea6-114">админконсентдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="9dea6-114">adminConsentDisplayName</span></span>|<span data-ttu-id="9dea6-115">Строка</span><span class="sxs-lookup"><span data-stu-id="9dea6-115">String</span></span>| <span data-ttu-id="9dea6-116">Отображаемое имя разрешения, которое отображается в качестве согласия администратора и взаимодействия с назначением приложений.</span><span class="sxs-lookup"><span data-stu-id="9dea6-116">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="9dea6-117">id</span><span class="sxs-lookup"><span data-stu-id="9dea6-117">id</span></span>|<span data-ttu-id="9dea6-118">GUID</span><span class="sxs-lookup"><span data-stu-id="9dea6-118">Guid</span></span>| <span data-ttu-id="9dea6-119">Уникальный идентификатор разрешения области в коллекции oauth2Permissions.</span><span class="sxs-lookup"><span data-stu-id="9dea6-119">Unique scope permission identifier inside the oauth2Permissions collection.</span></span> |
|<span data-ttu-id="9dea6-120">isEnabled</span><span class="sxs-lookup"><span data-stu-id="9dea6-120">isEnabled</span></span>|<span data-ttu-id="9dea6-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dea6-121">Boolean</span></span>| <span data-ttu-id="9dea6-122">При создании или обновлении разрешения для этого свойства должно быть задано **значение true** (значение по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="9dea6-122">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="9dea6-123">Чтобы удалить разрешение, необходимо сначала задать для этого свойства значение **false**.</span><span class="sxs-lookup"><span data-stu-id="9dea6-123">To delete a permission, this property must first be set to **false**.</span></span> <span data-ttu-id="9dea6-124">В этот момент разрешение может быть удалено из последующего вызова.</span><span class="sxs-lookup"><span data-stu-id="9dea6-124">At that point, in a subsequent call, the permission may be removed.</span></span> |
|<span data-ttu-id="9dea6-125">основания</span><span class="sxs-lookup"><span data-stu-id="9dea6-125">origin</span></span>|<span data-ttu-id="9dea6-126">Строка</span><span class="sxs-lookup"><span data-stu-id="9dea6-126">String</span></span>| <span data-ttu-id="9dea6-127">Для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="9dea6-127">For internal use.</span></span> |
|<span data-ttu-id="9dea6-128">type</span><span class="sxs-lookup"><span data-stu-id="9dea6-128">type</span></span>|<span data-ttu-id="9dea6-129">String</span><span class="sxs-lookup"><span data-stu-id="9dea6-129">String</span></span>| <span data-ttu-id="9dea6-130">Указывает, может ли пользователь иметь разрешение на доступ к области, а также о том, является ли оно разрешением, которое должно быть отослано администратором компании.</span><span class="sxs-lookup"><span data-stu-id="9dea6-130">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a company administrator.</span></span> <span data-ttu-id="9dea6-131">Возможные значения: *User* или *Admin*.</span><span class="sxs-lookup"><span data-stu-id="9dea6-131">Possible values are *User* or *Admin*.</span></span> |
|<span data-ttu-id="9dea6-132">усерконсентдескриптион</span><span class="sxs-lookup"><span data-stu-id="9dea6-132">userConsentDescription</span></span>|<span data-ttu-id="9dea6-133">Строка</span><span class="sxs-lookup"><span data-stu-id="9dea6-133">String</span></span>| <span data-ttu-id="9dea6-134">Текст справки по разрешениям, который отображается в диалоговом окне согласия конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="9dea6-134">Permission help text that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="9dea6-135">усерконсентдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="9dea6-135">userConsentDisplayName</span></span>|<span data-ttu-id="9dea6-136">Строка</span><span class="sxs-lookup"><span data-stu-id="9dea6-136">String</span></span>| <span data-ttu-id="9dea6-137">Отображаемое имя разрешения, которое отображается в диалоговом окне согласия конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="9dea6-137">Display name for the permission that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="9dea6-138">value</span><span class="sxs-lookup"><span data-stu-id="9dea6-138">value</span></span>|<span data-ttu-id="9dea6-139">String</span><span class="sxs-lookup"><span data-stu-id="9dea6-139">String</span></span>| <span data-ttu-id="9dea6-140">Значение утверждения области, которое должно ожидать приложение ресурсов в маркере доступа OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="9dea6-140">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9dea6-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9dea6-141">JSON representation</span></span>
<span data-ttu-id="9dea6-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9dea6-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.permissionScope"
}-->

```json
{
  "adminConsentDescription": "String",
  "adminConsentDisplayName": "String",
  "id": "Guid",
  "isEnabled": true,
  "origin": "String",
  "type": "String",
  "userConsentDescription": "String",
  "userConsentDisplayName": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "permissionScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
