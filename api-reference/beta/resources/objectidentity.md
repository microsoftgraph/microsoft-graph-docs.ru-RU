---
title: Тип ресурса Обжектидентити
description: Представляет идентификатор, используемый для входа в учетную запись пользователя.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: krbain
ms.openlocfilehash: 61d68865c0b1e77339b2e2ec2b0f27f095fc4e8f
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43109028"
---
# <a name="objectidentity-resource-type"></a><span data-ttu-id="36225-103">Тип ресурса Обжектидентити</span><span class="sxs-lookup"><span data-stu-id="36225-103">objectIdentity resource type</span></span>

<span data-ttu-id="36225-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36225-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36225-105">Представляет идентификатор, используемый для входа в учетную запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="36225-105">Represents an identity used to sign in to a user account.</span></span> <span data-ttu-id="36225-106">Удостоверение может предоставляться корпорацией Майкрософт, организациями или поставщиками социальных удостоверений, такими как Facebook, Google или Майкрософт, которые связаны с учетной записью пользователя.</span><span class="sxs-lookup"><span data-stu-id="36225-106">An identity can be provided by Microsoft, by organizations, or by social identity providers such as Facebook, Google, or Microsoft, that are tied to a user account.</span></span> <span data-ttu-id="36225-107">Это позволяет пользователю выполнить вход в учетную запись пользователя с любыми связанными удостоверениями.</span><span class="sxs-lookup"><span data-stu-id="36225-107">This enables the user to sign in to the user account with any of those associated identities.</span></span>

<span data-ttu-id="36225-108">Свойство **удостоверения** для ресурса [User](user.md) является объектом **обжектидентити** .</span><span class="sxs-lookup"><span data-stu-id="36225-108">The **identities** property of the [user](user.md) resource is an **objectIdentity** object.</span></span>

## <a name="properties"></a><span data-ttu-id="36225-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="36225-109">Properties</span></span>

