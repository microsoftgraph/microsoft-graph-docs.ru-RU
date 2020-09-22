---
title: Получение Континуаусакцессевалуатионполици
description: Чтение свойств объекта Континуаусакцессевалуатионполици.
author: jerrysai
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bea54ea801ee9d41314f1fbd2c87070ac4e92773
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023541"
---
# <a name="get-continuousaccessevaluationpolicy"></a><span data-ttu-id="d54a7-103">Получение Континуаусакцессевалуатионполици</span><span class="sxs-lookup"><span data-stu-id="d54a7-103">Get continuousAccessEvaluationPolicy</span></span>
<span data-ttu-id="d54a7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d54a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d54a7-105">Чтение свойств и связей объекта [континуаусакцессевалуатионполици](../resources/continuousaccessevaluationpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="d54a7-105">Read the properties and relationships of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d54a7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d54a7-106">Permissions</span></span>
<span data-ttu-id="d54a7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d54a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d54a7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d54a7-109">Permission type</span></span>|<span data-ttu-id="d54a7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d54a7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d54a7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d54a7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d54a7-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="d54a7-112">Policy.Read.All</span></span> |
|<span data-ttu-id="d54a7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d54a7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d54a7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d54a7-114">Not supported.</span></span> |
|<span data-ttu-id="d54a7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d54a7-115">Application</span></span>                            | <span data-ttu-id="d54a7-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="d54a7-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d54a7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d54a7-117">HTTP request</span></span>

<!-- {  "blockType": "ignored"} -->
``` http
GET /identity/continuousAccessEvaluationPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d54a7-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d54a7-118">Optional query parameters</span></span>
<span data-ttu-id="d54a7-119">Этот метод поддерживает параметр запроса OData "$select" для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d54a7-119">This method supports the '$select' OData query parameter to help customize the response.</span></span> <span data-ttu-id="d54a7-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d54a7-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d54a7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d54a7-121">Request headers</span></span>
|<span data-ttu-id="d54a7-122">Имя</span><span class="sxs-lookup"><span data-stu-id="d54a7-122">Name</span></span>|<span data-ttu-id="d54a7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d54a7-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d54a7-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d54a7-124">Authorization</span></span>|<span data-ttu-id="d54a7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d54a7-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d54a7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d54a7-127">Request body</span></span>
<span data-ttu-id="d54a7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d54a7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d54a7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d54a7-129">Response</span></span>

<span data-ttu-id="d54a7-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [континуаусакцессевалуатионполици](../resources/continuousaccessevaluationpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d54a7-130">If successful, this method returns a `200 OK` response code and a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d54a7-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="d54a7-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d54a7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d54a7-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_continuousaccessevaluationpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/identity/continuousAccessEvaluationPolicy
```


### <a name="response"></a><span data-ttu-id="d54a7-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d54a7-133">Response</span></span>

<span data-ttu-id="d54a7-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d54a7-134">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.continuousAccessEvaluationPolicy"
} -->

``` http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/continuousAccessEvaluationPolicy/$entity",
  "id": "00000000-0000-0000-0000-000000000006",
  "description": "Continuous Access Evaluation automatically blocks access to resources and applications in near real time when a user's access is removed or a client IP address changes.",
  "displayName": "Continuous Access Evaluation",
  "isEnabled": true,
  "users": [ "1608be63-df14-42a4-8932-1c9d963b026f" ],
  "groups": [ "4308b567-df14-0000-8932-1c9d963b026f" ]
}
```
