---
title: 'educationAssignment: Жетресаурцесфолдерурл'
description: 'Эта функция возвращает URL-адрес OneDrive, где будут отправляться все файловые ресурсы (Word, Excel и т. д.).  '
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 97730a35e107cbaa3f3901fac8eceb473e89c602
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436174"
---
# <a name="educationassignment-getresourcesfolderurl"></a><span data-ttu-id="05b0b-103">educationAssignment: Жетресаурцесфолдерурл</span><span class="sxs-lookup"><span data-stu-id="05b0b-103">educationAssignment: getResourcesFolderUrl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05b0b-104">Эта функция возвращает URL-адрес OneDrive, где будут отправляться все файловые ресурсы (Word, Excel и т. д.).</span><span class="sxs-lookup"><span data-stu-id="05b0b-104">This function returns the OneDrive URL where all file-based resources (Word, Excel, and so on) should be uploaded.</span></span>  
<span data-ttu-id="05b0b-105">Обратите внимание, что файлы должны находиться в этой папке, чтобы добавить их в качестве ресурсов.</span><span class="sxs-lookup"><span data-stu-id="05b0b-105">Note that files must be located in this folder in order to be added as resources.</span></span> <span data-ttu-id="05b0b-106">Файлы, которые требуется отправить, могут определить только преподаватель в классе.</span><span class="sxs-lookup"><span data-stu-id="05b0b-106">Only a teacher in the class can determine what files to upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="05b0b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="05b0b-107">Permissions</span></span>
<span data-ttu-id="05b0b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05b0b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05b0b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05b0b-110">Permission type</span></span>      | <span data-ttu-id="05b0b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="05b0b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05b0b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05b0b-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="05b0b-113">EduAssignments. ReadBasic, EduAssignments. Read</span><span class="sxs-lookup"><span data-stu-id="05b0b-113">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="05b0b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05b0b-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="05b0b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05b0b-115">Not supported.</span></span>  |
|<span data-ttu-id="05b0b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05b0b-116">Application</span></span> | <span data-ttu-id="05b0b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05b0b-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="05b0b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05b0b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/getResourcesFolderUrl

```
## <a name="request-headers"></a><span data-ttu-id="05b0b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05b0b-119">Request headers</span></span>
| <span data-ttu-id="05b0b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="05b0b-120">Header</span></span>       | <span data-ttu-id="05b0b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="05b0b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="05b0b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="05b0b-122">Authorization</span></span>  | <span data-ttu-id="05b0b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05b0b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="05b0b-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="05b0b-125">Request body</span></span>
<span data-ttu-id="05b0b-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="05b0b-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="05b0b-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="05b0b-127">Response</span></span>
<span data-ttu-id="05b0b-128">В случае успешного выполнения этот метод возвращает код отклика `200 Ok`.</span><span class="sxs-lookup"><span data-stu-id="05b0b-128">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="05b0b-129">Основной текст будет содержать URL-адрес OneDrive папки, в которую будут помещены все файловые ресурсы.</span><span class="sxs-lookup"><span data-stu-id="05b0b-129">The body will contain the OneDrive URL of a folder in which to put all file-based resources.</span></span>

## <a name="example"></a><span data-ttu-id="05b0b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="05b0b-130">Example</span></span>
<span data-ttu-id="05b0b-131">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="05b0b-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="05b0b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="05b0b-132">Request</span></span>
<span data-ttu-id="05b0b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05b0b-133">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="05b0b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="05b0b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/getResourcesFolderUrl
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="05b0b-135">C#</span><span class="sxs-lookup"><span data-stu-id="05b0b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-publish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="05b0b-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="05b0b-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-publish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="05b0b-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="05b0b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-publish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="05b0b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="05b0b-138">Response</span></span>
<span data-ttu-id="05b0b-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="05b0b-139">The following is an example of a response.</span></span> 

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
