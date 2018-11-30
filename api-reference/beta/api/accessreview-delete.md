---
title: Удаление accessReview
description: Доступ к функции проверки в Azure AD, удалить объект accessReview.
ms.openlocfilehash: b9578b575705de909eca99ac70f5efbb70d053cc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076009"
---
# <a name="delete-accessreview"></a><span data-ttu-id="da7d7-103">Удаление accessReview</span><span class="sxs-lookup"><span data-stu-id="da7d7-103">Delete accessReview</span></span>

> <span data-ttu-id="da7d7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="da7d7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da7d7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da7d7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="da7d7-106">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD удалите объект [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="da7d7-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="da7d7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da7d7-107">Permissions</span></span>
<span data-ttu-id="da7d7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da7d7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da7d7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da7d7-110">Permission type</span></span>                        | <span data-ttu-id="da7d7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da7d7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="da7d7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da7d7-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="da7d7-113">AccessReview.ReadWrite.All, а также должны иметь ProgramControl.ReadWrite.All для выполнения сценария с помощью вызова для удаления programControl</span><span class="sxs-lookup"><span data-stu-id="da7d7-113">AccessReview.ReadWrite.All, and should also have ProgramControl.ReadWrite.All to complete scenario with a call to delete a programControl</span></span> |
|<span data-ttu-id="da7d7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da7d7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da7d7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da7d7-115">Not supported.</span></span> |
|<span data-ttu-id="da7d7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da7d7-116">Application</span></span>                            | <span data-ttu-id="da7d7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da7d7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="da7d7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da7d7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="da7d7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da7d7-119">Request headers</span></span>
| <span data-ttu-id="da7d7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="da7d7-120">Name</span></span>         | <span data-ttu-id="da7d7-121">Тип</span><span class="sxs-lookup"><span data-stu-id="da7d7-121">Type</span></span>        | <span data-ttu-id="da7d7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="da7d7-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="da7d7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="da7d7-123">Authorization</span></span> | <span data-ttu-id="da7d7-124">string</span><span class="sxs-lookup"><span data-stu-id="da7d7-124">string</span></span> | <span data-ttu-id="da7d7-125">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="da7d7-125">Bearer \{token\}.</span></span> <span data-ttu-id="da7d7-126">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="da7d7-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da7d7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da7d7-127">Request body</span></span>
<span data-ttu-id="da7d7-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="da7d7-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="da7d7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="da7d7-129">Response</span></span>
<span data-ttu-id="da7d7-p104">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="da7d7-p104">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da7d7-132">Пример</span><span class="sxs-lookup"><span data-stu-id="da7d7-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da7d7-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="da7d7-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_accessReview"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')
```
##### <a name="response"></a><span data-ttu-id="da7d7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="da7d7-134">Response</span></span>
><span data-ttu-id="da7d7-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da7d7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
