---
title: Добавление identityProvider в b2xIdentityUserFlow
description: Добавление identityProvider в b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0a681c3531799175eec9264166fa716fd59ea08f
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406435"
---
# <a name="add-identityprovider-to-a-b2xidentityuserflow"></a><span data-ttu-id="ce3fb-103">Добавление identityProvider в b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="ce3fb-103">Add identityProvider to a b2xIdentityUserFlow</span></span>

<span data-ttu-id="ce3fb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce3fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce3fb-105">Обновление поставщиков удостоверений в объекте [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="ce3fb-105">Update the identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce3fb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ce3fb-106">Permissions</span></span>

<span data-ttu-id="ce3fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce3fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce3fb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce3fb-109">Permission type</span></span>      | <span data-ttu-id="ce3fb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce3fb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce3fb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce3fb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ce3fb-112">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ce3fb-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="ce3fb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce3fb-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ce3fb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce3fb-114">Not supported.</span></span>|
|<span data-ttu-id="ce3fb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce3fb-115">Application</span></span>| <span data-ttu-id="ce3fb-116">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ce3fb-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="ce3fb-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="ce3fb-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="ce3fb-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ce3fb-118">Global administrator</span></span>
* <span data-ttu-id="ce3fb-119">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="ce3fb-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="ce3fb-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce3fb-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /b2xUserFlows/{id}/identityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="ce3fb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce3fb-121">Request headers</span></span>

|<span data-ttu-id="ce3fb-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ce3fb-122">Name</span></span>|<span data-ttu-id="ce3fb-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ce3fb-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="ce3fb-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ce3fb-124">Authorization</span></span>|<span data-ttu-id="ce3fb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce3fb-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ce3fb-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ce3fb-127">Content-Type</span></span>|<span data-ttu-id="ce3fb-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce3fb-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce3fb-130">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce3fb-130">Request body</span></span>

<span data-ttu-id="ce3fb-131">В тексте запроса укажите представление объекта IdentityProvider, который требуется добавить, в формате JSON `id` . [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="ce3fb-131">In the request body, provide a JSON representation of the `id` of the [identityProvider](../resources/identityprovider.md) you want to add.</span></span> <span data-ttu-id="ce3fb-132">Для самостоятельной регистрации пользовательских потоков значения могут быть `Google-OAUTH` или `Facebook-OAUTH` .</span><span class="sxs-lookup"><span data-stu-id="ce3fb-132">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="response"></a><span data-ttu-id="ce3fb-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce3fb-133">Response</span></span>

<span data-ttu-id="ce3fb-134">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ce3fb-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="ce3fb-135">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="ce3fb-135">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="ce3fb-136">Пример</span><span class="sxs-lookup"><span data-stu-id="ce3fb-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce3fb-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce3fb-137">Request</span></span>

<span data-ttu-id="ce3fb-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce3fb-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ce3fb-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce3fb-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_b2xuserflows_identityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}/identityProviders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/identityProviders/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="ce3fb-140">C#</span><span class="sxs-lookup"><span data-stu-id="ce3fb-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-b2xuserflows-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ce3fb-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce3fb-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-b2xuserflows-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ce3fb-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce3fb-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-b2xuserflows-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ce3fb-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce3fb-143">Response</span></span>

<span data-ttu-id="ce3fb-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ce3fb-144">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


