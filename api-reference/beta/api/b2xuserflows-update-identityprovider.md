---
title: Добавление identityProvider в b2xUserFlow
description: Добавление identityProvider в b2xUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0e65a9f0df3ad54526cda89ab72cce9566d22a48
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991371"
---
# <a name="add-identityprovider-to-a-b2xuserflow"></a><span data-ttu-id="aaa0c-103">Добавление identityProvider в b2xUserFlow</span><span class="sxs-lookup"><span data-stu-id="aaa0c-103">Add identityProvider to a b2xUserFlow</span></span>

<span data-ttu-id="aaa0c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aaa0c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aaa0c-105">Обновление поставщиков удостоверений в объекте [b2xUserFlow](../resources/b2xuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="aaa0c-105">Update the identity providers in a [b2xUserFlow](../resources/b2xuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="aaa0c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aaa0c-106">Permissions</span></span>

<span data-ttu-id="aaa0c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aaa0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaa0c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aaa0c-109">Permission type</span></span>      | <span data-ttu-id="aaa0c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aaa0c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aaa0c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aaa0c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="aaa0c-112">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="aaa0c-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="aaa0c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aaa0c-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="aaa0c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aaa0c-114">Not supported.</span></span>|
|<span data-ttu-id="aaa0c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aaa0c-115">Application</span></span>| <span data-ttu-id="aaa0c-116">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="aaa0c-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="aaa0c-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="aaa0c-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="aaa0c-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="aaa0c-118">Global administrator</span></span>
* <span data-ttu-id="aaa0c-119">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="aaa0c-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="aaa0c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aaa0c-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /b2xUserFlows/{id}/identityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="aaa0c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aaa0c-121">Request headers</span></span>

|<span data-ttu-id="aaa0c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="aaa0c-122">Name</span></span>|<span data-ttu-id="aaa0c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="aaa0c-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="aaa0c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aaa0c-124">Authorization</span></span>|<span data-ttu-id="aaa0c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aaa0c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="aaa0c-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aaa0c-127">Content-Type</span></span>|<span data-ttu-id="aaa0c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aaa0c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aaa0c-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aaa0c-130">Request body</span></span>

<span data-ttu-id="aaa0c-131">В тексте запроса укажите представление объекта IdentityProvider, который требуется добавить, в формате JSON `id` . [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="aaa0c-131">In the request body, provide a JSON representation of the `id` of the [identityProvider](../resources/identityprovider.md) you want to add.</span></span> <span data-ttu-id="aaa0c-132">Для самостоятельной регистрации пользовательских потоков значения могут быть `Google-OAUTH` или `Facebook-OAUTH` .</span><span class="sxs-lookup"><span data-stu-id="aaa0c-132">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="response"></a><span data-ttu-id="aaa0c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="aaa0c-133">Response</span></span>

<span data-ttu-id="aaa0c-134">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="aaa0c-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="aaa0c-135">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="aaa0c-135">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="aaa0c-136">Пример</span><span class="sxs-lookup"><span data-stu-id="aaa0c-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="aaa0c-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="aaa0c-137">Request</span></span>

<span data-ttu-id="aaa0c-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aaa0c-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="aaa0c-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="aaa0c-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="aaa0c-140">C#</span><span class="sxs-lookup"><span data-stu-id="aaa0c-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-b2xuserflows-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aaa0c-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aaa0c-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-b2xuserflows-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aaa0c-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aaa0c-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-b2xuserflows-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="aaa0c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="aaa0c-143">Response</span></span>

<span data-ttu-id="aaa0c-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="aaa0c-144">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


