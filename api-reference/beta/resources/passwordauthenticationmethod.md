---
title: passwordAuthenticationMethod resource type
description: Представление пароля, зарегистрированного пользователю.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f902d47d0d06857537a07541456596c3a6204bc3
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720580"
---
# <a name="passwordauthenticationmethod-resource-type"></a><span data-ttu-id="c2bfc-103">passwordAuthenticationMethod resource type</span><span class="sxs-lookup"><span data-stu-id="c2bfc-103">passwordAuthenticationMethod resource type</span></span>

<span data-ttu-id="c2bfc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2bfc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2bfc-105">Представление пароля пользователя.</span><span class="sxs-lookup"><span data-stu-id="c2bfc-105">A representation of a user's password.</span></span> <span data-ttu-id="c2bfc-106">Для безопасности сам пароль никогда не будет возвращен в объекте, но можно принять меры для сброса пароля.</span><span class="sxs-lookup"><span data-stu-id="c2bfc-106">For security, the password itself will never be returned in the object, but action can be taken to reset a password.</span></span>

## <a name="methods"></a><span data-ttu-id="c2bfc-107">Методы</span><span class="sxs-lookup"><span data-stu-id="c2bfc-107">Methods</span></span>

| <span data-ttu-id="c2bfc-108">Метод</span><span class="sxs-lookup"><span data-stu-id="c2bfc-108">Method</span></span>       | <span data-ttu-id="c2bfc-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c2bfc-109">Return Type</span></span> | <span data-ttu-id="c2bfc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c2bfc-110">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="c2bfc-111">Список passwordAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="c2bfc-111">List passwordAuthenticationMethods</span></span>](../api/authentication-list-passwordmethods.md) | <span data-ttu-id="c2bfc-112">[passwordAuthenticationMethod](passwordauthenticationmethod.md) collection</span><span class="sxs-lookup"><span data-stu-id="c2bfc-112">[passwordAuthenticationMethod](passwordauthenticationmethod.md) collection</span></span> | <span data-ttu-id="c2bfc-113">Ознакомьтесь с свойствами и отношениями всех объектов **passwordAuthenticationMethod.**</span><span class="sxs-lookup"><span data-stu-id="c2bfc-113">Read the properties and relationships of all of this user's **passwordAuthenticationMethod** objects.</span></span> |
|[<span data-ttu-id="c2bfc-114">Get passwordAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c2bfc-114">Get passwordAuthenticationMethod</span></span>](../api/passwordauthenticationmethod-get.md) | [<span data-ttu-id="c2bfc-115">passwordAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c2bfc-115">passwordAuthenticationMethod</span></span>](passwordauthenticationmethod.md) | <span data-ttu-id="c2bfc-116">Ознакомьтесь с свойствами и отношениями объекта **passwordAuthenticationMethod.**</span><span class="sxs-lookup"><span data-stu-id="c2bfc-116">Read the properties and relationships of a **passwordAuthenticationMethod** object.</span></span> |
|[<span data-ttu-id="c2bfc-117">Сброс пароля</span><span class="sxs-lookup"><span data-stu-id="c2bfc-117">Reset password</span></span>](../api/passwordauthenticationmethod-resetpassword.md)|<span data-ttu-id="c2bfc-118">Нет</span><span class="sxs-lookup"><span data-stu-id="c2bfc-118">None</span></span>|<span data-ttu-id="c2bfc-119">Сброс пароля пользователя в облаке и при синхронизации с локальной.</span><span class="sxs-lookup"><span data-stu-id="c2bfc-119">Reset a user's password in the cloud and, if synced, on-premises.</span></span>|

## <a name="properties"></a><span data-ttu-id="c2bfc-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2bfc-120">Properties</span></span>

| <span data-ttu-id="c2bfc-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2bfc-121">Property</span></span>     | <span data-ttu-id="c2bfc-122">Тип</span><span class="sxs-lookup"><span data-stu-id="c2bfc-122">Type</span></span>        | <span data-ttu-id="c2bfc-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c2bfc-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c2bfc-124">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="c2bfc-124">creationDateTime</span></span>|<span data-ttu-id="c2bfc-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2bfc-125">DateTimeOffset</span></span>|<span data-ttu-id="c2bfc-126">Дата и время последнего обновления пароля.</span><span class="sxs-lookup"><span data-stu-id="c2bfc-126">The date and time when this password was last updated.</span></span> <span data-ttu-id="c2bfc-127">Это свойство в настоящее время не заполнено.</span><span class="sxs-lookup"><span data-stu-id="c2bfc-127">This property is currently not populated.</span></span> <span data-ttu-id="c2bfc-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2bfc-128">Read-only.</span></span> <span data-ttu-id="c2bfc-129">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="c2bfc-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c2bfc-130">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="c2bfc-130">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="c2bfc-131">id</span><span class="sxs-lookup"><span data-stu-id="c2bfc-131">id</span></span>|<span data-ttu-id="c2bfc-132">String</span><span class="sxs-lookup"><span data-stu-id="c2bfc-132">String</span></span>| <span data-ttu-id="c2bfc-133">Идентификатор этого пароля, зарегистрированного для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="c2bfc-133">The identifier of this password registered to this user.</span></span> <span data-ttu-id="c2bfc-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2bfc-134">Read-only.</span></span>|
|<span data-ttu-id="c2bfc-135">password</span><span class="sxs-lookup"><span data-stu-id="c2bfc-135">password</span></span>|<span data-ttu-id="c2bfc-136">Строка</span><span class="sxs-lookup"><span data-stu-id="c2bfc-136">String</span></span>|<span data-ttu-id="c2bfc-137">Для обеспечения безопасности пароль всегда возвращается в качестве null из операции LIST или GET.</span><span class="sxs-lookup"><span data-stu-id="c2bfc-137">For security, the password is always returned as null from a LIST or GET operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2bfc-138">Связи</span><span class="sxs-lookup"><span data-stu-id="c2bfc-138">Relationships</span></span>

<span data-ttu-id="c2bfc-139">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c2bfc-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2bfc-140">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c2bfc-140">JSON representation</span></span>

<span data-ttu-id="c2bfc-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2bfc-141">The following is a JSON representation of the resource.</span></span>

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


