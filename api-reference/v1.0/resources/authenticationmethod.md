---
title: тип ресурса authenticationMethod
description: Представляет метод проверки подлинности, зарегистрированный пользователем.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6f45971e29e3d1823f9dc7cc733bc089f04662cb
ms.sourcegitcommit: 2d8b04725ea4eaf304f3da1056a6451457a4630f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/12/2021
ms.locfileid: "52335585"
---
# <a name="authenticationmethod-resource-type"></a><span data-ttu-id="1e519-103">тип ресурса authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1e519-103">authenticationMethod resource type</span></span>

<span data-ttu-id="1e519-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e519-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1e519-105">Представляет метод проверки подлинности, зарегистрированный пользователем.</span><span class="sxs-lookup"><span data-stu-id="1e519-105">Represents an authentication method registered to a user.</span></span> <span data-ttu-id="1e519-106">Метод [проверки подлинности](/azure/active-directory/authentication/concept-authentication-methods) — это то, что используется пользователем для проверки подлинности или иного доказательства его подлинности в системе.</span><span class="sxs-lookup"><span data-stu-id="1e519-106">An [authentication method](/azure/active-directory/authentication/concept-authentication-methods) is something used by a user to authenticate or otherwise prove their identity to the system.</span></span> <span data-ttu-id="1e519-107">Некоторые примеры включают пароль, телефон (можно использовать SMS или голосовой вызов), ключи безопасности FIDO2 и другие.</span><span class="sxs-lookup"><span data-stu-id="1e519-107">Some examples include password, phone (usable via SMS or voice call), FIDO2 security keys, and more.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="1e519-108">Перечисление методов проверки подлинности пользователей возвращает только методы, поддерживаемые в этой версии API.</span><span class="sxs-lookup"><span data-stu-id="1e519-108">Listing users' authentication methods only returns methods supported on this API version.</span></span> <span data-ttu-id="1e519-109">Обзор [API методов проверки подлинности Azure AD](authenticationmethods-overview.md) см. в списке поддерживаемых в настоящее время методов.</span><span class="sxs-lookup"><span data-stu-id="1e519-109">See [Azure AD authentication methods API overview](authenticationmethods-overview.md) for a list of currently supported methods.</span></span>

## <a name="methods"></a><span data-ttu-id="1e519-110">Методы</span><span class="sxs-lookup"><span data-stu-id="1e519-110">Methods</span></span>

| <span data-ttu-id="1e519-111">Метод</span><span class="sxs-lookup"><span data-stu-id="1e519-111">Method</span></span>       | <span data-ttu-id="1e519-112">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="1e519-112">Return type</span></span> | <span data-ttu-id="1e519-113">Описание</span><span class="sxs-lookup"><span data-stu-id="1e519-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1e519-114">Проверка подлинности спискаМетходы</span><span class="sxs-lookup"><span data-stu-id="1e519-114">List authenticationMethods</span></span>](../api/authentication-list-methods.md) | <span data-ttu-id="1e519-115">[коллекция authenticationMethod](authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="1e519-115">[authenticationMethod](authenticationmethod.md) collection</span></span> | <span data-ttu-id="1e519-116">Ознакомьтесь с свойствами и отношениями всех объектов проверки подлинности **пользователяMethod.**</span><span class="sxs-lookup"><span data-stu-id="1e519-116">Read the properties and relationships of all of a user's **authenticationMethod** objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="1e519-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e519-117">Properties</span></span>

| <span data-ttu-id="1e519-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e519-118">Property</span></span>     | <span data-ttu-id="1e519-119">Тип</span><span class="sxs-lookup"><span data-stu-id="1e519-119">Type</span></span>        | <span data-ttu-id="1e519-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1e519-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1e519-121">id</span><span class="sxs-lookup"><span data-stu-id="1e519-121">id</span></span>|<span data-ttu-id="1e519-122">String</span><span class="sxs-lookup"><span data-stu-id="1e519-122">String</span></span>| <span data-ttu-id="1e519-123">Идентификатор этого экземпляра метода проверки подлинности, зарегистрированного для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="1e519-123">The identifier of this instance of an authentication method registered to this user.</span></span> <span data-ttu-id="1e519-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1e519-124">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1e519-125">Связи</span><span class="sxs-lookup"><span data-stu-id="1e519-125">Relationships</span></span>

<span data-ttu-id="1e519-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1e519-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e519-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1e519-127">JSON representation</span></span>

<span data-ttu-id="1e519-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e519-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authenticationMethod",
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