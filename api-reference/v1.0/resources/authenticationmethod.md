---
title: тип ресурса authenticationMethod
description: Представляет метод проверки подлинности, зарегистрированный пользователем.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b052a6034484a5d1d1f8edc8ff9adc3feac52e98
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469138"
---
# <a name="authenticationmethod-resource-type"></a><span data-ttu-id="8ff78-103">тип ресурса authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8ff78-103">authenticationMethod resource type</span></span>

<span data-ttu-id="8ff78-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ff78-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8ff78-105">Представляет метод проверки подлинности, зарегистрированный пользователем.</span><span class="sxs-lookup"><span data-stu-id="8ff78-105">Represents an authentication method registered to a user.</span></span> <span data-ttu-id="8ff78-106">Метод [проверки подлинности](/azure/active-directory/authentication/concept-authentication-methods) — это то, что используется пользователем для проверки подлинности или иного доказательства его подлинности в системе.</span><span class="sxs-lookup"><span data-stu-id="8ff78-106">An [authentication method](/azure/active-directory/authentication/concept-authentication-methods) is something used by a user to authenticate or otherwise prove their identity to the system.</span></span> <span data-ttu-id="8ff78-107">Некоторые примеры включают пароль, телефон (можно использовать с помощью SMS или голосового звонка), ключи безопасности FIDO2 и другие.</span><span class="sxs-lookup"><span data-stu-id="8ff78-107">Some examples include password, phone (usable via SMS or voice call), FIDO2 security keys, and more.</span></span>

## <a name="methods"></a><span data-ttu-id="8ff78-108">Методы</span><span class="sxs-lookup"><span data-stu-id="8ff78-108">Methods</span></span>

| <span data-ttu-id="8ff78-109">Метод</span><span class="sxs-lookup"><span data-stu-id="8ff78-109">Method</span></span>       | <span data-ttu-id="8ff78-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="8ff78-110">Return type</span></span> | <span data-ttu-id="8ff78-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8ff78-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8ff78-112">Проверка подлинности спискаМетходы</span><span class="sxs-lookup"><span data-stu-id="8ff78-112">List authenticationMethods</span></span>](../api/authentication-list-methods.md) | <span data-ttu-id="8ff78-113">[коллекция authenticationMethod](authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="8ff78-113">[authenticationMethod](authenticationmethod.md) collection</span></span> | <span data-ttu-id="8ff78-114">Ознакомьтесь с свойствами и отношениями всех объектов проверки подлинности **пользователяMethod.**</span><span class="sxs-lookup"><span data-stu-id="8ff78-114">Read the properties and relationships of all of a user's **authenticationMethod** objects.</span></span> |
| [<span data-ttu-id="8ff78-115">Получить проверку подлинностиMethod</span><span class="sxs-lookup"><span data-stu-id="8ff78-115">Get authenticationMethod</span></span>](../api/authenticationmethod-get.md) | [<span data-ttu-id="8ff78-116">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8ff78-116">authenticationMethod</span></span>](authenticationmethod.md) | <span data-ttu-id="8ff78-117">Ознакомьтесь с свойствами и отношениями объекта **authenticationMethod.**</span><span class="sxs-lookup"><span data-stu-id="8ff78-117">Read the properties and relationships of an **authenticationMethod** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8ff78-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="8ff78-118">Properties</span></span>

| <span data-ttu-id="8ff78-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ff78-119">Property</span></span>     | <span data-ttu-id="8ff78-120">Тип</span><span class="sxs-lookup"><span data-stu-id="8ff78-120">Type</span></span>        | <span data-ttu-id="8ff78-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8ff78-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8ff78-122">id</span><span class="sxs-lookup"><span data-stu-id="8ff78-122">id</span></span>|<span data-ttu-id="8ff78-123">String</span><span class="sxs-lookup"><span data-stu-id="8ff78-123">String</span></span>| <span data-ttu-id="8ff78-124">Идентификатор этого экземпляра метода проверки подлинности, зарегистрированного для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="8ff78-124">The identifier of this instance of an authentication method registered to this user.</span></span> <span data-ttu-id="8ff78-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8ff78-125">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8ff78-126">Связи</span><span class="sxs-lookup"><span data-stu-id="8ff78-126">Relationships</span></span>

<span data-ttu-id="8ff78-127">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8ff78-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ff78-128">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8ff78-128">JSON representation</span></span>

<span data-ttu-id="8ff78-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ff78-129">The following is a JSON representation of the resource.</span></span>

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