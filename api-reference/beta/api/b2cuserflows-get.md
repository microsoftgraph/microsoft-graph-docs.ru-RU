---
title: Получение b2cUserFlows
description: Получение свойств и связей объекта b2cUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ea558ddd1f8146b33eb5b153dfc0fcb73b21d6b1
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319817"
---
# <a name="get-b2cuserflow"></a><span data-ttu-id="267dd-103">Получение b2cUserFlow</span><span class="sxs-lookup"><span data-stu-id="267dd-103">Get b2cUserFlow</span></span>

<span data-ttu-id="267dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="267dd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="267dd-105">Получение свойств и связей объекта [b2cUserFlow](../resources/b2cuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="267dd-105">Retrieve the properties and relationships of a [b2cUserFlow](../resources/b2cuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="267dd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="267dd-106">Permissions</span></span>

<span data-ttu-id="267dd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="267dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="267dd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="267dd-109">Permission type</span></span>      | <span data-ttu-id="267dd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="267dd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="267dd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="267dd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="267dd-112">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="267dd-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="267dd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="267dd-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="267dd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="267dd-114">Not supported.</span></span>|
|<span data-ttu-id="267dd-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="267dd-115">Application</span></span>|<span data-ttu-id="267dd-116">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="267dd-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="267dd-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="267dd-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="267dd-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="267dd-118">Global administrator</span></span>
* <span data-ttu-id="267dd-119">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="267dd-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="267dd-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="267dd-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2cUserFlows/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="267dd-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="267dd-121">Optional query parameters</span></span>

<span data-ttu-id="267dd-122">Можно использовать `$expand` для расширения определенных свойств пользовательского пользовательского процесса, которые по умолчанию не развернуты.</span><span class="sxs-lookup"><span data-stu-id="267dd-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span>

<span data-ttu-id="267dd-123">Дополнительные сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="267dd-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="267dd-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="267dd-124">Request headers</span></span>

|<span data-ttu-id="267dd-125">Имя</span><span class="sxs-lookup"><span data-stu-id="267dd-125">Name</span></span>|<span data-ttu-id="267dd-126">Описание</span><span class="sxs-lookup"><span data-stu-id="267dd-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="267dd-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="267dd-127">Authorization</span></span>|<span data-ttu-id="267dd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="267dd-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="267dd-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="267dd-130">Request body</span></span>

<span data-ttu-id="267dd-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="267dd-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="267dd-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="267dd-132">Response</span></span>

<span data-ttu-id="267dd-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и представление объекта [b2cUserFlow](../resources/b2cuserflows.md) в тексте отклика в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="267dd-133">If successful, this method returns a `200 OK` response code and a JSON representation of the [b2cUserFlow](../resources/b2cuserflows.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="267dd-134">Пример</span><span class="sxs-lookup"><span data-stu-id="267dd-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="267dd-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="267dd-135">Request</span></span>

<span data-ttu-id="267dd-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="267dd-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2cUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}
```

### <a name="response"></a><span data-ttu-id="267dd-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="267dd-137">Response</span></span>

<span data-ttu-id="267dd-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="267dd-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "B2C_1_CustomerSignUp",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Get b2cUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: get_b2cUserFlows/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
