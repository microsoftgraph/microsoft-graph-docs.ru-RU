---
title: Удаление учащегося
description: Удаляет educationUser из educationClass.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 59f0971d1ebcee69344235032103a61dac949437
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951691"
---
# <a name="remove-a-student"></a><span data-ttu-id="7e1d2-103">Удаление учащегося</span><span class="sxs-lookup"><span data-stu-id="7e1d2-103">Remove a student</span></span>

<span data-ttu-id="7e1d2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e1d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e1d2-105">Удаляет [educationUser](../resources/educationuser.md) из [educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="7e1d2-105">Removes an [educationUser](../resources/educationuser.md) from an [educationClass](../resources/educationclass.md)</span></span>

><span data-ttu-id="7e1d2-106">**Примечание.** Преподаватели _и_ учащиеся включены в коллекцию **members** курса.</span><span class="sxs-lookup"><span data-stu-id="7e1d2-106">**Note:** Teachers _and_ students are in the class **members** collection.</span></span> <span data-ttu-id="7e1d2-107">Перед вызовом этого API нужно проверить, не представляет ли удаляемый объект **educationUser** преподавателя.</span><span class="sxs-lookup"><span data-stu-id="7e1d2-107">Before calling this API, insure that the **educationUser** you are removing is not a teacher.</span></span>  <span data-ttu-id="7e1d2-108">Для этого необходимо получить список преподавателей путем вызова [educationclass_list_teachers](educationclass-list-teachers.md) и проверить, не возвращается ли в этом списке ИД удаляемого пользователя.</span><span class="sxs-lookup"><span data-stu-id="7e1d2-108">Get the list of teachers by calling [educationclass_list_teachers](educationclass-list-teachers.md) and verifying the user Id of the user to be removed is not in the returned teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e1d2-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7e1d2-109">Permissions</span></span>
<span data-ttu-id="7e1d2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e1d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e1d2-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e1d2-112">Permission type</span></span>      | <span data-ttu-id="7e1d2-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e1d2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e1d2-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e1d2-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="7e1d2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e1d2-115">Not supported.</span></span>  |
|<span data-ttu-id="7e1d2-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e1d2-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7e1d2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e1d2-117">Not supported.</span></span>  |
|<span data-ttu-id="7e1d2-118">Application</span><span class="sxs-lookup"><span data-stu-id="7e1d2-118">Application</span></span> | <span data-ttu-id="7e1d2-119">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e1d2-119">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7e1d2-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e1d2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/members/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="7e1d2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e1d2-121">Request headers</span></span>
| <span data-ttu-id="7e1d2-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7e1d2-122">Header</span></span>       | <span data-ttu-id="7e1d2-123">Значение</span><span class="sxs-lookup"><span data-stu-id="7e1d2-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7e1d2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e1d2-124">Authorization</span></span>  | <span data-ttu-id="7e1d2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e1d2-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7e1d2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7e1d2-127">Request body</span></span>
<span data-ttu-id="7e1d2-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e1d2-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="7e1d2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e1d2-129">Response</span></span>
<span data-ttu-id="7e1d2-130">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="7e1d2-130">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e1d2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7e1d2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7e1d2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e1d2-132">Request</span></span>
<span data-ttu-id="7e1d2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e1d2-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7e1d2-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e1d2-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool_1"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11003/members/14008
```
# <a name="c"></a>[<span data-ttu-id="7e1d2-135">C#</span><span class="sxs-lookup"><span data-stu-id="7e1d2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e1d2-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e1d2-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e1d2-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e1d2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7e1d2-138">Java</span><span class="sxs-lookup"><span data-stu-id="7e1d2-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationschool-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7e1d2-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e1d2-139">Response</span></span>
<span data-ttu-id="7e1d2-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7e1d2-140">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


