---
title: Создание Воркфорцеинтегратион
description: Создание нового объекта Воркфорцеинтегратион.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6066005ff12e2cfa3513f1548b4e3895eb38f993
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870606"
---
# <a name="create-workforceintegration"></a><span data-ttu-id="3f581-103">Создание Воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="3f581-103">Create workforceIntegration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f581-104">Создание нового объекта [воркфорцеинтегратион](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="3f581-104">Create a new [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f581-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3f581-105">Permissions</span></span>

<span data-ttu-id="3f581-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f581-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3f581-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f581-108">Permission type</span></span>                        | <span data-ttu-id="3f581-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f581-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3f581-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f581-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3f581-111">Воркфорцеинтегратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3f581-111">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="3f581-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f581-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f581-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f581-113">Not supported.</span></span> |
| <span data-ttu-id="3f581-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3f581-114">Application</span></span>                            | <span data-ttu-id="3f581-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f581-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f581-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f581-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="3f581-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3f581-117">Request headers</span></span>

| <span data-ttu-id="3f581-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3f581-118">Name</span></span>          | <span data-ttu-id="3f581-119">Описание</span><span class="sxs-lookup"><span data-stu-id="3f581-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3f581-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3f581-120">Authorization</span></span> | <span data-ttu-id="3f581-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f581-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3f581-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3f581-123">Content-type</span></span> | <span data-ttu-id="3f581-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f581-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f581-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3f581-126">Request body</span></span>

<span data-ttu-id="3f581-127">В тексте запроса добавьте представление объекта [воркфорцеинтегратион](../resources/workforceintegration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f581-127">In the request body, supply a JSON representation of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3f581-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="3f581-128">Response</span></span>

<span data-ttu-id="3f581-129">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [воркфорцеинтегратион](../resources/workforceintegration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3f581-129">If successful, this method returns a `201 Created` response code and a new [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3f581-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="3f581-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3f581-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f581-131">Request</span></span>

<span data-ttu-id="3f581-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f581-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3f581-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f581-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_workforceintegration_from_teamwork"
}-->

```http
POST https://graph.microsoft.com/beta/teamwork/workforceIntegrations
Content-type: application/json

{
  "displayName": "displayName-value",
  "apiVersion": 99,
  "encryption": {
    "protocol": "protocol-value",
    "secret": "secret-value"
  },
  "isActive": true,
  "url": "url-value",
  "supports": "supports-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3f581-134">C#</span><span class="sxs-lookup"><span data-stu-id="3f581-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-workforceintegration-from-teamwork-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3f581-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f581-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-workforceintegration-from-teamwork-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3f581-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f581-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-workforceintegration-from-teamwork-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3f581-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f581-137">Response</span></span>

<span data-ttu-id="3f581-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3f581-138">The following is an example of the response.</span></span>

> <span data-ttu-id="3f581-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3f581-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "displayName": "displayName-value",
  "apiVersion": 99,
  "encryption": {
    "protocol": "protocol-value",
    "secret": "secret-value"
  },
  "isActive": true,
  "url": "url-value",
  "supports": "supports-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create workforceIntegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
