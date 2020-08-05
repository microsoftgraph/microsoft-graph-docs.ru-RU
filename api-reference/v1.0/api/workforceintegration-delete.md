---
title: Удаление Воркфорцеинтегратион
description: Удаление экземпляра объекта Воркфорцеинтегратион.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b3c3b0c33c617ba03b56a53e1ebb4be9c51bcaa2
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/04/2020
ms.locfileid: "44217303"
---
# <a name="delete-workforceintegration"></a><span data-ttu-id="8598e-103">Удаление Воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="8598e-103">Delete workforceIntegration</span></span>

<span data-ttu-id="8598e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8598e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8598e-105">Удаление экземпляра объекта [воркфорцеинтегратион](../resources/workforceintegration.md).</span><span class="sxs-lookup"><span data-stu-id="8598e-105">Delete an instance of a [workforceIntegration](../resources/workforceintegration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8598e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8598e-106">Permissions</span></span>

<span data-ttu-id="8598e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8598e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8598e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8598e-109">Permission type</span></span>                        | <span data-ttu-id="8598e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8598e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8598e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8598e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8598e-112">Воркфорцеинтегратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8598e-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="8598e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8598e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8598e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8598e-114">Not supported.</span></span> |
| <span data-ttu-id="8598e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8598e-115">Application</span></span>                            | <span data-ttu-id="8598e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8598e-116">Not supported.</span></span> |

> <span data-ttu-id="8598e-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="8598e-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8598e-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="8598e-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8598e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8598e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="request-headers"></a><span data-ttu-id="8598e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8598e-120">Request headers</span></span>

| <span data-ttu-id="8598e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="8598e-121">Name</span></span>          | <span data-ttu-id="8598e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8598e-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8598e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8598e-123">Authorization</span></span> | <span data-ttu-id="8598e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8598e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8598e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8598e-126">Request body</span></span>

<span data-ttu-id="8598e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8598e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8598e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8598e-128">Response</span></span>

<span data-ttu-id="8598e-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8598e-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8598e-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="8598e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8598e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8598e-132">Request</span></span>

<span data-ttu-id="8598e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8598e-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8598e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8598e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_workforceintegration"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations/{workforceIntegrationId}
```
# <a name="c"></a>[<span data-ttu-id="8598e-135">C#</span><span class="sxs-lookup"><span data-stu-id="8598e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8598e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8598e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8598e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8598e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8598e-138">Java</span><span class="sxs-lookup"><span data-stu-id="8598e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-workforceintegration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="8598e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="8598e-139">Response</span></span>

<span data-ttu-id="8598e-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8598e-140">The following is an example of the response.</span></span>

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
