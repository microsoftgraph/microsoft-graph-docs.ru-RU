---
title: тип ресурса objectIdentity
description: Представляет удостоверение, используемого для входов в учетную запись пользователя.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: jpettere
ms.openlocfilehash: 5f989325706ce45fe384370584b645959c153158
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080675"
---
# <a name="objectidentity-resource-type"></a><span data-ttu-id="62b63-103">тип ресурса objectIdentity</span><span class="sxs-lookup"><span data-stu-id="62b63-103">objectIdentity resource type</span></span>

<span data-ttu-id="62b63-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62b63-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="62b63-105">Представляет удостоверение, используемого для входов в учетную запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="62b63-105">Represents an identity used to sign in to a user account.</span></span> <span data-ttu-id="62b63-106">Удостоверение может быть предоставлено Корпорацией Майкрософт, организациями или поставщиками социальных удостоверений, такими как Facebook, Google или Microsoft, которые привязаны к учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="62b63-106">An identity can be provided by Microsoft, by organizations, or by social identity providers such as Facebook, Google, or Microsoft, that are tied to a user account.</span></span> <span data-ttu-id="62b63-107">Это позволяет пользователю войти в учетную запись пользователя с любым из связанных удостоверений.</span><span class="sxs-lookup"><span data-stu-id="62b63-107">This enables the user to sign in to the user account with any of those associated identities.</span></span>

<span data-ttu-id="62b63-108">Свойство **удостоверений** [пользовательского ресурса](user.md) — объект **objectIdentity.**</span><span class="sxs-lookup"><span data-stu-id="62b63-108">The **identities** property of the [user](user.md) resource is an **objectIdentity** object.</span></span>

## <a name="properties"></a><span data-ttu-id="62b63-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="62b63-109">Properties</span></span>

