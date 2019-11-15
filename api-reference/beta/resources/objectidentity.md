---
title: Тип ресурса Обжектидентити
description: Представляет идентификатор, используемый для входа в учетную запись пользователя.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: c29d7ca1b2b4f20f53ed4be45807eb666002163c
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "38658802"
---
# <a name="objectidentity-resource-type"></a><span data-ttu-id="067e0-103">Тип ресурса Обжектидентити</span><span class="sxs-lookup"><span data-stu-id="067e0-103">objectIdentity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="067e0-104">Представляет идентификатор, используемый для входа в учетную запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="067e0-104">Represents an identity used to sign in to a user account.</span></span> <span data-ttu-id="067e0-105">Удостоверение может предоставляться корпорацией Майкрософт, организациями или поставщиками социальных удостоверений, такими как Facebook, Google или Майкрософт, которые связаны с учетной записью пользователя.</span><span class="sxs-lookup"><span data-stu-id="067e0-105">An identity can be provided by Microsoft, by organizations, or by social identity providers such as Facebook, Google, or Microsoft, that are tied to a user account.</span></span> <span data-ttu-id="067e0-106">Это позволяет пользователю выполнить вход в учетную запись пользователя с любыми связанными удостоверениями.</span><span class="sxs-lookup"><span data-stu-id="067e0-106">This enables the user to sign in to the user account with any of those associated identities.</span></span>

<span data-ttu-id="067e0-107">Свойство **удостоверения** для ресурса [User](user.md) является объектом **обжектидентити** .</span><span class="sxs-lookup"><span data-stu-id="067e0-107">The **identities** property of the [user](user.md) resource is an **objectIdentity** object.</span></span>

## <a name="properties"></a><span data-ttu-id="067e0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="067e0-108">Properties</span></span>

