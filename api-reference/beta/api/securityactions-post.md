---
title: Создание объекта securityAction
description: Создайте новый объект securityAction. "
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 155e7a3155179cc82e6e065f51a966f739ea344b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977979"
---
# <a name="create-securityaction"></a><span data-ttu-id="4f689-103">Создание объекта securityAction</span><span class="sxs-lookup"><span data-stu-id="4f689-103">Create securityAction</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f689-104">Создайте новый объект [securityAction](../resources/securityaction.md) .</span><span class="sxs-lookup"><span data-stu-id="4f689-104">Create a new [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f689-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4f689-105">Permissions</span></span>

<span data-ttu-id="4f689-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f689-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4f689-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f689-108">Permission type</span></span>                        | <span data-ttu-id="4f689-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f689-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4f689-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f689-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f689-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f689-111">Not supported.</span></span> |
| <span data-ttu-id="4f689-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f689-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f689-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f689-113">Not supported.</span></span> |
| <span data-ttu-id="4f689-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f689-114">Application</span></span>                            | <span data-ttu-id="4f689-115">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f689-115">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f689-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f689-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions
```

## <a name="request-headers"></a><span data-ttu-id="4f689-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f689-117">Request headers</span></span>

| <span data-ttu-id="4f689-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4f689-118">Name</span></span>          | <span data-ttu-id="4f689-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4f689-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4f689-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f689-120">Authorization</span></span> | <span data-ttu-id="4f689-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4f689-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f689-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f689-122">Request body</span></span>

<span data-ttu-id="4f689-123">В тексте запроса добавьте представление объекта [securityAction](../resources/securityaction.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f689-123">In the request body, supply a JSON representation of a [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4f689-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f689-124">Response</span></span>

<span data-ttu-id="4f689-125">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [securityAction](../resources/securityaction.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4f689-125">If successful, this method returns `201 Created` response code and a [securityAction](../resources/securityaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4f689-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="4f689-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4f689-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f689-127">Request</span></span>

<span data-ttu-id="4f689-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f689-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4f689-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f689-129">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="4f689-130">C#</span><span class="sxs-lookup"><span data-stu-id="4f689-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-securityaction-from-security-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4f689-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="4f689-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-securityaction-from-security-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4f689-132">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4f689-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-securityaction-from-security-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4f689-133">Java</span><span class="sxs-lookup"><span data-stu-id="4f689-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-securityaction-from-security-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4f689-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f689-134">Response</span></span>

<span data-ttu-id="4f689-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4f689-135">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="4f689-136">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4f689-136">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4f689-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f689-137">All the properties will be returned from an actual call.</span></span>

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
