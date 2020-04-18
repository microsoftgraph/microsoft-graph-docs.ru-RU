---
title: Тип ресурса Пассвордаусентикатионмесод
description: Представление пароля, зарегистрированного для пользователя.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ba932538e984af37a4f005ddcc2167c29d2267d0
ms.sourcegitcommit: 9c16d84eac9c34134864ad63a9bb95c309218a44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/18/2020
ms.locfileid: "43557915"
---
# <a name="passwordauthenticationmethod-resource-type"></a><span data-ttu-id="8573e-103">Тип ресурса Пассвордаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="8573e-103">passwordAuthenticationMethod resource type</span></span>

<span data-ttu-id="8573e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8573e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8573e-105">Представление пароля пользователя.</span><span class="sxs-lookup"><span data-stu-id="8573e-105">A representation of a user's password.</span></span> <span data-ttu-id="8573e-106">В целях безопасности сам пароль никогда не возвращается в объекте, но для сброса пароля можно предпринять действие.</span><span class="sxs-lookup"><span data-stu-id="8573e-106">For security, the password itself will never be returned in the object, but action can be taken to reset a password.</span></span>

## <a name="methods"></a><span data-ttu-id="8573e-107">Методы</span><span class="sxs-lookup"><span data-stu-id="8573e-107">Methods</span></span>

| <span data-ttu-id="8573e-108">Метод</span><span class="sxs-lookup"><span data-stu-id="8573e-108">Method</span></span>       | <span data-ttu-id="8573e-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8573e-109">Return Type</span></span> | <span data-ttu-id="8573e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8573e-110">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="8573e-111">Список Пассвордаусентикатионмесодс</span><span class="sxs-lookup"><span data-stu-id="8573e-111">List passwordAuthenticationMethods</span></span>](../api/authentication-list-passwordmethods.md) | <span data-ttu-id="8573e-112">Коллекция [пассвордаусентикатионмесод](passwordauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="8573e-112">[passwordAuthenticationMethod](passwordauthenticationmethod.md) collection</span></span> | <span data-ttu-id="8573e-113">Чтение свойств и связей всех объектов **пассвордаусентикатионмесод** этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="8573e-113">Read the properties and relationships of all of this user's **passwordAuthenticationMethod** objects.</span></span> |
|[<span data-ttu-id="8573e-114">Получение Пассвордаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="8573e-114">Get passwordAuthenticationMethod</span></span>](../api/passwordauthenticationmethod-get.md) | [<span data-ttu-id="8573e-115">пассвордаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="8573e-115">passwordAuthenticationMethod</span></span>](passwordauthenticationmethod.md) | <span data-ttu-id="8573e-116">Чтение свойств и связей объекта **пассвордаусентикатионмесод** .</span><span class="sxs-lookup"><span data-stu-id="8573e-116">Read the properties and relationships of a **passwordAuthenticationMethod** object.</span></span> |
|[<span data-ttu-id="8573e-117">Сброс пароля</span><span class="sxs-lookup"><span data-stu-id="8573e-117">Reset password</span></span>](../api/passwordauthenticationmethod-resetpassword.md)|<span data-ttu-id="8573e-118">Нет</span><span class="sxs-lookup"><span data-stu-id="8573e-118">None</span></span>|<span data-ttu-id="8573e-119">Сброс пароля пользователя в облаке и, если синхронизация выполняется в локальной среде.</span><span class="sxs-lookup"><span data-stu-id="8573e-119">Reset a user's password in the cloud and, if synced, on-premises.</span></span>|

## <a name="properties"></a><span data-ttu-id="8573e-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="8573e-120">Properties</span></span>

| <span data-ttu-id="8573e-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="8573e-121">Property</span></span>     | <span data-ttu-id="8573e-122">Тип</span><span class="sxs-lookup"><span data-stu-id="8573e-122">Type</span></span>        | <span data-ttu-id="8573e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8573e-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8573e-124">креатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="8573e-124">creationDateTime</span></span>|<span data-ttu-id="8573e-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8573e-125">DateTimeOffset</span></span>|<span data-ttu-id="8573e-126">Дата и время последнего обновления этого пароля.</span><span class="sxs-lookup"><span data-stu-id="8573e-126">The date and time when this password was last updated.</span></span> <span data-ttu-id="8573e-127">В настоящее время это свойство не заполняется.</span><span class="sxs-lookup"><span data-stu-id="8573e-127">This property is currently not populated.</span></span> <span data-ttu-id="8573e-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8573e-128">Read-only.</span></span> <span data-ttu-id="8573e-129">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="8573e-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8573e-130">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8573e-130">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8573e-131">id</span><span class="sxs-lookup"><span data-stu-id="8573e-131">id</span></span>|<span data-ttu-id="8573e-132">String</span><span class="sxs-lookup"><span data-stu-id="8573e-132">String</span></span>| <span data-ttu-id="8573e-133">Идентификатор этого пароля, зарегистрированный для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="8573e-133">The identifier of this password registered to this user.</span></span> <span data-ttu-id="8573e-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8573e-134">Read-only.</span></span>|
|<span data-ttu-id="8573e-135">password</span><span class="sxs-lookup"><span data-stu-id="8573e-135">password</span></span>|<span data-ttu-id="8573e-136">Строка</span><span class="sxs-lookup"><span data-stu-id="8573e-136">String</span></span>|<span data-ttu-id="8573e-137">В целях безопасности пароль всегда возвращается как NULL из списка или операции GET.</span><span class="sxs-lookup"><span data-stu-id="8573e-137">For security, the password is always returned as null from a LIST or GET operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8573e-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="8573e-138">Relationships</span></span>

<span data-ttu-id="8573e-139">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8573e-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8573e-140">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8573e-140">JSON representation</span></span>

<span data-ttu-id="8573e-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8573e-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordAuthenticationMethod",
  "baseType": "",
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
