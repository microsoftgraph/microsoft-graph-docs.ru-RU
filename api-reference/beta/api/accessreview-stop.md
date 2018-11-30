---
title: Остановка accessReview
description: В Azure AD access дается обзор компонента, Остановка текущего активного accessReview.  Конечный объект может быть review однократного доступа или экземпляр повторяющейся проверки доступа.  (Чтобы предотвратить запуск будущих экземпляры повторяющихся проверки доступа, обновите его, чтобы изменить его дату окончания).  После обеспечения доступа просмотрите останавливается, рецензентов больше не могут предоставить входные данные и решения проверки доступа можно применить.
ms.openlocfilehash: 2a4ac5d13f3be70cc5a4a24f4051429c473e7690
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077632"
---
# <a name="stop-accessreview"></a><span data-ttu-id="b1451-106">Остановка accessReview</span><span class="sxs-lookup"><span data-stu-id="b1451-106">Stop accessReview</span></span>

> <span data-ttu-id="b1451-107">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b1451-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1451-108">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1451-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b1451-109">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD Остановка текущего активного [accessReview](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="b1451-109">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, stop a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="b1451-110">Конечный объект может быть review однократного доступа или экземпляр повторяющейся проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="b1451-110">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="b1451-111">(Чтобы предотвратить повторяющихся проверки доступа запуск будущих экземпляры, [обновите его](accessreview-update.md) , чтобы изменить его дату окончания).</span><span class="sxs-lookup"><span data-stu-id="b1451-111">(To prevent a recurring access review from starting future instances, [update it](accessreview-update.md) to change its scheduled end date).</span></span>  <span data-ttu-id="b1451-112">После обеспечения доступа просмотрите останавливается, рецензентов больше не могут предоставить входные данные и решения проверки доступа можно применить.</span><span class="sxs-lookup"><span data-stu-id="b1451-112">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="b1451-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1451-113">Permissions</span></span>
<span data-ttu-id="b1451-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1451-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1451-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1451-116">Permission type</span></span>                        | <span data-ttu-id="b1451-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1451-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1451-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1451-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="b1451-119">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1451-119">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="b1451-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1451-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1451-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1451-121">Not supported.</span></span> |
|<span data-ttu-id="b1451-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1451-122">Application</span></span>                            | <span data-ttu-id="b1451-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1451-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1451-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1451-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/stop()
```
## <a name="request-headers"></a><span data-ttu-id="b1451-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1451-125">Request headers</span></span>
| <span data-ttu-id="b1451-126">Имя</span><span class="sxs-lookup"><span data-stu-id="b1451-126">Name</span></span>         | <span data-ttu-id="b1451-127">Тип</span><span class="sxs-lookup"><span data-stu-id="b1451-127">Type</span></span>        | <span data-ttu-id="b1451-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b1451-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b1451-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1451-129">Authorization</span></span> | <span data-ttu-id="b1451-130">string</span><span class="sxs-lookup"><span data-stu-id="b1451-130">string</span></span> | <span data-ttu-id="b1451-131">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="b1451-131">Bearer \{token\}.</span></span> <span data-ttu-id="b1451-132">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="b1451-132">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1451-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1451-133">Request body</span></span>
<span data-ttu-id="b1451-134">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b1451-134">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="b1451-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1451-135">Response</span></span>
<span data-ttu-id="b1451-p106">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b1451-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1451-138">Пример</span><span class="sxs-lookup"><span data-stu-id="b1451-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1451-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1451-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "stop_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/stop()
```
##### <a name="response"></a><span data-ttu-id="b1451-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1451-140">Response</span></span>
><span data-ttu-id="b1451-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1451-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Stop accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
