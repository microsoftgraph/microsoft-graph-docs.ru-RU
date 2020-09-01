---
title: Получение b2xUserFlows
description: Получение свойств и связей объекта b2xUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 50089ec092dfe9802c97d253f872e47470d2f0f6
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319804"
---
# <a name="get-b2xuserflow"></a><span data-ttu-id="ccc87-103">Получение b2xUserFlow</span><span class="sxs-lookup"><span data-stu-id="ccc87-103">Get b2xUserFlow</span></span>

<span data-ttu-id="ccc87-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccc87-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccc87-105">Получение свойств и связей объекта [b2xUserFlow](../resources/b2xuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="ccc87-105">Retrieve the properties and relationships of a [b2xUserFlow](../resources/b2xuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ccc87-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ccc87-106">Permissions</span></span>

<span data-ttu-id="ccc87-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccc87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccc87-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccc87-109">Permission type</span></span>      | <span data-ttu-id="ccc87-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccc87-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccc87-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccc87-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ccc87-112">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ccc87-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="ccc87-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccc87-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ccc87-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccc87-114">Not supported.</span></span>|
|<span data-ttu-id="ccc87-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="ccc87-115">Application</span></span>|<span data-ttu-id="ccc87-116">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ccc87-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="ccc87-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="ccc87-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="ccc87-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ccc87-118">Global administrator</span></span>
* <span data-ttu-id="ccc87-119">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="ccc87-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="ccc87-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ccc87-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ccc87-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ccc87-121">Optional query parameters</span></span>

<span data-ttu-id="ccc87-122">Можно использовать `$expand` для расширения определенных свойств пользовательского пользовательского процесса, которые по умолчанию не развернуты.</span><span class="sxs-lookup"><span data-stu-id="ccc87-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span>

<span data-ttu-id="ccc87-123">Дополнительные сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ccc87-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ccc87-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ccc87-124">Request headers</span></span>

|<span data-ttu-id="ccc87-125">Имя</span><span class="sxs-lookup"><span data-stu-id="ccc87-125">Name</span></span>|<span data-ttu-id="ccc87-126">Описание</span><span class="sxs-lookup"><span data-stu-id="ccc87-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="ccc87-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ccc87-127">Authorization</span></span>|<span data-ttu-id="ccc87-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ccc87-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccc87-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ccc87-130">Request body</span></span>

<span data-ttu-id="ccc87-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ccc87-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ccc87-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccc87-132">Response</span></span>

<span data-ttu-id="ccc87-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и представление объекта [усерфловаттрибуте](../resources/b2xuserflows.md) в тексте отклика в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ccc87-133">If successful, this method returns a `200 OK` response code and a JSON representation of the [userFlowAttribute](../resources/b2xuserflows.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccc87-134">Пример</span><span class="sxs-lookup"><span data-stu-id="ccc87-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="ccc87-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccc87-135">Request</span></span>

<span data-ttu-id="ccc87-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ccc87-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}
```

### <a name="response"></a><span data-ttu-id="ccc87-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccc87-137">Response</span></span>

<span data-ttu-id="ccc87-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ccc87-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "B2X_1_PartnerSignUp",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Get b2xUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: get_b2xUserFlows/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
