---
title: Список legalHolds
description: Получите ресурсы legalHold из свойства навигации LegalHolds.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: eee7497c355743fb650192b5ae5842a273cf18d9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776692"
---
# <a name="list-legalholds"></a><span data-ttu-id="3a4d0-103">Список legalHolds</span><span class="sxs-lookup"><span data-stu-id="3a4d0-103">List legalHolds</span></span>

<span data-ttu-id="3a4d0-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="3a4d0-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a4d0-105">Получите [legalHolds,](../resources/ediscovery-legalhold.md) которые применяются к делу.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-105">Get the [legalHolds](../resources/ediscovery-legalhold.md) that are applied to a case.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a4d0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a4d0-106">Permissions</span></span>

<span data-ttu-id="3a4d0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a4d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a4d0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a4d0-109">Permission type</span></span>|<span data-ttu-id="3a4d0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a4d0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a4d0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a4d0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3a4d0-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a4d0-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="3a4d0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a4d0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a4d0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-114">Not supported.</span></span>|
|<span data-ttu-id="3a4d0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a4d0-115">Application</span></span>|<span data-ttu-id="3a4d0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a4d0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a4d0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/legalHolds
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3a4d0-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3a4d0-118">Optional query parameters</span></span>

<span data-ttu-id="3a4d0-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3a4d0-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3a4d0-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a4d0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a4d0-121">Request headers</span></span>

|<span data-ttu-id="3a4d0-122">Имя</span><span class="sxs-lookup"><span data-stu-id="3a4d0-122">Name</span></span>|<span data-ttu-id="3a4d0-123">Описание</span><span class="sxs-lookup"><span data-stu-id="3a4d0-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3a4d0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a4d0-124">Authorization</span></span>|<span data-ttu-id="3a4d0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a4d0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a4d0-127">Request body</span></span>

<span data-ttu-id="3a4d0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a4d0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a4d0-129">Response</span></span>

<span data-ttu-id="3a4d0-130">В случае успешной работы этот метод возвращает код ответа и коллекцию `200 OK` [объектов legalHold](../resources/ediscovery-legalhold.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-130">If successful, this method returns a `200 OK` response code and a collection of [legalHold](../resources/ediscovery-legalhold.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3a4d0-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="3a4d0-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3a4d0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a4d0-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3a4d0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a4d0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_legalhold"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/legalHolds
```
# <a name="c"></a>[<span data-ttu-id="3a4d0-134">C#</span><span class="sxs-lookup"><span data-stu-id="3a4d0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-legalhold-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a4d0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a4d0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-legalhold-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a4d0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a4d0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-legalhold-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a4d0-137">Java</span><span class="sxs-lookup"><span data-stu-id="3a4d0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-legalhold-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3a4d0-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a4d0-138">Response</span></span>

<span data-ttu-id="3a4d0-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.legalHold)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ediscovery.legalHold",
      "id": "700cd868-d868-700c-68d8-0c7068d80c70",
      "description": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "lastModifiedDateTime": "String (timestamp)",
      "isEnabled": "Boolean",
      "status": "String",
      "contentQuery": "String",
      "errors": [
        "String"
      ],
      "displayName": "String",
      "createdDateTime": "String (timestamp)"
    }
  ]
}
```