| <span data-ttu-id="62b63-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="62b63-110">Property</span></span>   | <span data-ttu-id="62b63-111">Тип</span><span class="sxs-lookup"><span data-stu-id="62b63-111">Type</span></span> |<span data-ttu-id="62b63-112">Описание</span><span class="sxs-lookup"><span data-stu-id="62b63-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62b63-113">signInType</span><span class="sxs-lookup"><span data-stu-id="62b63-113">signInType</span></span>|<span data-ttu-id="62b63-114">string</span><span class="sxs-lookup"><span data-stu-id="62b63-114">string</span></span>| <span data-ttu-id="62b63-115">Указывает типы входных данных пользователя в каталоге, такие как `emailAddress` , `userName` или `federated` .</span><span class="sxs-lookup"><span data-stu-id="62b63-115">Specifies the user sign-in types in your directory, such as `emailAddress`, `userName` or `federated`.</span></span> <span data-ttu-id="62b63-116">Здесь представлен уникальный идентификатор для пользователя от эмитента, который может быть в любом формате, `federated` выбранном эмитентом.</span><span class="sxs-lookup"><span data-stu-id="62b63-116">Here, `federated` represents a unique identifier for a user from an issuer, that can be in any format chosen by the issuer.</span></span> <span data-ttu-id="62b63-117">Дополнительные проверки применяются в **issuerAssignedId,** когда задан тип входного знака `emailAddress` или `userName` .</span><span class="sxs-lookup"><span data-stu-id="62b63-117">Additional validation is enforced on **issuerAssignedId** when the sign-in type is set to `emailAddress` or `userName`.</span></span> <span data-ttu-id="62b63-118">Это свойство также может быть заданной для любой настраиваемой строки.</span><span class="sxs-lookup"><span data-stu-id="62b63-118">This property can also be set to any custom string.</span></span>|
|<span data-ttu-id="62b63-119">эмитент</span><span class="sxs-lookup"><span data-stu-id="62b63-119">issuer</span></span>|<span data-ttu-id="62b63-120">string</span><span class="sxs-lookup"><span data-stu-id="62b63-120">string</span></span>|<span data-ttu-id="62b63-121">Указывает эмитент удостоверения, например `facebook.com` .</span><span class="sxs-lookup"><span data-stu-id="62b63-121">Specifies the issuer of the identity, for example `facebook.com`.</span></span><br><span data-ttu-id="62b63-122">Для локальных учетных записей (где **signInType** не является) это свойство является локальным доменным именем `federated` клиента B2C по умолчанию, например `contoso.onmicrosoft.com` .</span><span class="sxs-lookup"><span data-stu-id="62b63-122">For local accounts (where **signInType** is not `federated`), this property is the local B2C tenant default domain name, for example `contoso.onmicrosoft.com`.</span></span><br><span data-ttu-id="62b63-123">Для внешних пользователей из другой организации Azure AD это будет домен федерарной организации, например `contoso.com` .</span><span class="sxs-lookup"><span data-stu-id="62b63-123">For external users from other Azure AD organization, this will be the domain of the federated organization, for example `contoso.com`.</span></span><br><br><span data-ttu-id="62b63-124">Поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="62b63-124">Supports `$filter`.</span></span> <span data-ttu-id="62b63-125">Ограничение 512 символов.</span><span class="sxs-lookup"><span data-stu-id="62b63-125">512 character limit.</span></span>|
|<span data-ttu-id="62b63-126">issuerAssignedId</span><span class="sxs-lookup"><span data-stu-id="62b63-126">issuerAssignedId</span></span>|<span data-ttu-id="62b63-127">string</span><span class="sxs-lookup"><span data-stu-id="62b63-127">string</span></span>|<span data-ttu-id="62b63-128">Указывает уникальный идентификатор, присвоенный пользователю эмитентом.</span><span class="sxs-lookup"><span data-stu-id="62b63-128">Specifies the unique identifier assigned to the user by the issuer.</span></span> <span data-ttu-id="62b63-129">Сочетание **эмитента и** **issuerAssignedId должно** быть уникальным в организации.</span><span class="sxs-lookup"><span data-stu-id="62b63-129">The combination of **issuer** and **issuerAssignedId** must be unique within the organization.</span></span> <span data-ttu-id="62b63-130">Представляет имя входного знака для пользователя при зачете **signInType** `emailAddress` `userName` или (также известном как локальные учетные записи).</span><span class="sxs-lookup"><span data-stu-id="62b63-130">Represents the sign-in name for the user, when **signInType** is set to `emailAddress` or `userName` (also known as local accounts).</span></span><br><span data-ttu-id="62b63-131">При **входеInType** установлено:</span><span class="sxs-lookup"><span data-stu-id="62b63-131">When **signInType** is set to:</span></span> <ul><li><span data-ttu-id="62b63-132">`emailAddress`, (или настраиваемая строка, которая начинается с `emailAddress` `emailAddress1` типа) **issuerAssignedId** должен быть допустимым адресом электронной почты</span><span class="sxs-lookup"><span data-stu-id="62b63-132">`emailAddress`, (or a custom string that starts with `emailAddress` like `emailAddress1`) **issuerAssignedId** must be a valid email address</span></span></li><li><span data-ttu-id="62b63-133">`userName`, **issuerAssignedId** должен быть допустимой локальной [частью адреса электронной почты](https://tools.ietf.org/html/rfc3696#section-3)</span><span class="sxs-lookup"><span data-stu-id="62b63-133">`userName`, **issuerAssignedId** must be a valid [local part of an email address](https://tools.ietf.org/html/rfc3696#section-3)</span></span></li></ul><span data-ttu-id="62b63-134">Поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="62b63-134">Supports `$filter`.</span></span> <span data-ttu-id="62b63-135">Ограничение 100 символов.</span><span class="sxs-lookup"><span data-stu-id="62b63-135">100 character limit.</span></span>|

><span data-ttu-id="62b63-136">**Примечание:** При фильтрации свойств **удостоверений** необходимо предоставить  как эмитент, так **и issuerAssignedId.**</span><span class="sxs-lookup"><span data-stu-id="62b63-136">**Note:** When filtering on the **identities** property, you must supply both **issuer** and **issuerAssignedId**.</span></span>

## <a name="json-representation"></a><span data-ttu-id="62b63-137">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="62b63-137">JSON representation</span></span>

<span data-ttu-id="62b63-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62b63-138">The following is a JSON representation of the resource.</span></span>

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

