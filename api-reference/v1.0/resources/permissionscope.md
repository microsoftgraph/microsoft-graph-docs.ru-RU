---
title: Тип ресурса permissionScope
description: Представляет область делегированного разрешения OAuth 2,0.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: be8d9a7d08334bd716cfcbf565225add790b65e3
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939371"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="d3412-103">Тип ресурса permissionScope</span><span class="sxs-lookup"><span data-stu-id="d3412-103">permissionScope resource type</span></span>

<span data-ttu-id="d3412-104">Представляет область делегированного разрешения OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="d3412-104">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="d3412-105">Указанные делегированные области разрешений OAuth 2,0 могут запрашиваться клиентскими приложениями (через коллекцию **рекуиредресаурцеакцесс** для объекта [Application](application.md) ) при вызове приложения-ресурса.</span><span class="sxs-lookup"><span data-stu-id="d3412-105">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="d3412-106">Свойство **oauth2Permissions**</span><span class="sxs-lookup"><span data-stu-id="d3412-106">The **oauth2Permissions** property</span></span> <!-- of the [servicePrincipal](serviceprincipal.md) entity and --> <span data-ttu-id="d3412-107">объекта [Application](application.md) — коллекция **permissionScope**.</span><span class="sxs-lookup"><span data-stu-id="d3412-107">of the [Application](application.md) entity is a collection of **permissionScope**.</span></span>

## <a name="properties"></a><span data-ttu-id="d3412-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3412-108">Properties</span></span>

| <span data-ttu-id="d3412-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3412-109">Property</span></span> | <span data-ttu-id="d3412-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d3412-110">Type</span></span> | <span data-ttu-id="d3412-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d3412-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d3412-112">админконсентдескриптион</span><span class="sxs-lookup"><span data-stu-id="d3412-112">adminConsentDescription</span></span>|<span data-ttu-id="d3412-113">String</span><span class="sxs-lookup"><span data-stu-id="d3412-113">String</span></span>| <span data-ttu-id="d3412-114">Текст справки по разрешениям, который отображается в качестве согласия администратора и взаимодействия с назначением приложений.</span><span class="sxs-lookup"><span data-stu-id="d3412-114">Permission help text that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="d3412-115">админконсентдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="d3412-115">adminConsentDisplayName</span></span>|<span data-ttu-id="d3412-116">String</span><span class="sxs-lookup"><span data-stu-id="d3412-116">String</span></span>| <span data-ttu-id="d3412-117">Отображаемое имя разрешения, которое отображается в качестве согласия администратора и взаимодействия с назначением приложений.</span><span class="sxs-lookup"><span data-stu-id="d3412-117">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="d3412-118">id</span><span class="sxs-lookup"><span data-stu-id="d3412-118">id</span></span>|<span data-ttu-id="d3412-119">GUID</span><span class="sxs-lookup"><span data-stu-id="d3412-119">Guid</span></span>| <span data-ttu-id="d3412-120">Уникальный идентификатор разрешения области в коллекции oauth2Permissions.</span><span class="sxs-lookup"><span data-stu-id="d3412-120">Unique scope permission identifier inside the oauth2Permissions collection.</span></span> |
|<span data-ttu-id="d3412-121">isEnabled</span><span class="sxs-lookup"><span data-stu-id="d3412-121">isEnabled</span></span>|<span data-ttu-id="d3412-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3412-122">Boolean</span></span>| <span data-ttu-id="d3412-123">При создании или обновлении разрешения для этого свойства должно быть задано **значение true** (значение по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="d3412-123">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="d3412-124">Чтобы удалить разрешение, необходимо сначала задать для этого свойства значение **false**.</span><span class="sxs-lookup"><span data-stu-id="d3412-124">To delete a permission, this property must first be set to **false**.</span></span> <span data-ttu-id="d3412-125">В этот момент разрешение может быть удалено из последующего вызова.</span><span class="sxs-lookup"><span data-stu-id="d3412-125">At that point, in a subsequent call, the permission may be removed.</span></span> |
|<span data-ttu-id="d3412-126">основания</span><span class="sxs-lookup"><span data-stu-id="d3412-126">origin</span></span>|<span data-ttu-id="d3412-127">String</span><span class="sxs-lookup"><span data-stu-id="d3412-127">String</span></span>| <span data-ttu-id="d3412-128">Для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="d3412-128">For internal use.</span></span> |
|<span data-ttu-id="d3412-129">type</span><span class="sxs-lookup"><span data-stu-id="d3412-129">type</span></span>|<span data-ttu-id="d3412-130">String</span><span class="sxs-lookup"><span data-stu-id="d3412-130">String</span></span>| <span data-ttu-id="d3412-131">Указывает, может ли пользователь иметь разрешение на доступ к области, а также о том, является ли оно разрешением, которое должно быть отослано администратором компании.</span><span class="sxs-lookup"><span data-stu-id="d3412-131">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a company administrator.</span></span> <span data-ttu-id="d3412-132">Возможные значения: *User* или *Admin*.</span><span class="sxs-lookup"><span data-stu-id="d3412-132">Possible values are *User* or *Admin*.</span></span> |
|<span data-ttu-id="d3412-133">усерконсентдескриптион</span><span class="sxs-lookup"><span data-stu-id="d3412-133">userConsentDescription</span></span>|<span data-ttu-id="d3412-134">String</span><span class="sxs-lookup"><span data-stu-id="d3412-134">String</span></span>| <span data-ttu-id="d3412-135">Текст справки по разрешениям, который отображается в диалоговом окне согласия конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="d3412-135">Permission help text that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="d3412-136">усерконсентдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="d3412-136">userConsentDisplayName</span></span>|<span data-ttu-id="d3412-137">String</span><span class="sxs-lookup"><span data-stu-id="d3412-137">String</span></span>| <span data-ttu-id="d3412-138">Отображаемое имя разрешения, которое отображается в диалоговом окне согласия конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="d3412-138">Display name for the permission that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="d3412-139">value</span><span class="sxs-lookup"><span data-stu-id="d3412-139">value</span></span>|<span data-ttu-id="d3412-140">String</span><span class="sxs-lookup"><span data-stu-id="d3412-140">String</span></span>| <span data-ttu-id="d3412-141">Значение утверждения области, которое должно ожидать приложение ресурсов в маркере доступа OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="d3412-141">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d3412-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d3412-142">JSON representation</span></span>
<span data-ttu-id="d3412-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3412-143">Here is a JSON representation of the resource.</span></span>

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
