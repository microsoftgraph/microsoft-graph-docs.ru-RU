---
title: Список Усерфловс
description: Получение списка объектов Усерфлов.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 32957546d058d9f7b6aafabd6d635de067266be4
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734673"
---
# <a name="list-userflows"></a><span data-ttu-id="4df0a-103">Список Усерфловс</span><span class="sxs-lookup"><span data-stu-id="4df0a-103">List userFlows</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4df0a-104">Получение списка [усерфловс](../resources/identityuserflow.md).</span><span class="sxs-lookup"><span data-stu-id="4df0a-104">Retrieve a list of [userflows](../resources/identityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4df0a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4df0a-105">Permissions</span></span>

<span data-ttu-id="4df0a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4df0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4df0a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4df0a-108">Permission type</span></span>                        | <span data-ttu-id="4df0a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4df0a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4df0a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4df0a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4df0a-111">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4df0a-111">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>  |
| <span data-ttu-id="4df0a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4df0a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4df0a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4df0a-113">Not supported.</span></span> |
| <span data-ttu-id="4df0a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4df0a-114">Application</span></span>                            | <span data-ttu-id="4df0a-115">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4df0a-115">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4df0a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4df0a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlows
```

## <a name="request-headers"></a><span data-ttu-id="4df0a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4df0a-117">Request headers</span></span>

| <span data-ttu-id="4df0a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4df0a-118">Name</span></span>      |<span data-ttu-id="4df0a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4df0a-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4df0a-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4df0a-120">Authorization</span></span> | <span data-ttu-id="4df0a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4df0a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4df0a-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4df0a-123">Request body</span></span>

<span data-ttu-id="4df0a-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4df0a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4df0a-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="4df0a-125">Response</span></span>

<span data-ttu-id="4df0a-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усерфлов](../resources/identityuserflow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4df0a-126">If successful, this method returns a `200 OK` response code and a collection of [userFlow](../resources/identityuserflow.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4df0a-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="4df0a-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4df0a-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="4df0a-128">Request</span></span>

<span data-ttu-id="4df0a-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4df0a-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_userflows"
}-->

```http
GET https://graph.microsoft.com/beta/identity/userFlows
```

### <a name="response"></a><span data-ttu-id="4df0a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="4df0a-130">Response</span></span>

<span data-ttu-id="4df0a-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4df0a-131">The following is an example of the response.</span></span>

> <span data-ttu-id="4df0a-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4df0a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.UserFlow",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "B2C_1_UserFlow1",
      "userFlowType": "signUpOrSignIn",
      "userFlowTypeVersion": 1
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List userFlows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: get_userflows/container/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->