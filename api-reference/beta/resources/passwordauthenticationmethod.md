---
title: Тип ресурса passwordAuthenticationMethod
description: Представление пароля, зарегистрированного для пользователя.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 92e135b74bc68662749376298b4be44155b577b2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156695"
---
# <a name="passwordauthenticationmethod-resource-type"></a><span data-ttu-id="a013b-103">Тип ресурса passwordAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a013b-103">passwordAuthenticationMethod resource type</span></span>

<span data-ttu-id="a013b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a013b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a013b-105">Представление пароля пользователя.</span><span class="sxs-lookup"><span data-stu-id="a013b-105">A representation of a user's password.</span></span> <span data-ttu-id="a013b-106">В целях безопасности сам пароль никогда не возвращается в объекте, но для сброса пароля можно принять меры.</span><span class="sxs-lookup"><span data-stu-id="a013b-106">For security, the password itself will never be returned in the object, but action can be taken to reset a password.</span></span>

## <a name="methods"></a><span data-ttu-id="a013b-107">Методы</span><span class="sxs-lookup"><span data-stu-id="a013b-107">Methods</span></span>

| <span data-ttu-id="a013b-108">Метод</span><span class="sxs-lookup"><span data-stu-id="a013b-108">Method</span></span>       | <span data-ttu-id="a013b-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a013b-109">Return Type</span></span> | <span data-ttu-id="a013b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a013b-110">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="a013b-111">Список passwordAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="a013b-111">List passwordAuthenticationMethods</span></span>](../api/authentication-list-passwordmethods.md) | <span data-ttu-id="a013b-112">[Коллекция passwordAuthenticationMethod](passwordauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="a013b-112">[passwordAuthenticationMethod](passwordauthenticationmethod.md) collection</span></span> | <span data-ttu-id="a013b-113">Чтение свойств и связей всех объектов **passwordAuthenticationMethod** этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="a013b-113">Read the properties and relationships of all of this user's **passwordAuthenticationMethod** objects.</span></span> |
|[<span data-ttu-id="a013b-114">Get passwordAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a013b-114">Get passwordAuthenticationMethod</span></span>](../api/passwordauthenticationmethod-get.md) | [<span data-ttu-id="a013b-115">passwordAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a013b-115">passwordAuthenticationMethod</span></span>](passwordauthenticationmethod.md) | <span data-ttu-id="a013b-116">Чтение свойств и связей объекта **passwordAuthenticationMethod.**</span><span class="sxs-lookup"><span data-stu-id="a013b-116">Read the properties and relationships of a **passwordAuthenticationMethod** object.</span></span> |
|[<span data-ttu-id="a013b-117">Сброс пароля</span><span class="sxs-lookup"><span data-stu-id="a013b-117">Reset password</span></span>](../api/passwordauthenticationmethod-resetpassword.md)|<span data-ttu-id="a013b-118">Нет</span><span class="sxs-lookup"><span data-stu-id="a013b-118">None</span></span>|<span data-ttu-id="a013b-119">Сброс пароля пользователя в облаке и, если он синхронизирован, в локальной сети.</span><span class="sxs-lookup"><span data-stu-id="a013b-119">Reset a user's password in the cloud and, if synced, on-premises.</span></span>|

## <a name="properties"></a><span data-ttu-id="a013b-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="a013b-120">Properties</span></span>

| <span data-ttu-id="a013b-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="a013b-121">Property</span></span>     | <span data-ttu-id="a013b-122">Тип</span><span class="sxs-lookup"><span data-stu-id="a013b-122">Type</span></span>        | <span data-ttu-id="a013b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a013b-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a013b-124">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="a013b-124">creationDateTime</span></span>|<span data-ttu-id="a013b-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a013b-125">DateTimeOffset</span></span>|<span data-ttu-id="a013b-126">Дата и время последнего обновления пароля.</span><span class="sxs-lookup"><span data-stu-id="a013b-126">The date and time when this password was last updated.</span></span> <span data-ttu-id="a013b-127">Это свойство в настоящее время не заполнено.</span><span class="sxs-lookup"><span data-stu-id="a013b-127">This property is currently not populated.</span></span> <span data-ttu-id="a013b-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a013b-128">Read-only.</span></span> <span data-ttu-id="a013b-129">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="a013b-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a013b-130">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a013b-130">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a013b-131">id</span><span class="sxs-lookup"><span data-stu-id="a013b-131">id</span></span>|<span data-ttu-id="a013b-132">String</span><span class="sxs-lookup"><span data-stu-id="a013b-132">String</span></span>| <span data-ttu-id="a013b-133">Идентификатор этого пароля, зарегистрированного для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="a013b-133">The identifier of this password registered to this user.</span></span> <span data-ttu-id="a013b-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a013b-134">Read-only.</span></span>|
|<span data-ttu-id="a013b-135">password</span><span class="sxs-lookup"><span data-stu-id="a013b-135">password</span></span>|<span data-ttu-id="a013b-136">Строка</span><span class="sxs-lookup"><span data-stu-id="a013b-136">String</span></span>|<span data-ttu-id="a013b-137">Для обеспечения безопасности пароль всегда возвращается в качестве NULL из операции LIST или GET.</span><span class="sxs-lookup"><span data-stu-id="a013b-137">For security, the password is always returned as null from a LIST or GET operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a013b-138">Связи</span><span class="sxs-lookup"><span data-stu-id="a013b-138">Relationships</span></span>

<span data-ttu-id="a013b-139">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a013b-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a013b-140">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a013b-140">JSON representation</span></span>

<span data-ttu-id="a013b-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a013b-141">The following is a JSON representation of the resource.</span></span>

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


