---
title: SendReminder accessReview
description: 'Доступ к функции проверки в Azure AD, отправьте напоминание рецензентов текущего активного accessReview.  Конечный объект может быть review однократного доступа или экземпляр повторяющейся проверки доступа. '
ms.openlocfilehash: fd8c204db207ae9f58c4dd5e6337e65efe160824
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077621"
---
# <a name="sendreminder-accessreview"></a><span data-ttu-id="7d282-104">SendReminder accessReview</span><span class="sxs-lookup"><span data-stu-id="7d282-104">SendReminder accessReview</span></span>

> <span data-ttu-id="7d282-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7d282-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d282-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d282-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7d282-107">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD отправьте напоминание рецензентов текущего активного [accessReview](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="7d282-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, send a reminder to the reviewers of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="7d282-108">Конечный объект может быть review однократного доступа или экземпляр повторяющейся проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="7d282-108">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span> 

## <a name="permissions"></a><span data-ttu-id="7d282-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7d282-109">Permissions</span></span>
<span data-ttu-id="7d282-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d282-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d282-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d282-112">Permission type</span></span>                        | <span data-ttu-id="7d282-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d282-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d282-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d282-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="7d282-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d282-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="7d282-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d282-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d282-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d282-117">Not supported.</span></span> |
|<span data-ttu-id="7d282-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7d282-118">Application</span></span>                            | <span data-ttu-id="7d282-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d282-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d282-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d282-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/sendReminder()
```
## <a name="request-headers"></a><span data-ttu-id="7d282-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d282-121">Request headers</span></span>
| <span data-ttu-id="7d282-122">Имя</span><span class="sxs-lookup"><span data-stu-id="7d282-122">Name</span></span>         | <span data-ttu-id="7d282-123">Тип</span><span class="sxs-lookup"><span data-stu-id="7d282-123">Type</span></span>        | <span data-ttu-id="7d282-124">Описание</span><span class="sxs-lookup"><span data-stu-id="7d282-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7d282-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d282-125">Authorization</span></span> | <span data-ttu-id="7d282-126">string</span><span class="sxs-lookup"><span data-stu-id="7d282-126">string</span></span> | <span data-ttu-id="7d282-127">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="7d282-127">Bearer \{token\}.</span></span> <span data-ttu-id="7d282-128">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="7d282-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d282-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d282-129">Request body</span></span>
<span data-ttu-id="7d282-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7d282-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="7d282-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d282-131">Response</span></span>
<span data-ttu-id="7d282-p106">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7d282-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d282-134">Пример</span><span class="sxs-lookup"><span data-stu-id="7d282-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7d282-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d282-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/sendReminder()
```
##### <a name="response"></a><span data-ttu-id="7d282-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d282-136">Response</span></span>
><span data-ttu-id="7d282-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d282-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "SendReminder accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
