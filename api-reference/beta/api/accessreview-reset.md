---
title: Сброс accessReview
description: В компоненте обзоры доступа Azure AD Сброс решения текущего активного accessReview.  Конечный объект может быть review однократного доступа или экземпляр повторяющейся проверки доступа.  Предыдущие решения больше не записываются, но рецензентов можно продолжить обновление решения.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0b1f107733543380dbd6ad095133f09befc03736
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941494"
---
# <a name="reset-accessreview"></a><span data-ttu-id="25589-105">Сброс accessReview</span><span class="sxs-lookup"><span data-stu-id="25589-105">Reset accessReview</span></span>

> <span data-ttu-id="25589-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="25589-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="25589-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25589-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="25589-108">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD Сброс решения текущего активного [accessReview](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="25589-108">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, reset the decisions of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="25589-109">Конечный объект может быть review однократного доступа или экземпляр повторяющейся проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="25589-109">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="25589-110">Предыдущие решения больше не записываются, но рецензентов можно продолжить обновление решения.</span><span class="sxs-lookup"><span data-stu-id="25589-110">Previous decisions are no longer recorded, but reviewers can continue to update decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="25589-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="25589-111">Permissions</span></span>
<span data-ttu-id="25589-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25589-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25589-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25589-114">Permission type</span></span>                        | <span data-ttu-id="25589-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="25589-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="25589-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25589-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="25589-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25589-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="25589-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25589-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25589-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25589-119">Not supported.</span></span> |
|<span data-ttu-id="25589-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25589-120">Application</span></span>                            | <span data-ttu-id="25589-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25589-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="25589-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25589-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/resetDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="25589-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25589-123">Request headers</span></span>
| <span data-ttu-id="25589-124">Имя</span><span class="sxs-lookup"><span data-stu-id="25589-124">Name</span></span>         | <span data-ttu-id="25589-125">Тип</span><span class="sxs-lookup"><span data-stu-id="25589-125">Type</span></span>        | <span data-ttu-id="25589-126">Описание</span><span class="sxs-lookup"><span data-stu-id="25589-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="25589-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="25589-127">Authorization</span></span> | <span data-ttu-id="25589-128">строка</span><span class="sxs-lookup"><span data-stu-id="25589-128">string</span></span> | <span data-ttu-id="25589-129">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="25589-129">Bearer \{token\}.</span></span> <span data-ttu-id="25589-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25589-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25589-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="25589-131">Request body</span></span>
<span data-ttu-id="25589-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="25589-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="25589-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="25589-133">Response</span></span>
<span data-ttu-id="25589-p106">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="25589-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25589-136">Пример</span><span class="sxs-lookup"><span data-stu-id="25589-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="25589-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="25589-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "reset_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/resetDecisions()
```
##### <a name="response"></a><span data-ttu-id="25589-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="25589-138">Response</span></span>
><span data-ttu-id="25589-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="25589-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
