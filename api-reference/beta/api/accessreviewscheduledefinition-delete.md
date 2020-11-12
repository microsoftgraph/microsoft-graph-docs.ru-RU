---
title: Удаление Акцессревиевсчедуледефинитион
description: Удаление объекта Акцессревиевсчедуледефинитион.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d72e5321cf74e66bd34e48b4d6000715f11ea09d
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000982"
---
# <a name="delete-accessreviewscheduledefinition"></a><span data-ttu-id="8f5ee-103">Удаление Акцессревиевсчедуледефинитион</span><span class="sxs-lookup"><span data-stu-id="8f5ee-103">Delete accessReviewScheduleDefinition</span></span>

<span data-ttu-id="8f5ee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f5ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f5ee-105">Удаление объекта [акцессревиевсчедуледефинитион](../resources/accessreviewscheduledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="8f5ee-105">Delete an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8f5ee-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f5ee-106">Permissions</span></span>
<span data-ttu-id="8f5ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f5ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f5ee-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f5ee-109">Permission type</span></span>                        | <span data-ttu-id="8f5ee-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f5ee-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f5ee-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f5ee-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f5ee-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f5ee-112">AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="8f5ee-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f5ee-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f5ee-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f5ee-114">Not supported.</span></span>|
|<span data-ttu-id="8f5ee-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f5ee-115">Application</span></span>                            | <span data-ttu-id="8f5ee-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f5ee-116">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f5ee-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f5ee-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a><span data-ttu-id="8f5ee-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f5ee-118">Request headers</span></span>
<span data-ttu-id="8f5ee-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="8f5ee-119">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="8f5ee-120">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f5ee-120">Request body</span></span>
<span data-ttu-id="8f5ee-121">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8f5ee-121">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="8f5ee-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f5ee-122">Response</span></span>
<span data-ttu-id="8f5ee-p102">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8f5ee-p102">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8f5ee-125">Примеры</span><span class="sxs-lookup"><span data-stu-id="8f5ee-125">Examples</span></span>
### <a name="request"></a><span data-ttu-id="8f5ee-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f5ee-126">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_accessReviewScheduleDefinition"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/29f2d16e-9ca6-4052-bbfe-802c48981fd8
```

---

### <a name="response"></a><span data-ttu-id="8f5ee-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f5ee-127">Response</span></span>
><span data-ttu-id="8f5ee-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f5ee-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Delete accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
