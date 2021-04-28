---
title: Получить accessReviewPolicy
description: Ознакомьтесь с свойствами и отношениями объекта accessReviewPolicy.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 05b6cbae21ea3a40b179d646feaeb9ff243f0a81
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068058"
---
# <a name="get-accessreviewpolicy"></a><span data-ttu-id="fab52-103">Получить accessReviewPolicy</span><span class="sxs-lookup"><span data-stu-id="fab52-103">Get accessReviewPolicy</span></span>
<span data-ttu-id="fab52-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fab52-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fab52-105">Ознакомьтесь с свойствами и отношениями [объекта accessReviewPolicy.](../resources/accessreviewpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fab52-105">Read the properties and relationships of an [accessReviewPolicy](../resources/accessreviewpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fab52-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fab52-106">Permissions</span></span>
<span data-ttu-id="fab52-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fab52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fab52-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fab52-109">Permission type</span></span>|<span data-ttu-id="fab52-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fab52-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fab52-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fab52-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fab52-112">Policy.Read.All, Policy.ReadWrite.AccessReviews</span><span class="sxs-lookup"><span data-stu-id="fab52-112">Policy.Read.All, Policy.ReadWrite.AccessReviews</span></span>|
|<span data-ttu-id="fab52-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fab52-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fab52-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fab52-114">Not supported.</span></span>|
|<span data-ttu-id="fab52-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fab52-115">Application</span></span>|<span data-ttu-id="fab52-116">Policy.Read.All, Policy.ReadWrite.AccessReviews</span><span class="sxs-lookup"><span data-stu-id="fab52-116">Policy.Read.All, Policy.ReadWrite.AccessReviews</span></span>|

## <a name="http-request"></a><span data-ttu-id="fab52-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fab52-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/accessReviewPolicy
GET /identityGovernance/accessReviews/policy
```

## <a name="request-headers"></a><span data-ttu-id="fab52-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fab52-118">Request headers</span></span>
|<span data-ttu-id="fab52-119">Имя</span><span class="sxs-lookup"><span data-stu-id="fab52-119">Name</span></span>|<span data-ttu-id="fab52-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fab52-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fab52-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fab52-121">Authorization</span></span>|<span data-ttu-id="fab52-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fab52-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fab52-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fab52-124">Request body</span></span>
<span data-ttu-id="fab52-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fab52-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fab52-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="fab52-126">Response</span></span>

<span data-ttu-id="fab52-127">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект accessReviewPolicy](../resources/accessreviewpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fab52-127">If successful, this method returns a `200 OK` response code and an [accessReviewPolicy](../resources/accessreviewpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fab52-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="fab52-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fab52-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="fab52-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accessreviewpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/accessReviewPolicy
```


### <a name="response"></a><span data-ttu-id="fab52-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="fab52-130">Response</span></span>
<span data-ttu-id="fab52-131">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fab52-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.accessReviewPolicy",
    "displayName": "Access Review Policy",
    "description": "Policy contains directory-level access review settings.",
    "isGroupOwnerManagementEnabled": false
  }
}
```

### <a name="request"></a><span data-ttu-id="fab52-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fab52-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accessreviewpolicy_2"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/policy
```


### <a name="response"></a><span data-ttu-id="fab52-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="fab52-133">Response</span></span>
<span data-ttu-id="fab52-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fab52-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.accessReviewPolicy",
    "displayName": "Access Review Policy",
    "description": "Policy contains directory-level access review settings.",
    "isGroupOwnerManagementEnabled": false
  }
}
```
