---
title: Публикация назначения на образование
description: Это действие публикует назначение образования.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 8ba9c8933585997392f7e5aead6abd6fa34fa672
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912739"
---
# <a name="publish-an-education-assignment"></a><span data-ttu-id="dc2f8-103">Публикация назначения на образование</span><span class="sxs-lookup"><span data-stu-id="dc2f8-103">Publish an education assignment</span></span>

<span data-ttu-id="dc2f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc2f8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dc2f8-105">Это действие публикует назначение образования.</span><span class="sxs-lookup"><span data-stu-id="dc2f8-105">This action publishes an education assignment.</span></span>

 <span data-ttu-id="dc2f8-106">Только учитель в классе может сделать этот вызов.</span><span class="sxs-lookup"><span data-stu-id="dc2f8-106">Only a teacher in the class can make this call.</span></span> <span data-ttu-id="dc2f8-107">Когда назначение находится в состоянии черновика, учащиеся не будут видеть назначение, равно как и объекты отправки.</span><span class="sxs-lookup"><span data-stu-id="dc2f8-107">When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects.</span></span> <span data-ttu-id="dc2f8-108">Вызов этого API создает [объекты educationSubmission](../resources/educationsubmission.md) и отображает назначение в списке каждого учащегося.</span><span class="sxs-lookup"><span data-stu-id="dc2f8-108">Calling this API creates [educationSubmission](../resources/educationsubmission.md) objects and displays the assignment in each student's list.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc2f8-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dc2f8-109">Permissions</span></span>
<span data-ttu-id="dc2f8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc2f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc2f8-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc2f8-112">Permission type</span></span>      | <span data-ttu-id="dc2f8-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc2f8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc2f8-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc2f8-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="dc2f8-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc2f8-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="dc2f8-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc2f8-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="dc2f8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc2f8-117">Not supported.</span></span>  |
|<span data-ttu-id="dc2f8-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc2f8-118">Application</span></span> | <span data-ttu-id="dc2f8-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc2f8-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="dc2f8-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc2f8-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="dc2f8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc2f8-121">Request headers</span></span>
| <span data-ttu-id="dc2f8-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dc2f8-122">Header</span></span>       | <span data-ttu-id="dc2f8-123">Значение</span><span class="sxs-lookup"><span data-stu-id="dc2f8-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dc2f8-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc2f8-124">Authorization</span></span>  | <span data-ttu-id="dc2f8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc2f8-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dc2f8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dc2f8-127">Request body</span></span>
<span data-ttu-id="dc2f8-128">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dc2f8-128">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc2f8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc2f8-129">Response</span></span>
<span data-ttu-id="dc2f8-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dc2f8-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc2f8-132">Пример</span><span class="sxs-lookup"><span data-stu-id="dc2f8-132">Example</span></span>
<span data-ttu-id="dc2f8-133">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="dc2f8-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="dc2f8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc2f8-134">Request</span></span>
<span data-ttu-id="dc2f8-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc2f8-135">The following is an example of a request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["ad8afb28-c138-4ad7-b7f5-a6986c2655a8"],
  "name": "educationassignment_publish_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/publish
```

### <a name="response"></a><span data-ttu-id="dc2f8-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc2f8-136">Response</span></span>
<span data-ttu-id="dc2f8-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dc2f8-137">The following is an example of a response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 204 No Content

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


