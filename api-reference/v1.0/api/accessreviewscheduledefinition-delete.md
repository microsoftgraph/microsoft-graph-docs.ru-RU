---
title: Удаление accessReviewScheduleDefinition
description: Удаляет объект accessReviewScheduleDefinition.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 697a762ec6234d14d55dfc7f345299dc071af2f1
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031280"
---
# <a name="delete-accessreviewscheduledefinition"></a><span data-ttu-id="39679-103">Удаление accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="39679-103">Delete accessReviewScheduleDefinition</span></span>
<span data-ttu-id="39679-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39679-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="39679-105">Удаляет объект [accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="39679-105">Deletes an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="39679-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="39679-106">Permissions</span></span>
<span data-ttu-id="39679-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39679-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39679-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39679-109">Permission type</span></span>|<span data-ttu-id="39679-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39679-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39679-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39679-111">Delegated (work or school account)</span></span>| <span data-ttu-id="39679-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39679-112">AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="39679-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39679-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39679-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39679-114">Not supported.</span></span>|
|<span data-ttu-id="39679-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39679-115">Application</span></span>| <span data-ttu-id="39679-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39679-116">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="39679-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39679-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="39679-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39679-118">Request headers</span></span>
|<span data-ttu-id="39679-119">Имя</span><span class="sxs-lookup"><span data-stu-id="39679-119">Name</span></span>|<span data-ttu-id="39679-120">Описание</span><span class="sxs-lookup"><span data-stu-id="39679-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="39679-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39679-121">Authorization</span></span>|<span data-ttu-id="39679-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39679-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="39679-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39679-124">Request body</span></span>
<span data-ttu-id="39679-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="39679-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39679-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="39679-126">Response</span></span>

<span data-ttu-id="39679-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="39679-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="39679-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="39679-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="39679-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="39679-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_accessreviewscheduledefinition"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/3856fd6f-36e2-4152-97c9-76070d19f730
```


### <a name="response"></a><span data-ttu-id="39679-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="39679-130">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