| <span data-ttu-id="36225-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="36225-110">Property</span></span>   | <span data-ttu-id="36225-111">Тип</span><span class="sxs-lookup"><span data-stu-id="36225-111">Type</span></span> |<span data-ttu-id="36225-112">Описание</span><span class="sxs-lookup"><span data-stu-id="36225-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36225-113">сигнинтипе</span><span class="sxs-lookup"><span data-stu-id="36225-113">signInType</span></span>|<span data-ttu-id="36225-114">строка</span><span class="sxs-lookup"><span data-stu-id="36225-114">string</span></span>| <span data-ttu-id="36225-115">Задает типы входа пользователя в каталоге, например `emailAddress`, `userName` или. `federated`</span><span class="sxs-lookup"><span data-stu-id="36225-115">Specifies the user sign-in types in your directory, such as `emailAddress`, `userName` or `federated`.</span></span> <span data-ttu-id="36225-116">Здесь `federated` представляет уникальный идентификатор пользователя у поставщика, который может быть в любом формате, выбранном поставщиком.</span><span class="sxs-lookup"><span data-stu-id="36225-116">Here, `federated` represents a unique identifier for a user from an issuer, that can be in any format chosen by the issuer.</span></span> <span data-ttu-id="36225-117">Дополнительная проверка применяется к **иссуерассигнедид** , если для `emailAddress` параметра Тип входа задано значение или. `userName`</span><span class="sxs-lookup"><span data-stu-id="36225-117">Additional validation is enforced on **issuerAssignedId** when the sign-in type is set to `emailAddress` or `userName`.</span></span> <span data-ttu-id="36225-118">Этому свойству также можно присвоить любую настраиваемую строку.</span><span class="sxs-lookup"><span data-stu-id="36225-118">This property can also be set to any custom string.</span></span>|
|<span data-ttu-id="36225-119">имени</span><span class="sxs-lookup"><span data-stu-id="36225-119">issuer</span></span>|<span data-ttu-id="36225-120">строка</span><span class="sxs-lookup"><span data-stu-id="36225-120">string</span></span>|<span data-ttu-id="36225-121">Указывает издателя удостоверения, например `facebook.com`.</span><span class="sxs-lookup"><span data-stu-id="36225-121">Specifies the issuer of the identity, for example `facebook.com`.</span></span><br><span data-ttu-id="36225-122">Для локальных учетных записей **signInType** (где сигнинтипе `federated`— нет) это свойство является локальным именем домена по умолчанию для клиента `contoso.onmicrosoft.com`B2C, например.</span><span class="sxs-lookup"><span data-stu-id="36225-122">For local accounts (where **signInType** is not `federated`), this property is the local B2C tenant default domain name, for example `contoso.onmicrosoft.com`.</span></span><br><span data-ttu-id="36225-123">Для внешних пользователей из другой организации Azure AD это будет домен федеративной организации, например `contoso.com`.</span><span class="sxs-lookup"><span data-stu-id="36225-123">For external users from other Azure AD organization, this will be the domain of the federated organization, for example `contoso.com`.</span></span><br><br><span data-ttu-id="36225-124">Поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="36225-124">Supports `$filter`.</span></span> <span data-ttu-id="36225-125">512 знаков.</span><span class="sxs-lookup"><span data-stu-id="36225-125">512 character limit.</span></span>|
|<span data-ttu-id="36225-126">иссуерассигнедид</span><span class="sxs-lookup"><span data-stu-id="36225-126">issuerAssignedId</span></span>|<span data-ttu-id="36225-127">строка</span><span class="sxs-lookup"><span data-stu-id="36225-127">string</span></span>|<span data-ttu-id="36225-128">Задает уникальный идентификатор, назначенный пользователю поставщиком.</span><span class="sxs-lookup"><span data-stu-id="36225-128">Specifies the unique identifier assigned to the user by the issuer.</span></span> <span data-ttu-id="36225-129">Сочетание **издателя** и **иссуерассигнедид** должно быть уникальным в пределах организации.</span><span class="sxs-lookup"><span data-stu-id="36225-129">The combination of **issuer** and **issuerAssignedId** must be unique within the organization.</span></span> <span data-ttu-id="36225-130">Представляет имя входа для пользователя, когда **сигнинтипе** имеет значение `emailAddress` или `userName` (Local Accounts).</span><span class="sxs-lookup"><span data-stu-id="36225-130">Represents the sign-in name for the user, when **signInType** is set to `emailAddress` or `userName` (also known as local accounts).</span></span><br><span data-ttu-id="36225-131">Если для **сигнинтипе** задано значение:</span><span class="sxs-lookup"><span data-stu-id="36225-131">When **signInType** is set to:</span></span> <ul><li><span data-ttu-id="36225-132">`emailAddress`(или начинается с `emailAddress` Like `emailAddress1`) **иссуерассигнедид** должен быть допустимым адресом электронной почты</span><span class="sxs-lookup"><span data-stu-id="36225-132">`emailAddress`, (or starts with `emailAddress` like `emailAddress1`) **issuerAssignedId** must be a valid email address</span></span></li><li><span data-ttu-id="36225-133">`userName`, **иссуерассигнедид** должна быть действительной [локальной частью адреса электронной почты](https://tools.ietf.org/html/rfc3696#section-3)</span><span class="sxs-lookup"><span data-stu-id="36225-133">`userName`, **issuerAssignedId** must be a valid [local part of an email address](https://tools.ietf.org/html/rfc3696#section-3)</span></span></li></ul><span data-ttu-id="36225-134">Поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="36225-134">Supports `$filter`.</span></span> <span data-ttu-id="36225-135">512 знаков.</span><span class="sxs-lookup"><span data-stu-id="36225-135">512 character limit.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="36225-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="36225-136">JSON representation</span></span>

<span data-ttu-id="36225-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36225-137">The following is a JSON representation of the resource.</span></span>

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
