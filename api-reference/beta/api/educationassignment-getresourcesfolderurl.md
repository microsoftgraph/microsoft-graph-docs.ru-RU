---
title: 'educationAssignment: Жетресаурцесфолдерурл'
description: 'Эта функция возвращает URL-адрес OneDrive, где будут отправляться все файловые ресурсы (Word, Excel и т. д.).  '
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 4745e62b043baba21bbb207f34f1da09d58a16b4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324234"
---
# <a name="educationassignment-getresourcesfolderurl"></a><span data-ttu-id="25e72-103">educationAssignment: Жетресаурцесфолдерурл</span><span class="sxs-lookup"><span data-stu-id="25e72-103">educationAssignment: getResourcesFolderUrl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25e72-104">Эта функция возвращает URL-адрес OneDrive, где будут отправляться все файловые ресурсы (Word, Excel и т. д.).</span><span class="sxs-lookup"><span data-stu-id="25e72-104">This function returns the OneDrive URL where all file-based resources (Word, Excel, and so on) should be uploaded.</span></span>  
<span data-ttu-id="25e72-105">Обратите внимание, что файлы должны находиться в этой папке, чтобы добавить их в качестве ресурсов.</span><span class="sxs-lookup"><span data-stu-id="25e72-105">Note that files must be located in this folder in order to be added as resources.</span></span> <span data-ttu-id="25e72-106">Файлы, которые требуется отправить, могут определить только преподаватель в классе.</span><span class="sxs-lookup"><span data-stu-id="25e72-106">Only a teacher in the class can determine what files to upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="25e72-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="25e72-107">Permissions</span></span>
<span data-ttu-id="25e72-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25e72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25e72-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25e72-110">Permission type</span></span>      | <span data-ttu-id="25e72-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="25e72-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25e72-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25e72-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="25e72-113">EduAssignments. ReadBasic, EduAssignments. Read</span><span class="sxs-lookup"><span data-stu-id="25e72-113">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="25e72-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25e72-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="25e72-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25e72-115">Not supported.</span></span>  |
|<span data-ttu-id="25e72-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25e72-116">Application</span></span> | <span data-ttu-id="25e72-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25e72-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="25e72-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25e72-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/getResourcesFolderUrl

```
## <a name="request-headers"></a><span data-ttu-id="25e72-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25e72-119">Request headers</span></span>
| <span data-ttu-id="25e72-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="25e72-120">Header</span></span>       | <span data-ttu-id="25e72-121">Значение</span><span class="sxs-lookup"><span data-stu-id="25e72-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="25e72-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="25e72-122">Authorization</span></span>  | <span data-ttu-id="25e72-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25e72-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="25e72-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="25e72-125">Request body</span></span>
<span data-ttu-id="25e72-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="25e72-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="25e72-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="25e72-127">Response</span></span>
<span data-ttu-id="25e72-128">В случае успешного выполнения этот метод возвращает код отклика `200 Ok`.</span><span class="sxs-lookup"><span data-stu-id="25e72-128">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="25e72-129">Основной текст будет содержать URL-адрес OneDrive папки, в которую будут помещены все файловые ресурсы.</span><span class="sxs-lookup"><span data-stu-id="25e72-129">The body will contain the OneDrive URL of a folder in which to put all file-based resources.</span></span>

## <a name="example"></a><span data-ttu-id="25e72-130">Пример</span><span class="sxs-lookup"><span data-stu-id="25e72-130">Example</span></span>
<span data-ttu-id="25e72-131">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="25e72-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="25e72-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="25e72-132">Request</span></span>
<span data-ttu-id="25e72-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25e72-133">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="25e72-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="25e72-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/getResourcesFolderUrl
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="25e72-135">C#</span><span class="sxs-lookup"><span data-stu-id="25e72-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-publish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="25e72-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25e72-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-publish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="25e72-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="25e72-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-publish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="25e72-138">Java</span><span class="sxs-lookup"><span data-stu-id="25e72-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationassignment-publish-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="25e72-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="25e72-139">Response</span></span>
<span data-ttu-id="25e72-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="25e72-140">The following is an example of a response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Edm.String",
    "value": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T"
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
