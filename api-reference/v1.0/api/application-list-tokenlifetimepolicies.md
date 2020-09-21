---
title: Список назначенных ТокенлифетимеполиЦиес
description: Список ТокенлифетимеполиЦиес, назначенных приложению.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 17b6502323b62603c119fa04137d46b0ffef770c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966445"
---
# <a name="list-assigned-tokenlifetimepolicy"></a><span data-ttu-id="75c1d-103">Список назначенных Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="75c1d-103">List assigned tokenLifetimePolicy</span></span>

<span data-ttu-id="75c1d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75c1d-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="75c1d-105">Перечисление объектов [токенлифетимеполици](../resources/tokenlifetimepolicy.md) , назначенных [приложению](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="75c1d-105">List the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects that are assigned to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="75c1d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75c1d-106">Permissions</span></span>

<span data-ttu-id="75c1d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75c1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="75c1d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75c1d-109">Permission type</span></span>                        | <span data-ttu-id="75c1d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75c1d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="75c1d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75c1d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="75c1d-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="75c1d-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="75c1d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75c1d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75c1d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75c1d-114">Not supported.</span></span> |
| <span data-ttu-id="75c1d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75c1d-115">Application</span></span>                            | <span data-ttu-id="75c1d-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="75c1d-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="75c1d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75c1d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="75c1d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75c1d-118">Request headers</span></span>

| <span data-ttu-id="75c1d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="75c1d-119">Name</span></span>          | <span data-ttu-id="75c1d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="75c1d-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="75c1d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75c1d-121">Authorization</span></span> | <span data-ttu-id="75c1d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75c1d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75c1d-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="75c1d-124">Request body</span></span>

<span data-ttu-id="75c1d-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75c1d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75c1d-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="75c1d-126">Response</span></span>

<span data-ttu-id="75c1d-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [токенлифетимеполици](../resources/tokenlifetimepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="75c1d-127">If successful, this method returns a `200 OK` response code and a collection of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="75c1d-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="75c1d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="75c1d-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="75c1d-129">Request</span></span>

<span data-ttu-id="75c1d-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75c1d-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="75c1d-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="75c1d-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tokenlifetimepolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/{id}/tokenLifetimePolicies
```
# <a name="c"></a>[<span data-ttu-id="75c1d-132">C#</span><span class="sxs-lookup"><span data-stu-id="75c1d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tokenlifetimepolicies-on-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75c1d-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75c1d-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tokenlifetimepolicies-on-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75c1d-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75c1d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tokenlifetimepolicies-on-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="75c1d-135">Java</span><span class="sxs-lookup"><span data-stu-id="75c1d-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tokenlifetimepolicies-on-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="75c1d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="75c1d-136">Response</span></span>

<span data-ttu-id="75c1d-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="75c1d-137">The following is an example of the response.</span></span>

> <span data-ttu-id="75c1d-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75c1d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

