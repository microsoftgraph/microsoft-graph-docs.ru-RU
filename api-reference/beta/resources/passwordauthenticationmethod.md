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
# <a name="passwordauthenticationmethod-resource-type"></a><span data-ttu-id="f4355-103">Тип ресурса Пассвордаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="f4355-103">passwordAuthenticationMethod resource type</span></span>

<span data-ttu-id="f4355-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4355-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4355-105">Представление пароля пользователя.</span><span class="sxs-lookup"><span data-stu-id="f4355-105">A representation of a user's password.</span></span> <span data-ttu-id="f4355-106">В целях безопасности сам пароль никогда не возвращается в объекте, но для сброса пароля можно предпринять действие.</span><span class="sxs-lookup"><span data-stu-id="f4355-106">For security, the password itself will never be returned in the object, but action can be taken to reset a password.</span></span>

## <a name="methods"></a><span data-ttu-id="f4355-107">Методы</span><span class="sxs-lookup"><span data-stu-id="f4355-107">Methods</span></span>

| <span data-ttu-id="f4355-108">Метод</span><span class="sxs-lookup"><span data-stu-id="f4355-108">Method</span></span>       | <span data-ttu-id="f4355-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f4355-109">Return Type</span></span> | <span data-ttu-id="f4355-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f4355-110">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="f4355-111">Список Пассвордаусентикатионмесодс</span><span class="sxs-lookup"><span data-stu-id="f4355-111">List passwordAuthenticationMethods</span></span>](../api/authentication-list-passwordmethods.md) | <span data-ttu-id="f4355-112">Коллекция [пассвордаусентикатионмесод](passwordauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="f4355-112">[passwordAuthenticationMethod](passwordauthenticationmethod.md) collection</span></span> | <span data-ttu-id="f4355-113">Чтение свойств и связей всех объектов **пассвордаусентикатионмесод** этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="f4355-113">Read the properties and relationships of all of this user's **passwordAuthenticationMethod** objects.</span></span> |
|[<span data-ttu-id="f4355-114">Получение Пассвордаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="f4355-114">Get passwordAuthenticationMethod</span></span>](../api/passwordauthenticationmethod-get.md) | [<span data-ttu-id="f4355-115">пассвордаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="f4355-115">passwordAuthenticationMethod</span></span>](passwordauthenticationmethod.md) | <span data-ttu-id="f4355-116">Чтение свойств и связей объекта **пассвордаусентикатионмесод** .</span><span class="sxs-lookup"><span data-stu-id="f4355-116">Read the properties and relationships of a **passwordAuthenticationMethod** object.</span></span> |
|[<span data-ttu-id="f4355-117">Сброс пароля</span><span class="sxs-lookup"><span data-stu-id="f4355-117">Reset password</span></span>](../api/passwordauthenticationmethod-resetpassword.md)|<span data-ttu-id="f4355-118">Нет</span><span class="sxs-lookup"><span data-stu-id="f4355-118">None</span></span>|<span data-ttu-id="f4355-119">Сброс пароля пользователя в облаке и, если синхронизация выполняется в локальной среде.</span><span class="sxs-lookup"><span data-stu-id="f4355-119">Reset a user's password in the cloud and, if synced, on-premises.</span></span>|

## <a name="properties"></a><span data-ttu-id="f4355-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="f4355-120">Properties</span></span>

| <span data-ttu-id="f4355-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4355-121">Property</span></span>     | <span data-ttu-id="f4355-122">Тип</span><span class="sxs-lookup"><span data-stu-id="f4355-122">Type</span></span>        | <span data-ttu-id="f4355-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f4355-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f4355-124">креатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="f4355-124">creationDateTime</span></span>|<span data-ttu-id="f4355-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4355-125">DateTimeOffset</span></span>|<span data-ttu-id="f4355-126">Дата и время последнего обновления этого пароля.</span><span class="sxs-lookup"><span data-stu-id="f4355-126">The date and time when this password was last updated.</span></span> <span data-ttu-id="f4355-127">В настоящее время это свойство не заполняется.</span><span class="sxs-lookup"><span data-stu-id="f4355-127">This property is currently not populated.</span></span> <span data-ttu-id="f4355-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4355-128">Read-only.</span></span> <span data-ttu-id="f4355-129">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="f4355-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f4355-130">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f4355-130">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f4355-131">id</span><span class="sxs-lookup"><span data-stu-id="f4355-131">id</span></span>|<span data-ttu-id="f4355-132">String</span><span class="sxs-lookup"><span data-stu-id="f4355-132">String</span></span>| <span data-ttu-id="f4355-133">Идентификатор этого пароля, зарегистрированный для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="f4355-133">The identifier of this password registered to this user.</span></span> <span data-ttu-id="f4355-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4355-134">Read-only.</span></span>|
|<span data-ttu-id="f4355-135">password</span><span class="sxs-lookup"><span data-stu-id="f4355-135">password</span></span>|<span data-ttu-id="f4355-136">Строка</span><span class="sxs-lookup"><span data-stu-id="f4355-136">String</span></span>|<span data-ttu-id="f4355-137">В целях безопасности пароль всегда возвращается как NULL из списка или операции GET.</span><span class="sxs-lookup"><span data-stu-id="f4355-137">For security, the password is always returned as null from a LIST or GET operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4355-138">Связи</span><span class="sxs-lookup"><span data-stu-id="f4355-138">Relationships</span></span>

<span data-ttu-id="f4355-139">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f4355-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4355-140">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f4355-140">JSON representation</span></span>

<span data-ttu-id="f4355-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4355-141">The following is a JSON representation of the resource.</span></span>

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
