---
title: Удаление учащегося
description: Удаляет educationUser из educationClass.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 58d288a4ab60d306b8346fa8681cd18621c83fb0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517631"
---
# <a name="remove-a-student"></a><span data-ttu-id="bdbc3-103">Удаление учащегося</span><span class="sxs-lookup"><span data-stu-id="bdbc3-103">Remove a student</span></span>

<span data-ttu-id="bdbc3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdbc3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bdbc3-105">Удаляет [educationUser](../resources/educationuser.md) из [educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="bdbc3-105">Removes an [educationUser](../resources/educationuser.md) from an [educationClass](../resources/educationclass.md)</span></span>

><span data-ttu-id="bdbc3-106">**Примечание.** Преподаватели _и_ учащиеся включены в коллекцию **members** курса.</span><span class="sxs-lookup"><span data-stu-id="bdbc3-106">**Note:** Teachers _and_ students are in the class **members** collection.</span></span> <span data-ttu-id="bdbc3-107">Перед вызовом этого API нужно проверить, не представляет ли удаляемый объект **educationUser** преподавателя.</span><span class="sxs-lookup"><span data-stu-id="bdbc3-107">Before calling this API, insure that the **educationUser** you are removing is not a teacher.</span></span>  <span data-ttu-id="bdbc3-108">Для этого необходимо получить список преподавателей путем вызова [educationclass_list_teachers](educationclass-list-teachers.md) и проверить, не возвращается ли в этом списке ИД удаляемого пользователя.</span><span class="sxs-lookup"><span data-stu-id="bdbc3-108">Get the list of teachers by calling [educationclass_list_teachers](educationclass-list-teachers.md) and verifying the user Id of the user to be removed is not in the returned teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="bdbc3-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bdbc3-109">Permissions</span></span>
<span data-ttu-id="bdbc3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdbc3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdbc3-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bdbc3-112">Permission type</span></span>      | <span data-ttu-id="bdbc3-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bdbc3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdbc3-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bdbc3-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="bdbc3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdbc3-115">Not supported.</span></span>  |
|<span data-ttu-id="bdbc3-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdbc3-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="bdbc3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdbc3-117">Not supported.</span></span>  |
|<span data-ttu-id="bdbc3-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bdbc3-118">Application</span></span> | <span data-ttu-id="bdbc3-119">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdbc3-119">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="bdbc3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bdbc3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/members/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="bdbc3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bdbc3-121">Request headers</span></span>
| <span data-ttu-id="bdbc3-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bdbc3-122">Header</span></span>       | <span data-ttu-id="bdbc3-123">Значение</span><span class="sxs-lookup"><span data-stu-id="bdbc3-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bdbc3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bdbc3-124">Authorization</span></span>  | <span data-ttu-id="bdbc3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bdbc3-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bdbc3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bdbc3-127">Request body</span></span>
<span data-ttu-id="bdbc3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bdbc3-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="bdbc3-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="bdbc3-129">Response</span></span>
<span data-ttu-id="bdbc3-130">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="bdbc3-130">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdbc3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bdbc3-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bdbc3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdbc3-132">Request</span></span>
<span data-ttu-id="bdbc3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bdbc3-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bdbc3-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="bdbc3-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}/members/{member-id}
```
# <a name="c"></a>[<span data-ttu-id="bdbc3-135">C#</span><span class="sxs-lookup"><span data-stu-id="bdbc3-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bdbc3-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bdbc3-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bdbc3-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bdbc3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bdbc3-138">Java</span><span class="sxs-lookup"><span data-stu-id="bdbc3-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bdbc3-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdbc3-139">Response</span></span>
<span data-ttu-id="bdbc3-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bdbc3-140">The following is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
