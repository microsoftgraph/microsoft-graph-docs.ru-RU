---
title: SendReminder accessReview
description: 'Доступ к функции проверки в Azure AD, отправьте напоминание рецензентов текущего активного accessReview.  Конечный объект может быть review однократного доступа или экземпляр повторяющейся проверки доступа. '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cf5b78d2c67993fbf2da9be7c55a07fb752985c7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917281"
---
# <a name="sendreminder-accessreview"></a><span data-ttu-id="a6a06-104">SendReminder accessReview</span><span class="sxs-lookup"><span data-stu-id="a6a06-104">SendReminder accessReview</span></span>

> <span data-ttu-id="a6a06-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a6a06-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6a06-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6a06-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a6a06-107">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD отправьте напоминание рецензентов текущего активного [accessReview](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="a6a06-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, send a reminder to the reviewers of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="a6a06-108">Конечный объект может быть review однократного доступа или экземпляр повторяющейся проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="a6a06-108">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a6a06-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6a06-109">Permissions</span></span>
<span data-ttu-id="a6a06-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6a06-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6a06-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6a06-112">Permission type</span></span>                        | <span data-ttu-id="a6a06-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6a06-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6a06-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6a06-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="a6a06-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6a06-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="a6a06-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6a06-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6a06-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6a06-117">Not supported.</span></span> |
|<span data-ttu-id="a6a06-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6a06-118">Application</span></span>                            | <span data-ttu-id="a6a06-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6a06-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6a06-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6a06-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/sendReminder()
```
## <a name="request-headers"></a><span data-ttu-id="a6a06-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6a06-121">Request headers</span></span>
| <span data-ttu-id="a6a06-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a6a06-122">Name</span></span>         | <span data-ttu-id="a6a06-123">Тип</span><span class="sxs-lookup"><span data-stu-id="a6a06-123">Type</span></span>        | <span data-ttu-id="a6a06-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a6a06-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a6a06-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6a06-125">Authorization</span></span> | <span data-ttu-id="a6a06-126">string</span><span class="sxs-lookup"><span data-stu-id="a6a06-126">string</span></span> | <span data-ttu-id="a6a06-127">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="a6a06-127">Bearer \{token\}.</span></span> <span data-ttu-id="a6a06-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6a06-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6a06-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a6a06-129">Request body</span></span>
<span data-ttu-id="a6a06-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a6a06-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="a6a06-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6a06-131">Response</span></span>
<span data-ttu-id="a6a06-p106">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a6a06-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6a06-134">Пример</span><span class="sxs-lookup"><span data-stu-id="a6a06-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a6a06-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6a06-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/sendReminder()
```
##### <a name="response"></a><span data-ttu-id="a6a06-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6a06-136">Response</span></span>
><span data-ttu-id="a6a06-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6a06-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
