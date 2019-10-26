---
title: Получение Усерфлов
description: Получение свойств и связей объекта усерфлов.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 820e4597b1616e5e34e567af6f09f7e620bec695
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734675"
---
# <a name="get-userflow"></a><span data-ttu-id="86f16-103">Получение Усерфлов</span><span class="sxs-lookup"><span data-stu-id="86f16-103">Get userFlow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86f16-104">Получение свойств и связей для объекта [усерфлов](../resources/identityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="86f16-104">Retrieve the properties and associations for an [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="86f16-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="86f16-105">Permissions</span></span>

<span data-ttu-id="86f16-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86f16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="86f16-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86f16-108">Permission type</span></span>                        | <span data-ttu-id="86f16-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="86f16-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="86f16-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86f16-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="86f16-111">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="86f16-111">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="86f16-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86f16-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86f16-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86f16-113">Not supported.</span></span> |
| <span data-ttu-id="86f16-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86f16-114">Application</span></span>                            | <span data-ttu-id="86f16-115">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="86f16-115">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="86f16-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86f16-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="86f16-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="86f16-117">Request headers</span></span>

| <span data-ttu-id="86f16-118">Имя</span><span class="sxs-lookup"><span data-stu-id="86f16-118">Name</span></span>      |<span data-ttu-id="86f16-119">Описание</span><span class="sxs-lookup"><span data-stu-id="86f16-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="86f16-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="86f16-120">Authorization</span></span> | <span data-ttu-id="86f16-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86f16-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="86f16-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="86f16-123">Content-type</span></span> | <span data-ttu-id="86f16-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86f16-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="86f16-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="86f16-126">Request body</span></span>

<span data-ttu-id="86f16-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="86f16-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86f16-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="86f16-128">Response</span></span>

<span data-ttu-id="86f16-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [усерфлов](../resources/identityuserflow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="86f16-129">If successful, this method returns a `200 OK` response code and the requested [userFlow](../resources/identityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="86f16-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="86f16-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="86f16-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="86f16-131">Request</span></span>

<span data-ttu-id="86f16-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86f16-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityuserflow"
}-->

```http
GET https://graph.microsoft.com/beta/identity/userFlows/B2C_1_Pol1
```

### <a name="response"></a><span data-ttu-id="86f16-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="86f16-133">Response</span></span>

<span data-ttu-id="86f16-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="86f16-134">The following is an example of the response.</span></span>

> <span data-ttu-id="86f16-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="86f16-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.UserFlow"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "B2C_1_Pol1",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get UserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
   "suppressions": [
    "Error: get_identityuserflow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
