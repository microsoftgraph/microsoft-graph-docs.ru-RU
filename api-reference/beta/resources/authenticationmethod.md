---
title: Тип ресурса authenticationMethod
description: Представляет метод проверки подлинности, зарегистрированный для пользователя.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d6afb785527b2d2448e54533ce02c0a72bf84353
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402347"
---
# <a name="authenticationmethod-resource-type"></a><span data-ttu-id="270bf-103">Тип ресурса authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="270bf-103">authenticationMethod resource type</span></span>

<span data-ttu-id="270bf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="270bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="270bf-105">Представляет метод проверки подлинности, зарегистрированный для пользователя.</span><span class="sxs-lookup"><span data-stu-id="270bf-105">Represents an authentication method registered to a user.</span></span> <span data-ttu-id="270bf-106">[Способ проверки подлинности](/azure/active-directory/authentication/concept-authentication-methods) используется пользователем для проверки подлинности или подтверждения удостоверения системы.</span><span class="sxs-lookup"><span data-stu-id="270bf-106">An [authentication method](/azure/active-directory/authentication/concept-authentication-methods) is something used by a user to authenticate or otherwise prove their identity to the system.</span></span> <span data-ttu-id="270bf-107">В качестве примеров можно привести пароль, Телефон (с помощью SMS или голосового вызова), ключи безопасности FIDO2 и многое другое.</span><span class="sxs-lookup"><span data-stu-id="270bf-107">Some examples include password, phone (usable via SMS or voice call), FIDO2 security keys, and more.</span></span> <span data-ttu-id="270bf-108">В настоящее время применяются методы Password и Phone.</span><span class="sxs-lookup"><span data-stu-id="270bf-108">Currently, password and phone methods are implemented.</span></span>

## <a name="methods"></a><span data-ttu-id="270bf-109">Методы</span><span class="sxs-lookup"><span data-stu-id="270bf-109">Methods</span></span>

| <span data-ttu-id="270bf-110">Метод</span><span class="sxs-lookup"><span data-stu-id="270bf-110">Method</span></span>       | <span data-ttu-id="270bf-111">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="270bf-111">Return type</span></span> | <span data-ttu-id="270bf-112">Описание</span><span class="sxs-lookup"><span data-stu-id="270bf-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="270bf-113">Список Аусентикатионмесодс</span><span class="sxs-lookup"><span data-stu-id="270bf-113">List authenticationMethods</span></span>](../api/authentication-list-methods.md) | <span data-ttu-id="270bf-114">Коллекция [authenticationMethod](authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="270bf-114">[authenticationMethod](authenticationmethod.md) collection</span></span> | <span data-ttu-id="270bf-115">Чтение свойств и связей всех объектов **authenticationMethod** пользователя.</span><span class="sxs-lookup"><span data-stu-id="270bf-115">Read the properties and relationships of all of a user's **authenticationMethod** objects.</span></span> |
| [<span data-ttu-id="270bf-116">Получение параметра authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="270bf-116">Get authenticationMethod</span></span>](../api/authenticationmethod-get.md) | [<span data-ttu-id="270bf-117">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="270bf-117">authenticationMethod</span></span>](authenticationmethod.md) | <span data-ttu-id="270bf-118">Чтение свойств и связей объекта **authenticationMethod** .</span><span class="sxs-lookup"><span data-stu-id="270bf-118">Read the properties and relationships of an **authenticationMethod** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="270bf-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="270bf-119">Properties</span></span>

| <span data-ttu-id="270bf-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="270bf-120">Property</span></span>     | <span data-ttu-id="270bf-121">Тип</span><span class="sxs-lookup"><span data-stu-id="270bf-121">Type</span></span>        | <span data-ttu-id="270bf-122">Описание</span><span class="sxs-lookup"><span data-stu-id="270bf-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="270bf-123">id</span><span class="sxs-lookup"><span data-stu-id="270bf-123">id</span></span>|<span data-ttu-id="270bf-124">String</span><span class="sxs-lookup"><span data-stu-id="270bf-124">String</span></span>| <span data-ttu-id="270bf-125">Идентификатор этого экземпляра метода проверки подлинности, зарегистрированный для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="270bf-125">The identifier of this instance of an authentication method registered to this user.</span></span> <span data-ttu-id="270bf-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="270bf-126">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="270bf-127">Связи</span><span class="sxs-lookup"><span data-stu-id="270bf-127">Relationships</span></span>

<span data-ttu-id="270bf-128">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="270bf-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="270bf-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="270bf-129">JSON representation</span></span>

<span data-ttu-id="270bf-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="270bf-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authenticationMethod",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "authenticationMethod resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->