---
title: Создание Воркфорцеинтегратион
description: Создание нового объекта Воркфорцеинтегратион.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b818b55d95485ca17aff581f8b986f3fbb01465d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451275"
---
# <a name="create-workforceintegration"></a><span data-ttu-id="8e63d-103">Создание Воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="8e63d-103">Create workforceIntegration</span></span>

<span data-ttu-id="8e63d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e63d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e63d-105">Создание нового объекта [воркфорцеинтегратион](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="8e63d-105">Create a new [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e63d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e63d-106">Permissions</span></span>

<span data-ttu-id="8e63d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e63d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8e63d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e63d-109">Permission type</span></span>                        | <span data-ttu-id="8e63d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e63d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8e63d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e63d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8e63d-112">Воркфорцеинтегратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8e63d-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="8e63d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e63d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e63d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e63d-114">Not supported.</span></span> |
| <span data-ttu-id="8e63d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e63d-115">Application</span></span>                            | <span data-ttu-id="8e63d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e63d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e63d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e63d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="8e63d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e63d-118">Request headers</span></span>

| <span data-ttu-id="8e63d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8e63d-119">Name</span></span>          | <span data-ttu-id="8e63d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8e63d-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8e63d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e63d-121">Authorization</span></span> | <span data-ttu-id="8e63d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e63d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8e63d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8e63d-124">Content-type</span></span> | <span data-ttu-id="8e63d-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e63d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e63d-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e63d-127">Request body</span></span>

<span data-ttu-id="8e63d-128">В тексте запроса добавьте представление объекта [воркфорцеинтегратион](../resources/workforceintegration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e63d-128">In the request body, supply a JSON representation of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8e63d-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="8e63d-129">Response</span></span>

<span data-ttu-id="8e63d-130">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [воркфорцеинтегратион](../resources/workforceintegration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8e63d-130">If successful, this method returns a `201 Created` response code and a new [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8e63d-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="8e63d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8e63d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e63d-132">Request</span></span>

<span data-ttu-id="8e63d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e63d-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8e63d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e63d-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8e63d-135">C#</span><span class="sxs-lookup"><span data-stu-id="8e63d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-workforceintegration-from-teamwork-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e63d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e63d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-workforceintegration-from-teamwork-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e63d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e63d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-workforceintegration-from-teamwork-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8e63d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e63d-138">Response</span></span>

<span data-ttu-id="8e63d-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8e63d-139">The following is an example of the response.</span></span>

> <span data-ttu-id="8e63d-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e63d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
