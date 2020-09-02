---
title: Добавление identityProvider в b2cUserFlow
description: Добавление identityProvider в b2cUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2365d16255543a99562be41fb8b3742972293fca
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329662"
---
# <a name="add-identityprovider-to-a-b2cuserflow"></a><span data-ttu-id="5b6ec-103">Добавление identityProvider в b2cUserFlow</span><span class="sxs-lookup"><span data-stu-id="5b6ec-103">Add identityProvider to a b2cUserFlow</span></span>

<span data-ttu-id="5b6ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b6ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b6ec-105">Добавление поставщиков удостоверений в объект [b2cUserFlow](../resources/b2cuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="5b6ec-105">Add identity providers in a [b2cUserFlow](../resources/b2cuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b6ec-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5b6ec-106">Permissions</span></span>

<span data-ttu-id="5b6ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b6ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b6ec-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b6ec-109">Permission type</span></span>      | <span data-ttu-id="5b6ec-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b6ec-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b6ec-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b6ec-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5b6ec-112">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5b6ec-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="5b6ec-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b6ec-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="5b6ec-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b6ec-114">Not supported.</span></span>|
|<span data-ttu-id="5b6ec-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="5b6ec-115">Application</span></span>| <span data-ttu-id="5b6ec-116">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5b6ec-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="5b6ec-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="5b6ec-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="5b6ec-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="5b6ec-118">Global administrator</span></span>
* <span data-ttu-id="5b6ec-119">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="5b6ec-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="5b6ec-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b6ec-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /b2cUserFlows/{id}/identityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="5b6ec-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b6ec-121">Request headers</span></span>

|<span data-ttu-id="5b6ec-122">Имя</span><span class="sxs-lookup"><span data-stu-id="5b6ec-122">Name</span></span>|<span data-ttu-id="5b6ec-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5b6ec-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="5b6ec-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b6ec-124">Authorization</span></span>|<span data-ttu-id="5b6ec-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b6ec-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5b6ec-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5b6ec-127">Content-Type</span></span>|<span data-ttu-id="5b6ec-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b6ec-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b6ec-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b6ec-130">Request body</span></span>

<span data-ttu-id="5b6ec-131">В тексте запроса укажите представление объекта IdentityProvider, который требуется добавить, в формате JSON `id` . [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="5b6ec-131">In the request body, provide a JSON representation of the `id` of the [identityProvider](../resources/identityprovider.md) you want to add.</span></span> <span data-ttu-id="5b6ec-132">Дополнительные сведения о поставщиках удостоверений, доступных для пользовательских потоков, представлены в справочнике по API [идентитипровидерс](../resources/identityprovider.md) .</span><span class="sxs-lookup"><span data-stu-id="5b6ec-132">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityprovider.md) API reference.</span></span>

## <a name="response"></a><span data-ttu-id="5b6ec-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b6ec-133">Response</span></span>

<span data-ttu-id="5b6ec-134">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5b6ec-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="5b6ec-135">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="5b6ec-135">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="5b6ec-136">Пример</span><span class="sxs-lookup"><span data-stu-id="5b6ec-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b6ec-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b6ec-137">Request</span></span>

<span data-ttu-id="5b6ec-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b6ec-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5b6ec-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b6ec-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_b2cuserflows_identityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/identityProviders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/identityProviders/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="5b6ec-140">C#</span><span class="sxs-lookup"><span data-stu-id="5b6ec-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-b2cuserflows-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5b6ec-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b6ec-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-b2cuserflows-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5b6ec-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b6ec-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-b2cuserflows-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5b6ec-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b6ec-143">Response</span></span>

<span data-ttu-id="5b6ec-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5b6ec-144">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
