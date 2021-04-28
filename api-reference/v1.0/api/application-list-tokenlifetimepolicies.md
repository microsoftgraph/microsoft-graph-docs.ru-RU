---
title: Список назначенного маркераLifetimePolicies
description: Список tokenLifetimePolicies, которые назначены приложению.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 68dac1d77011f0d82c9b786b64a2218a09a82535
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035934"
---
# <a name="list-assigned-tokenlifetimepolicy"></a><span data-ttu-id="7dec1-103">Список назначенного tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="7dec1-103">List assigned tokenLifetimePolicy</span></span>

<span data-ttu-id="7dec1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7dec1-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="7dec1-105">Список [объектов tokenLifetimePolicy,](../resources/tokenlifetimepolicy.md) которые назначены [приложению.](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="7dec1-105">List the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects that are assigned to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7dec1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7dec1-106">Permissions</span></span>

<span data-ttu-id="7dec1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dec1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7dec1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7dec1-109">Permission type</span></span>                        | <span data-ttu-id="7dec1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7dec1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7dec1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7dec1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7dec1-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dec1-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="7dec1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7dec1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7dec1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7dec1-114">Not supported.</span></span> |
| <span data-ttu-id="7dec1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7dec1-115">Application</span></span>                            | <span data-ttu-id="7dec1-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dec1-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7dec1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7dec1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="7dec1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7dec1-118">Request headers</span></span>

| <span data-ttu-id="7dec1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7dec1-119">Name</span></span>          | <span data-ttu-id="7dec1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7dec1-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7dec1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7dec1-121">Authorization</span></span> | <span data-ttu-id="7dec1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7dec1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7dec1-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7dec1-124">Request body</span></span>

<span data-ttu-id="7dec1-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7dec1-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7dec1-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dec1-126">Response</span></span>

<span data-ttu-id="7dec1-127">В случае успеха этот метод возвращает код отклика и коллекцию `200 OK` [объектов tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7dec1-127">If successful, this method returns a `200 OK` response code and a collection of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7dec1-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="7dec1-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7dec1-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="7dec1-129">Request</span></span>

<span data-ttu-id="7dec1-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7dec1-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7dec1-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="7dec1-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tokenlifetimepolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/{id}/tokenLifetimePolicies
```
# <a name="c"></a>[<span data-ttu-id="7dec1-132">C#</span><span class="sxs-lookup"><span data-stu-id="7dec1-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tokenlifetimepolicies-on-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7dec1-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7dec1-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tokenlifetimepolicies-on-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7dec1-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7dec1-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tokenlifetimepolicies-on-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7dec1-135">Java</span><span class="sxs-lookup"><span data-stu-id="7dec1-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tokenlifetimepolicies-on-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7dec1-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dec1-136">Response</span></span>

<span data-ttu-id="7dec1-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7dec1-137">The following is an example of the response.</span></span>

> <span data-ttu-id="7dec1-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7dec1-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List assigned tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