| <span data-ttu-id="067e0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="067e0-109">Property</span></span>   | <span data-ttu-id="067e0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="067e0-110">Type</span></span> |<span data-ttu-id="067e0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="067e0-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="067e0-112">сигнинтипе</span><span class="sxs-lookup"><span data-stu-id="067e0-112">signInType</span></span>|<span data-ttu-id="067e0-113">string</span><span class="sxs-lookup"><span data-stu-id="067e0-113">string</span></span>| <span data-ttu-id="067e0-114">Задает типы входа пользователя в каталоге, например `emailAddress`, `userName` или. `federated`</span><span class="sxs-lookup"><span data-stu-id="067e0-114">Specifies the user sign-in types in your directory, such as `emailAddress`, `userName` or `federated`.</span></span> <span data-ttu-id="067e0-115">Здесь `federated` представляет уникальный идентификатор пользователя у поставщика, который может быть в любом формате, выбранном поставщиком.</span><span class="sxs-lookup"><span data-stu-id="067e0-115">Here, `federated` represents a unique identifier for a user from an issuer, that can be in any format chosen by the issuer.</span></span> <span data-ttu-id="067e0-116">Дополнительная проверка применяется к **иссуерассигнедид** , если для `emailAddress` параметра Тип входа задано значение или. `userName`</span><span class="sxs-lookup"><span data-stu-id="067e0-116">Additional validation is enforced on **issuerAssignedId** when the sign-in type is set to `emailAddress` or `userName`.</span></span> <span data-ttu-id="067e0-117">Этому свойству также можно присвоить любую настраиваемую строку.</span><span class="sxs-lookup"><span data-stu-id="067e0-117">This property can also be set to any custom string.</span></span>|
|<span data-ttu-id="067e0-118">имени</span><span class="sxs-lookup"><span data-stu-id="067e0-118">issuer</span></span>|<span data-ttu-id="067e0-119">string</span><span class="sxs-lookup"><span data-stu-id="067e0-119">string</span></span>|<span data-ttu-id="067e0-120">Указывает издателя удостоверения, например `facebook.com`.</span><span class="sxs-lookup"><span data-stu-id="067e0-120">Specifies the issuer of the identity, for example `facebook.com`.</span></span><br><span data-ttu-id="067e0-121">Для локальных учетных записей \*\*\*\* (где сигнинтипе `federated`— нет) это свойство является локальным именем домена по умолчанию для клиента `contoso.onmicrosoft.com`B2C, например.</span><span class="sxs-lookup"><span data-stu-id="067e0-121">For local accounts (where **signInType** is not `federated`), this property is the local B2C tenant default domain name, for example `contoso.onmicrosoft.com`.</span></span><br><span data-ttu-id="067e0-122">Для внешних пользователей из другой организации Azure AD это будет домен федеративной организации, например `contoso.com`.</span><span class="sxs-lookup"><span data-stu-id="067e0-122">For external users from other Azure AD organization, this will be the domain of the federated organization, for example `contoso.com`.</span></span><br><br><span data-ttu-id="067e0-123">Поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="067e0-123">Supports `$filter`.</span></span> <span data-ttu-id="067e0-124">512 знаков.</span><span class="sxs-lookup"><span data-stu-id="067e0-124">512 character limit.</span></span>|
|<span data-ttu-id="067e0-125">иссуерассигнедид</span><span class="sxs-lookup"><span data-stu-id="067e0-125">issuerAssignedId</span></span>|<span data-ttu-id="067e0-126">string</span><span class="sxs-lookup"><span data-stu-id="067e0-126">string</span></span>|<span data-ttu-id="067e0-127">Задает уникальный идентификатор, назначенный пользователю поставщиком.</span><span class="sxs-lookup"><span data-stu-id="067e0-127">Specifies the unique identifier assigned to the user by the issuer.</span></span> <span data-ttu-id="067e0-128">Сочетание **издателя** и **иссуерассигнедид** должно быть уникальным в пределах организации.</span><span class="sxs-lookup"><span data-stu-id="067e0-128">The combination of **issuer** and **issuerAssignedId** must be unique within the organization.</span></span> <span data-ttu-id="067e0-129">Представляет имя входа для пользователя, когда **сигнинтипе** имеет значение `emailAddress` или `userName` (Local Accounts).</span><span class="sxs-lookup"><span data-stu-id="067e0-129">Represents the sign-in name for the user, when **signInType** is set to `emailAddress` or `userName` (also known as local accounts).</span></span><br><span data-ttu-id="067e0-130">Если для **сигнинтипе** задано значение:</span><span class="sxs-lookup"><span data-stu-id="067e0-130">When **signInType** is set to:</span></span> <ul><li><span data-ttu-id="067e0-131">`emailAddress`(или начинается с `emailAddress` Like `emailAddress1`) **иссуерассигнедид** должен быть допустимым адресом электронной почты</span><span class="sxs-lookup"><span data-stu-id="067e0-131">`emailAddress`, (or starts with `emailAddress` like `emailAddress1`) **issuerAssignedId** must be a valid email address</span></span></li><li><span data-ttu-id="067e0-132">`userName`, **иссуерассигнедид** должна быть действительной [локальной частью адреса электронной почты](https://tools.ietf.org/html/rfc3696#section-3)</span><span class="sxs-lookup"><span data-stu-id="067e0-132">`userName`, **issuerAssignedId** must be a valid [local part of an email address](https://tools.ietf.org/html/rfc3696#section-3)</span></span></li></ul><span data-ttu-id="067e0-133">Поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="067e0-133">Supports `$filter`.</span></span> <span data-ttu-id="067e0-134">512 знаков.</span><span class="sxs-lookup"><span data-stu-id="067e0-134">512 character limit.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="067e0-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="067e0-135">JSON representation</span></span>

<span data-ttu-id="067e0-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="067e0-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.objectIdentity"
}-->

```json
{
  "signInType": "string",
  "issuer": "string",
  "issuerAssignedId": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "objectIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
