---
title: Удаление Воркфорцеинтегратион
description: Удаление экземпляра объекта Воркфорцеинтегратион.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6d13f2ba5a67d56547daa05e3595d155a260fbb2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967746"
---
# <a name="delete-workforceintegration"></a><span data-ttu-id="f7ad1-103">Удаление Воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="f7ad1-103">Delete workforceIntegration</span></span>

<span data-ttu-id="f7ad1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7ad1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f7ad1-105">Удаление экземпляра объекта [воркфорцеинтегратион](../resources/workforceintegration.md).</span><span class="sxs-lookup"><span data-stu-id="f7ad1-105">Delete an instance of a [workforceIntegration](../resources/workforceintegration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f7ad1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7ad1-106">Permissions</span></span>

<span data-ttu-id="f7ad1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7ad1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f7ad1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7ad1-109">Permission type</span></span>                        | <span data-ttu-id="f7ad1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7ad1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f7ad1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7ad1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f7ad1-112">Воркфорцеинтегратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f7ad1-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="f7ad1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7ad1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7ad1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7ad1-114">Not supported.</span></span> |
| <span data-ttu-id="f7ad1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7ad1-115">Application</span></span>                            | <span data-ttu-id="f7ad1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7ad1-116">Not supported.</span></span> |

> <span data-ttu-id="f7ad1-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="f7ad1-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f7ad1-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="f7ad1-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f7ad1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7ad1-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="request-headers"></a><span data-ttu-id="f7ad1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7ad1-120">Request headers</span></span>

| <span data-ttu-id="f7ad1-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f7ad1-121">Name</span></span>          | <span data-ttu-id="f7ad1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f7ad1-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f7ad1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7ad1-123">Authorization</span></span> | <span data-ttu-id="f7ad1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7ad1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7ad1-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f7ad1-126">Request body</span></span>

<span data-ttu-id="f7ad1-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f7ad1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7ad1-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7ad1-128">Response</span></span>

<span data-ttu-id="f7ad1-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f7ad1-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f7ad1-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="f7ad1-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f7ad1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7ad1-132">Request</span></span>

<span data-ttu-id="f7ad1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7ad1-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f7ad1-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7ad1-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_workforceintegration"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations/{workforceIntegrationId}
```
# <a name="c"></a>[<span data-ttu-id="f7ad1-135">C#</span><span class="sxs-lookup"><span data-stu-id="f7ad1-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7ad1-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7ad1-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7ad1-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7ad1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7ad1-138">Java</span><span class="sxs-lookup"><span data-stu-id="f7ad1-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-workforceintegration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="f7ad1-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7ad1-139">Response</span></span>

<span data-ttu-id="f7ad1-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f7ad1-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete workforceIntegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

