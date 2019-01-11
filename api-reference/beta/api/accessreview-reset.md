---
title: Сброс accessReview
description: В компоненте обзоры доступа Azure AD Сброс решения текущего активного accessReview.  Конечный объект может быть review однократного доступа или экземпляр повторяющейся проверки доступа.  Предыдущие решения больше не записываются, но рецензентов можно продолжить обновление решения.
localization_priority: Normal
ms.openlocfilehash: 750b9e4da130a087350b7b78c53e71c835d12be1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809578"
---
# <a name="reset-accessreview"></a><span data-ttu-id="11b6d-105">Сброс accessReview</span><span class="sxs-lookup"><span data-stu-id="11b6d-105">Reset accessReview</span></span>

> <span data-ttu-id="11b6d-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="11b6d-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11b6d-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11b6d-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="11b6d-108">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD Сброс решения текущего активного [accessReview](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="11b6d-108">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, reset the decisions of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="11b6d-109">Конечный объект может быть review однократного доступа или экземпляр повторяющейся проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="11b6d-109">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="11b6d-110">Предыдущие решения больше не записываются, но рецензентов можно продолжить обновление решения.</span><span class="sxs-lookup"><span data-stu-id="11b6d-110">Previous decisions are no longer recorded, but reviewers can continue to update decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="11b6d-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="11b6d-111">Permissions</span></span>
<span data-ttu-id="11b6d-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11b6d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11b6d-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11b6d-114">Permission type</span></span>                        | <span data-ttu-id="11b6d-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="11b6d-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="11b6d-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11b6d-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="11b6d-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11b6d-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="11b6d-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11b6d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11b6d-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11b6d-119">Not supported.</span></span> |
|<span data-ttu-id="11b6d-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11b6d-120">Application</span></span>                            | <span data-ttu-id="11b6d-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11b6d-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="11b6d-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11b6d-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/resetDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="11b6d-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11b6d-123">Request headers</span></span>
| <span data-ttu-id="11b6d-124">Имя</span><span class="sxs-lookup"><span data-stu-id="11b6d-124">Name</span></span>         | <span data-ttu-id="11b6d-125">Тип</span><span class="sxs-lookup"><span data-stu-id="11b6d-125">Type</span></span>        | <span data-ttu-id="11b6d-126">Описание</span><span class="sxs-lookup"><span data-stu-id="11b6d-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="11b6d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="11b6d-127">Authorization</span></span> | <span data-ttu-id="11b6d-128">string</span><span class="sxs-lookup"><span data-stu-id="11b6d-128">string</span></span> | <span data-ttu-id="11b6d-129">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="11b6d-129">Bearer \{token\}.</span></span> <span data-ttu-id="11b6d-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11b6d-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11b6d-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="11b6d-131">Request body</span></span>
<span data-ttu-id="11b6d-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="11b6d-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="11b6d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="11b6d-133">Response</span></span>
<span data-ttu-id="11b6d-p106">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="11b6d-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11b6d-136">Пример</span><span class="sxs-lookup"><span data-stu-id="11b6d-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="11b6d-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="11b6d-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "reset_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/resetDecisions()
```
##### <a name="response"></a><span data-ttu-id="11b6d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="11b6d-138">Response</span></span>
><span data-ttu-id="11b6d-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="11b6d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Reset accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
