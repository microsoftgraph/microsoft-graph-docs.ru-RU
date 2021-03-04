---
title: passwordAuthenticationMethod resource type
description: Представление пароля, зарегистрированного пользователю.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2982b79df70b65bf09dff8f9b906ed85a8854b52
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444086"
---
# <a name="passwordauthenticationmethod-resource-type"></a><span data-ttu-id="e09c0-103">passwordAuthenticationMethod resource type</span><span class="sxs-lookup"><span data-stu-id="e09c0-103">passwordAuthenticationMethod resource type</span></span>

<span data-ttu-id="e09c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e09c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e09c0-105">Представление пароля пользователя.</span><span class="sxs-lookup"><span data-stu-id="e09c0-105">A representation of a user's password.</span></span> <span data-ttu-id="e09c0-106">Для безопасности сам пароль никогда не будет возвращен в объекте, но можно принять меры для сброса пароля.</span><span class="sxs-lookup"><span data-stu-id="e09c0-106">For security, the password itself will never be returned in the object, but action can be taken to reset a password.</span></span>

## <a name="methods"></a><span data-ttu-id="e09c0-107">Методы</span><span class="sxs-lookup"><span data-stu-id="e09c0-107">Methods</span></span>

| <span data-ttu-id="e09c0-108">Метод</span><span class="sxs-lookup"><span data-stu-id="e09c0-108">Method</span></span>       | <span data-ttu-id="e09c0-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e09c0-109">Return Type</span></span> | <span data-ttu-id="e09c0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e09c0-110">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="e09c0-111">Список passwordAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="e09c0-111">List passwordAuthenticationMethods</span></span>](../api/authentication-list-passwordmethods.md) | <span data-ttu-id="e09c0-112">[passwordAuthenticationMethod](passwordauthenticationmethod.md) collection</span><span class="sxs-lookup"><span data-stu-id="e09c0-112">[passwordAuthenticationMethod](passwordauthenticationmethod.md) collection</span></span> | <span data-ttu-id="e09c0-113">Ознакомьтесь с свойствами и отношениями всех объектов **passwordAuthenticationMethod.**</span><span class="sxs-lookup"><span data-stu-id="e09c0-113">Read the properties and relationships of all of this user's **passwordAuthenticationMethod** objects.</span></span> |
|[<span data-ttu-id="e09c0-114">Get passwordAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e09c0-114">Get passwordAuthenticationMethod</span></span>](../api/passwordauthenticationmethod-get.md) | [<span data-ttu-id="e09c0-115">passwordAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e09c0-115">passwordAuthenticationMethod</span></span>](passwordauthenticationmethod.md) | <span data-ttu-id="e09c0-116">Ознакомьтесь с свойствами и отношениями объекта **passwordAuthenticationMethod.**</span><span class="sxs-lookup"><span data-stu-id="e09c0-116">Read the properties and relationships of a **passwordAuthenticationMethod** object.</span></span> |
|[<span data-ttu-id="e09c0-117">Сброс пароля</span><span class="sxs-lookup"><span data-stu-id="e09c0-117">Reset password</span></span>](../api/passwordauthenticationmethod-resetpassword.md)|<span data-ttu-id="e09c0-118">Нет</span><span class="sxs-lookup"><span data-stu-id="e09c0-118">None</span></span>|<span data-ttu-id="e09c0-119">Сброс пароля пользователя в облаке и при синхронизации с локальной.</span><span class="sxs-lookup"><span data-stu-id="e09c0-119">Reset a user's password in the cloud and, if synced, on-premises.</span></span>|

## <a name="properties"></a><span data-ttu-id="e09c0-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="e09c0-120">Properties</span></span>

| <span data-ttu-id="e09c0-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="e09c0-121">Property</span></span>     | <span data-ttu-id="e09c0-122">Тип</span><span class="sxs-lookup"><span data-stu-id="e09c0-122">Type</span></span>        | <span data-ttu-id="e09c0-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e09c0-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e09c0-124">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="e09c0-124">creationDateTime</span></span>|<span data-ttu-id="e09c0-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e09c0-125">DateTimeOffset</span></span>|<span data-ttu-id="e09c0-126">Дата и время последнего обновления пароля.</span><span class="sxs-lookup"><span data-stu-id="e09c0-126">The date and time when this password was last updated.</span></span> <span data-ttu-id="e09c0-127">Это свойство в настоящее время не заполнено.</span><span class="sxs-lookup"><span data-stu-id="e09c0-127">This property is currently not populated.</span></span> <span data-ttu-id="e09c0-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e09c0-128">Read-only.</span></span> <span data-ttu-id="e09c0-129">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="e09c0-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e09c0-130">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e09c0-130">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e09c0-131">id</span><span class="sxs-lookup"><span data-stu-id="e09c0-131">id</span></span>|<span data-ttu-id="e09c0-132">String</span><span class="sxs-lookup"><span data-stu-id="e09c0-132">String</span></span>| <span data-ttu-id="e09c0-133">Идентификатор этого пароля, зарегистрированного для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="e09c0-133">The identifier of this password registered to this user.</span></span> <span data-ttu-id="e09c0-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e09c0-134">Read-only.</span></span>|
|<span data-ttu-id="e09c0-135">password</span><span class="sxs-lookup"><span data-stu-id="e09c0-135">password</span></span>|<span data-ttu-id="e09c0-136">Строка</span><span class="sxs-lookup"><span data-stu-id="e09c0-136">String</span></span>|<span data-ttu-id="e09c0-137">Для обеспечения безопасности пароль всегда возвращается в качестве null из операции LIST или GET.</span><span class="sxs-lookup"><span data-stu-id="e09c0-137">For security, the password is always returned as null from a LIST or GET operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e09c0-138">Связи</span><span class="sxs-lookup"><span data-stu-id="e09c0-138">Relationships</span></span>

<span data-ttu-id="e09c0-139">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e09c0-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e09c0-140">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e09c0-140">JSON representation</span></span>

<span data-ttu-id="e09c0-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e09c0-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordAuthenticationMethod",
  "keyProperty": "id"
}-->

```json
{
  "creationDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "password": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordAuthenticationMethod resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


