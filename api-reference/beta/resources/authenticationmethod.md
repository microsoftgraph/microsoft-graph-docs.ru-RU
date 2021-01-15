---
title: Тип ресурса authenticationMethod
description: Представляет метод проверки подлинности, зарегистрированный для пользователя.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d1c43525352411a4b27952be4e6592401d28c54b
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874328"
---
# <a name="authenticationmethod-resource-type"></a><span data-ttu-id="86ccd-103">Тип ресурса authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="86ccd-103">authenticationMethod resource type</span></span>

<span data-ttu-id="86ccd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86ccd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86ccd-105">Представляет метод проверки подлинности, зарегистрированный для пользователя.</span><span class="sxs-lookup"><span data-stu-id="86ccd-105">Represents an authentication method registered to a user.</span></span> <span data-ttu-id="86ccd-106">Метод [проверки подлинности](/azure/active-directory/authentication/concept-authentication-methods) используется пользователем для проверки подлинности или иной проверки подлинности в системе.</span><span class="sxs-lookup"><span data-stu-id="86ccd-106">An [authentication method](/azure/active-directory/authentication/concept-authentication-methods) is something used by a user to authenticate or otherwise prove their identity to the system.</span></span> <span data-ttu-id="86ccd-107">Некоторые примеры включают пароль, телефон (можно использовать через SMS или голосовой вызов), ключи безопасности FIDO2 и другие.</span><span class="sxs-lookup"><span data-stu-id="86ccd-107">Some examples include password, phone (usable via SMS or voice call), FIDO2 security keys, and more.</span></span>

## <a name="methods"></a><span data-ttu-id="86ccd-108">Методы</span><span class="sxs-lookup"><span data-stu-id="86ccd-108">Methods</span></span>

| <span data-ttu-id="86ccd-109">Метод</span><span class="sxs-lookup"><span data-stu-id="86ccd-109">Method</span></span>       | <span data-ttu-id="86ccd-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="86ccd-110">Return type</span></span> | <span data-ttu-id="86ccd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="86ccd-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="86ccd-112">Список authenticationMethods</span><span class="sxs-lookup"><span data-stu-id="86ccd-112">List authenticationMethods</span></span>](../api/authentication-list-methods.md) | <span data-ttu-id="86ccd-113">[Коллекция authenticationMethod](authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="86ccd-113">[authenticationMethod](authenticationmethod.md) collection</span></span> | <span data-ttu-id="86ccd-114">Чтение свойств и связей всех объектов **authenticationMethod** пользователя.</span><span class="sxs-lookup"><span data-stu-id="86ccd-114">Read the properties and relationships of all of a user's **authenticationMethod** objects.</span></span> |
| [<span data-ttu-id="86ccd-115">Get authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="86ccd-115">Get authenticationMethod</span></span>](../api/authenticationmethod-get.md) | [<span data-ttu-id="86ccd-116">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="86ccd-116">authenticationMethod</span></span>](authenticationmethod.md) | <span data-ttu-id="86ccd-117">Чтение свойств и связей объекта **authenticationMethod.**</span><span class="sxs-lookup"><span data-stu-id="86ccd-117">Read the properties and relationships of an **authenticationMethod** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="86ccd-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="86ccd-118">Properties</span></span>

| <span data-ttu-id="86ccd-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="86ccd-119">Property</span></span>     | <span data-ttu-id="86ccd-120">Тип</span><span class="sxs-lookup"><span data-stu-id="86ccd-120">Type</span></span>        | <span data-ttu-id="86ccd-121">Описание</span><span class="sxs-lookup"><span data-stu-id="86ccd-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="86ccd-122">id</span><span class="sxs-lookup"><span data-stu-id="86ccd-122">id</span></span>|<span data-ttu-id="86ccd-123">String</span><span class="sxs-lookup"><span data-stu-id="86ccd-123">String</span></span>| <span data-ttu-id="86ccd-124">Идентификатор этого экземпляра метода проверки подлинности, зарегистрированного для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="86ccd-124">The identifier of this instance of an authentication method registered to this user.</span></span> <span data-ttu-id="86ccd-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="86ccd-125">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="86ccd-126">Связи</span><span class="sxs-lookup"><span data-stu-id="86ccd-126">Relationships</span></span>

<span data-ttu-id="86ccd-127">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="86ccd-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="86ccd-128">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="86ccd-128">JSON representation</span></span>

<span data-ttu-id="86ccd-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86ccd-129">The following is a JSON representation of the resource.</span></span>

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