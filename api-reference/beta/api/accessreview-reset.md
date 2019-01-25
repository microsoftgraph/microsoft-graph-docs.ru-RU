---
title: Сброс accessReview
description: В компоненте обзоры доступа Azure AD Сброс решения текущего активного accessReview.  Конечный объект может быть review однократного доступа или экземпляр повторяющейся проверки доступа.  Предыдущие решения больше не записываются, но рецензентов можно продолжить обновление решения.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4e258a781707d2c3fe5419e3ebd5f7c6b43f271b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517017"
---
# <a name="reset-accessreview"></a><span data-ttu-id="3ada0-105">Сброс accessReview</span><span class="sxs-lookup"><span data-stu-id="3ada0-105">Reset accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ada0-106">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD Сброс решения текущего активного [accessReview](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="3ada0-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, reset the decisions of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="3ada0-107">Конечный объект может быть review однократного доступа или экземпляр повторяющейся проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="3ada0-107">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="3ada0-108">Предыдущие решения больше не записываются, но рецензентов можно продолжить обновление решения.</span><span class="sxs-lookup"><span data-stu-id="3ada0-108">Previous decisions are no longer recorded, but reviewers can continue to update decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ada0-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3ada0-109">Permissions</span></span>
<span data-ttu-id="3ada0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ada0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ada0-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ada0-112">Permission type</span></span>                        | <span data-ttu-id="3ada0-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ada0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ada0-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ada0-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="3ada0-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ada0-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="3ada0-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ada0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ada0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ada0-117">Not supported.</span></span> |
|<span data-ttu-id="3ada0-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ada0-118">Application</span></span>                            | <span data-ttu-id="3ada0-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ada0-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ada0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ada0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/resetDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="3ada0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ada0-121">Request headers</span></span>
| <span data-ttu-id="3ada0-122">Имя</span><span class="sxs-lookup"><span data-stu-id="3ada0-122">Name</span></span>         | <span data-ttu-id="3ada0-123">Тип</span><span class="sxs-lookup"><span data-stu-id="3ada0-123">Type</span></span>        | <span data-ttu-id="3ada0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3ada0-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3ada0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ada0-125">Authorization</span></span> | <span data-ttu-id="3ada0-126">string</span><span class="sxs-lookup"><span data-stu-id="3ada0-126">string</span></span> | <span data-ttu-id="3ada0-127">Маркер носителя</span><span class="sxs-lookup"><span data-stu-id="3ada0-127">Bearer \{token\}.</span></span> <span data-ttu-id="3ada0-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ada0-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ada0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3ada0-129">Request body</span></span>
<span data-ttu-id="3ada0-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3ada0-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="3ada0-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="3ada0-131">Response</span></span>
<span data-ttu-id="3ada0-p105">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3ada0-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ada0-134">Пример</span><span class="sxs-lookup"><span data-stu-id="3ada0-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3ada0-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ada0-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "reset_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/resetDecisions()
```
##### <a name="response"></a><span data-ttu-id="3ada0-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ada0-136">Response</span></span>
><span data-ttu-id="3ada0-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3ada0-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Reset accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-reset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
