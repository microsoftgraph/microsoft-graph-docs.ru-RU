---
title: 'educationSubmission: отзыв'
description: 'Указывает, что студенту требуется выполнить отправку. Это действие можно выполнить только студентом. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 606a2a5325da9aed6203303e40ad5b3b95f0d7d6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007251"
---
# <a name="educationsubmission-recall"></a><span data-ttu-id="32949-104">educationSubmission: отзыв</span><span class="sxs-lookup"><span data-stu-id="32949-104">educationSubmission: recall</span></span>

<span data-ttu-id="32949-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32949-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32949-106">Указывает, что студенту требуется выполнить отправку.</span><span class="sxs-lookup"><span data-stu-id="32949-106">Indicates that a student wants to take back a submission.</span></span> <span data-ttu-id="32949-107">Это действие можно выполнить только студентом.</span><span class="sxs-lookup"><span data-stu-id="32949-107">This action can only be done by a student.</span></span> <span data-ttu-id="32949-108">Он изменит состояние отправки с "Отправлено" обратно на "работает".</span><span class="sxs-lookup"><span data-stu-id="32949-108">It will change the status of the submission from "submitted" back to "working".</span></span>

## <a name="permissions"></a><span data-ttu-id="32949-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="32949-109">Permissions</span></span>

<span data-ttu-id="32949-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32949-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="32949-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32949-112">Permission type</span></span>                        | <span data-ttu-id="32949-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="32949-113">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="32949-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32949-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="32949-115">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32949-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="32949-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32949-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32949-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="32949-117">Not supported</span></span>                                           |
| <span data-ttu-id="32949-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32949-118">Application</span></span>                            | <span data-ttu-id="32949-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32949-119">Not supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="32949-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32949-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/recall
```

## <a name="request-headers"></a><span data-ttu-id="32949-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32949-121">Request headers</span></span>

| <span data-ttu-id="32949-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="32949-122">Header</span></span>        | <span data-ttu-id="32949-123">Значение</span><span class="sxs-lookup"><span data-stu-id="32949-123">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="32949-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32949-124">Authorization</span></span> | <span data-ttu-id="32949-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32949-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="32949-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="32949-127">Response</span></span>

<span data-ttu-id="32949-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="32949-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32949-130">Пример</span><span class="sxs-lookup"><span data-stu-id="32949-130">Example</span></span>

<span data-ttu-id="32949-131">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="32949-131">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="32949-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="32949-132">Request</span></span>

<span data-ttu-id="32949-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32949-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationsubmission_recall"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/recall
```

##### <a name="response"></a><span data-ttu-id="32949-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="32949-134">Response</span></span>

<span data-ttu-id="32949-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="32949-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission: recall",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


