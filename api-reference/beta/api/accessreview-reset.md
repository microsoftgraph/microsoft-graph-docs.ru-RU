---
title: Сброс accessReview
description: В компоненте обзоры доступа Azure AD Сброс решения текущего активного accessReview.  Конечный объект может быть review однократного доступа или экземпляр повторяющейся проверки доступа.  Предыдущие решения больше не записываются, но рецензентов можно продолжить обновление решения.
ms.openlocfilehash: b633a56926b56b33c509214d7574971056831967
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076017"
---
# <a name="reset-accessreview"></a><span data-ttu-id="8b8d2-105">Сброс accessReview</span><span class="sxs-lookup"><span data-stu-id="8b8d2-105">Reset accessReview</span></span>

> <span data-ttu-id="8b8d2-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8b8d2-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b8d2-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b8d2-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8b8d2-108">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD Сброс решения текущего активного [accessReview](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="8b8d2-108">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, reset the decisions of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="8b8d2-109">Конечный объект может быть review однократного доступа или экземпляр повторяющейся проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="8b8d2-109">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="8b8d2-110">Предыдущие решения больше не записываются, но рецензентов можно продолжить обновление решения.</span><span class="sxs-lookup"><span data-stu-id="8b8d2-110">Previous decisions are no longer recorded, but reviewers can continue to update decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b8d2-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b8d2-111">Permissions</span></span>
<span data-ttu-id="8b8d2-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b8d2-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b8d2-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b8d2-114">Permission type</span></span>                        | <span data-ttu-id="8b8d2-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b8d2-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b8d2-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b8d2-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b8d2-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b8d2-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="8b8d2-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b8d2-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b8d2-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b8d2-119">Not supported.</span></span> |
|<span data-ttu-id="8b8d2-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b8d2-120">Application</span></span>                            | <span data-ttu-id="8b8d2-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b8d2-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b8d2-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b8d2-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/resetDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="8b8d2-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b8d2-123">Request headers</span></span>
| <span data-ttu-id="8b8d2-124">Имя</span><span class="sxs-lookup"><span data-stu-id="8b8d2-124">Name</span></span>         | <span data-ttu-id="8b8d2-125">Тип</span><span class="sxs-lookup"><span data-stu-id="8b8d2-125">Type</span></span>        | <span data-ttu-id="8b8d2-126">Описание</span><span class="sxs-lookup"><span data-stu-id="8b8d2-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="8b8d2-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b8d2-127">Authorization</span></span> | <span data-ttu-id="8b8d2-128">string</span><span class="sxs-lookup"><span data-stu-id="8b8d2-128">string</span></span> | <span data-ttu-id="8b8d2-129">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="8b8d2-129">Bearer \{token\}.</span></span> <span data-ttu-id="8b8d2-130">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="8b8d2-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b8d2-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b8d2-131">Request body</span></span>
<span data-ttu-id="8b8d2-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8b8d2-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="8b8d2-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b8d2-133">Response</span></span>
<span data-ttu-id="8b8d2-p106">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8b8d2-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b8d2-136">Пример</span><span class="sxs-lookup"><span data-stu-id="8b8d2-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b8d2-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b8d2-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "reset_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/resetDecisions()
```
##### <a name="response"></a><span data-ttu-id="8b8d2-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b8d2-138">Response</span></span>
><span data-ttu-id="8b8d2-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b8d2-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
