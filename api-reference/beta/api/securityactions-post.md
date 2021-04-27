---
title: Создание объекта securityAction
description: Создайте новый объект securityAction".
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: f1d513ca1a24a1314be48f550be1ceae81282609
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049739"
---
# <a name="create-securityaction"></a><span data-ttu-id="21407-103">Создание объекта securityAction</span><span class="sxs-lookup"><span data-stu-id="21407-103">Create securityAction</span></span>

<span data-ttu-id="21407-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21407-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21407-105">Создание нового [объекта securityAction.](../resources/securityaction.md)</span><span class="sxs-lookup"><span data-stu-id="21407-105">Create a new [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="21407-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="21407-106">Permissions</span></span>

<span data-ttu-id="21407-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21407-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="21407-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21407-109">Permission type</span></span>                        | <span data-ttu-id="21407-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="21407-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="21407-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21407-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="21407-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21407-112">Not supported.</span></span> |
| <span data-ttu-id="21407-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21407-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21407-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21407-114">Not supported.</span></span> |
| <span data-ttu-id="21407-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="21407-115">Application</span></span>                            | <span data-ttu-id="21407-116">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21407-116">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="21407-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21407-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions
```

## <a name="request-headers"></a><span data-ttu-id="21407-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21407-118">Request headers</span></span>

| <span data-ttu-id="21407-119">Имя</span><span class="sxs-lookup"><span data-stu-id="21407-119">Name</span></span>          | <span data-ttu-id="21407-120">Описание</span><span class="sxs-lookup"><span data-stu-id="21407-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="21407-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="21407-121">Authorization</span></span> | <span data-ttu-id="21407-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="21407-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="21407-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="21407-123">Request body</span></span>

<span data-ttu-id="21407-124">В теле запроса поставляем представление JSON объекта [securityAction.](../resources/securityaction.md)</span><span class="sxs-lookup"><span data-stu-id="21407-124">In the request body, supply a JSON representation of a [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="21407-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="21407-125">Response</span></span>

<span data-ttu-id="21407-126">В случае успешной работы этот метод возвращает код ответа и объект `201 Created` [securityAction](../resources/securityaction.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="21407-126">If successful, this method returns `201 Created` response code and a [securityAction](../resources/securityaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="21407-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="21407-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="21407-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="21407-128">Request</span></span>

<span data-ttu-id="21407-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21407-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="21407-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="21407-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_securityaction_from_security"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions
Content-type: application/json

{
  "name": "BlockIp",
  "actionReason": "Test",
  "parameters": [
    {
      "name": "IP",
      "value": "1.2.3.4"
    }
  ],
  "vendorInformation": {
    "provider": "Windows Defender ATP",
    "vendor": "Microsoft"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="21407-131">C#</span><span class="sxs-lookup"><span data-stu-id="21407-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-securityaction-from-security-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21407-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21407-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-securityaction-from-security-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21407-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21407-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-securityaction-from-security-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="21407-134">Java</span><span class="sxs-lookup"><span data-stu-id="21407-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-securityaction-from-security-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="21407-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="21407-135">Response</span></span>

<span data-ttu-id="21407-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="21407-136">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="21407-137">Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="21407-137">The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securityAction"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id" : "1234567890",
    "status" : "notStarted",
    "createdDateTime": "2019-01-10 12:23:23.33333",
    "lastActionDateTime": "2019-01-10 12:23:23.33333",
    "name": "blockIp",
    "actionReason": "Test",
    "errorInfo": null,
    "vendorInformation": {
        "provider": "Windows Defender ATP",
        "providerVersion": null,
        "subProvider": null,
        "vendor": "Microsoft"
    },
    "parameters": [
        {
            "name": "IP",
            "value": "1.2.3.4"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create securityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


