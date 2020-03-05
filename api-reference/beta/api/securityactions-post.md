---
title: Создание объекта securityAction
description: Создайте новый объект securityAction. "
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 3ea1d95e1ff9380919d3d4afd2877cab2e370eae
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453550"
---
# <a name="create-securityaction"></a><span data-ttu-id="7b902-103">Создание объекта securityAction</span><span class="sxs-lookup"><span data-stu-id="7b902-103">Create securityAction</span></span>

<span data-ttu-id="7b902-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7b902-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b902-105">Создайте новый объект [securityAction](../resources/securityaction.md) .</span><span class="sxs-lookup"><span data-stu-id="7b902-105">Create a new [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b902-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b902-106">Permissions</span></span>

<span data-ttu-id="7b902-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b902-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7b902-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b902-109">Permission type</span></span>                        | <span data-ttu-id="7b902-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b902-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7b902-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b902-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7b902-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b902-112">Not supported.</span></span> |
| <span data-ttu-id="7b902-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b902-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b902-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b902-114">Not supported.</span></span> |
| <span data-ttu-id="7b902-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b902-115">Application</span></span>                            | <span data-ttu-id="7b902-116">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b902-116">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b902-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b902-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions
```

## <a name="request-headers"></a><span data-ttu-id="7b902-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b902-118">Request headers</span></span>

| <span data-ttu-id="7b902-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7b902-119">Name</span></span>          | <span data-ttu-id="7b902-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7b902-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7b902-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b902-121">Authorization</span></span> | <span data-ttu-id="7b902-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="7b902-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b902-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7b902-123">Request body</span></span>

<span data-ttu-id="7b902-124">В тексте запроса добавьте представление объекта [securityAction](../resources/securityaction.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b902-124">In the request body, supply a JSON representation of a [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7b902-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b902-125">Response</span></span>

<span data-ttu-id="7b902-126">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [securityAction](../resources/securityaction.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7b902-126">If successful, this method returns `201 Created` response code and a [securityAction](../resources/securityaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7b902-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="7b902-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7b902-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b902-128">Request</span></span>

<span data-ttu-id="7b902-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b902-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7b902-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b902-130">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7b902-131">C#</span><span class="sxs-lookup"><span data-stu-id="7b902-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-securityaction-from-security-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7b902-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b902-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-securityaction-from-security-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7b902-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b902-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-securityaction-from-security-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7b902-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b902-134">Response</span></span>

<span data-ttu-id="7b902-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7b902-135">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="7b902-136">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7b902-136">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7b902-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7b902-137">All the properties will be returned from an actual call.</span></span>

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
