---
title: Тип ресурса b2cAuthenticationMethodsPolicy
description: Представляет метод проверки подлинности локальной учетной записи, зарегистрированный для пользователя, настроенного в клиенте Azure Active Directory (Azure AD) B2C.
localization_priority: Priority
author: namkedia
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3a7a7e5218e58891649a0caae7d7de43e5629288
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433168"
---
# <a name="b2cauthenticationmethodspolicy-resource-type"></a><span data-ttu-id="ebd91-103">Тип ресурса b2cAuthenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="ebd91-103">b2cAuthenticationMethodsPolicy resource type</span></span>

<span data-ttu-id="ebd91-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebd91-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebd91-105">Azure Active Directory (Azure AD) B2C позволяет администраторам клиента выбрать механизм разрешения конечным пользователям регистрироваться с помощью локальных учетных записей.</span><span class="sxs-lookup"><span data-stu-id="ebd91-105">Azure Active Directory (Azure AD) B2C allows tenant admins to choose a mechanism for letting end users register via local accounts.</span></span> <span data-ttu-id="ebd91-106">Локальные учетные записи — это учетные записи, в которых утверждение удостоверения выполняется посредством Azure AD, а не поставщиком федеративных удостоверений, например Google или Facebook и т. д.</span><span class="sxs-lookup"><span data-stu-id="ebd91-106">Local accounts are the accounts where Azure AD does the identity assertion, as opposed to a federated identity provider such as Google or Facebook etc.</span></span>

<span data-ttu-id="ebd91-107">Локальные учетные записи в Azure AD B2C не используют параметры и парадигмы из Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ebd91-107">The local accounts in Azure AD B2C do not follow the settings or paradigms from Azure AD.</span></span> <span data-ttu-id="ebd91-108">Политика методов проверки подлинности Azure AD не используется и не внедряется службой Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="ebd91-108">The Azure AD authentication methods policy is not used or enforced by Azure AD B2C.</span></span> <span data-ttu-id="ebd91-109">Azure AD B2C сохраняет эти параметры в другой политике, применяемой пользовательскими потоками.</span><span class="sxs-lookup"><span data-stu-id="ebd91-109">Azure AD B2C stores these settings in a different policy, which is consumed by user flows.</span></span>

## <a name="methods"></a><span data-ttu-id="ebd91-110">Методы</span><span class="sxs-lookup"><span data-stu-id="ebd91-110">Methods</span></span>

| <span data-ttu-id="ebd91-111">Метод</span><span class="sxs-lookup"><span data-stu-id="ebd91-111">Method</span></span>       | <span data-ttu-id="ebd91-112">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="ebd91-112">Return type</span></span> | <span data-ttu-id="ebd91-113">Описание</span><span class="sxs-lookup"><span data-stu-id="ebd91-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ebd91-114">Получение b2cAuthenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="ebd91-114">Get b2cAuthenticationMethodsPolicy</span></span>](../api/b2cauthenticationmethodspolicy-get.md) | [<span data-ttu-id="ebd91-115">b2cauthenticationmethodspolicy</span><span class="sxs-lookup"><span data-stu-id="ebd91-115">b2cauthenticationmethodspolicy</span></span>](b2cauthenticationmethodspolicy.md) | <span data-ttu-id="ebd91-116">Чтение свойств объекта **b2cauthenticationmethodspolicy**.</span><span class="sxs-lookup"><span data-stu-id="ebd91-116">Read the properties of a **b2cauthenticationmethodspolicy** object.</span></span> |
| [<span data-ttu-id="ebd91-117">Обновление b2cAuthenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="ebd91-117">Update b2cAuthenticationMethodsPolicy</span></span>](../api/b2cauthenticationmethodspolicy-update.md) | <span data-ttu-id="ebd91-118">Нет</span><span class="sxs-lookup"><span data-stu-id="ebd91-118">None</span></span> | <span data-ttu-id="ebd91-119">Обновление свойств объекта **b2cauthenticationmethodspolicy**.</span><span class="sxs-lookup"><span data-stu-id="ebd91-119">Update the properties of a **b2cauthenticationmethodspolicy** objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="ebd91-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="ebd91-120">Properties</span></span>

| <span data-ttu-id="ebd91-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="ebd91-121">Property</span></span>     | <span data-ttu-id="ebd91-122">Тип</span><span class="sxs-lookup"><span data-stu-id="ebd91-122">Type</span></span>        | <span data-ttu-id="ebd91-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ebd91-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ebd91-124">id</span><span class="sxs-lookup"><span data-stu-id="ebd91-124">id</span></span>|<span data-ttu-id="ebd91-125">String</span><span class="sxs-lookup"><span data-stu-id="ebd91-125">String</span></span>|<span data-ttu-id="ebd91-126">Идентификатор политики методов проверки подлинности B2C.</span><span class="sxs-lookup"><span data-stu-id="ebd91-126">The id of the B2C authentication methods policy.</span></span> <span data-ttu-id="ebd91-127">Это свойство только для чтения и ключ.</span><span class="sxs-lookup"><span data-stu-id="ebd91-127">This is a read only property and the key.</span></span>|
|<span data-ttu-id="ebd91-128">isEmailPasswordAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="ebd91-128">isEmailPasswordAuthenticationEnabled</span></span>|<span data-ttu-id="ebd91-129">Логическое</span><span class="sxs-lookup"><span data-stu-id="ebd91-129">Boolean</span></span>|<span data-ttu-id="ebd91-130">Администратор клиента может настраивать локальные учетные записи, используя электронную почту, если включен метод проверки подлинности электронной почты и пароля.</span><span class="sxs-lookup"><span data-stu-id="ebd91-130">The tenant admin can configure local accounts using email if the email and password authentication method is enabled.</span></span>|
|<span data-ttu-id="ebd91-131">isUserNameAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="ebd91-131">isUserNameAuthenticationEnabled</span></span>|<span data-ttu-id="ebd91-132">Логическое</span><span class="sxs-lookup"><span data-stu-id="ebd91-132">Boolean</span></span>|<span data-ttu-id="ebd91-133">Администратор клиента может настраивать локальные учетные записи, используя имя пользователя, если включен метод проверки подлинности электронной почты и пароля.</span><span class="sxs-lookup"><span data-stu-id="ebd91-133">The tenant admin can configure local accounts using username if the username and password authentication method is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebd91-134">Связи</span><span class="sxs-lookup"><span data-stu-id="ebd91-134">Relationships</span></span>

<span data-ttu-id="ebd91-135">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ebd91-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ebd91-136">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ebd91-136">JSON representation</span></span>

<span data-ttu-id="ebd91-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ebd91-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.b2cAuthenticationMethodsPolicy",
  "keyProperty": "id"
}-->

```json
{
    "id": "b2CAuthenticationMethodsPolicy",
    "isEmailPasswordAuthenticationEnabled": true,
    "isUserNameAuthenticationEnabled": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "b2cAuthenticationMethodsPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
