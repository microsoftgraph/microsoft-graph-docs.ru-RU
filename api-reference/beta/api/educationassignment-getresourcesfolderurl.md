---
title: 'educationAssignment: Жетресаурцесфолдерурл'
description: 'Эта функция возвращает URL-адрес OneDrive, где будут отправляться все файловые ресурсы (Word, Excel и т. д.).  '
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: d172928f0bfd25e80e1ae8c5b1b2cafbc9958b5a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33588117"
---
# <a name="educationassignment-getresourcesfolderurl"></a><span data-ttu-id="51ae2-103">educationAssignment: Жетресаурцесфолдерурл</span><span class="sxs-lookup"><span data-stu-id="51ae2-103">educationAssignment: getResourcesFolderUrl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51ae2-104">Эта функция возвращает URL-адрес OneDrive, где будут отправляться все файловые ресурсы (Word, Excel и т. д.).</span><span class="sxs-lookup"><span data-stu-id="51ae2-104">This function returns the OneDrive URL where all file-based resources (Word, Excel, and so on) should be uploaded.</span></span>  
<span data-ttu-id="51ae2-105">Обратите внимание, что файлы должны находиться в этой папке, чтобы добавить их в качестве ресурсов.</span><span class="sxs-lookup"><span data-stu-id="51ae2-105">Note that files must be located in this folder in order to be added as resources.</span></span> <span data-ttu-id="51ae2-106">Файлы, которые требуется отправить, могут определить только преподаватель в классе.</span><span class="sxs-lookup"><span data-stu-id="51ae2-106">Only a teacher in the class can determine what files to upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="51ae2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51ae2-107">Permissions</span></span>
<span data-ttu-id="51ae2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51ae2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51ae2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51ae2-110">Permission type</span></span>      | <span data-ttu-id="51ae2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51ae2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51ae2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51ae2-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="51ae2-113">EduAssignments. ReadBasic, EduAssignments. Read</span><span class="sxs-lookup"><span data-stu-id="51ae2-113">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="51ae2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51ae2-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="51ae2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51ae2-115">Not supported.</span></span>  |
|<span data-ttu-id="51ae2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51ae2-116">Application</span></span> | <span data-ttu-id="51ae2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51ae2-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="51ae2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51ae2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/getResourcesFolderUrl

```
## <a name="request-headers"></a><span data-ttu-id="51ae2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51ae2-119">Request headers</span></span>
| <span data-ttu-id="51ae2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51ae2-120">Header</span></span>       | <span data-ttu-id="51ae2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="51ae2-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="51ae2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51ae2-122">Authorization</span></span>  | <span data-ttu-id="51ae2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51ae2-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="51ae2-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51ae2-125">Request body</span></span>
<span data-ttu-id="51ae2-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51ae2-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="51ae2-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="51ae2-127">Response</span></span>
<span data-ttu-id="51ae2-128">В случае успешного выполнения этот метод возвращает код отклика `200 Ok`.</span><span class="sxs-lookup"><span data-stu-id="51ae2-128">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="51ae2-129">Основной текст будет содержать URL-адрес OneDrive папки, в которую будут помещены все файловые ресурсы.</span><span class="sxs-lookup"><span data-stu-id="51ae2-129">The body will contain the OneDrive URL of a folder in which to put all file-based resources.</span></span>

## <a name="example"></a><span data-ttu-id="51ae2-130">Пример</span><span class="sxs-lookup"><span data-stu-id="51ae2-130">Example</span></span>
<span data-ttu-id="51ae2-131">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="51ae2-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="51ae2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="51ae2-132">Request</span></span>
<span data-ttu-id="51ae2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51ae2-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/getResourcesFolderUrl
```

##### <a name="response"></a><span data-ttu-id="51ae2-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="51ae2-134">Response</span></span>
<span data-ttu-id="51ae2-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="51ae2-135">The following is an example of a response.</span></span> 

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="51ae2-136">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="51ae2-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="51ae2-137">Языках</span><span class="sxs-lookup"><span data-stu-id="51ae2-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/educationassignment_publish-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="51ae2-138">Язык</span><span class="sxs-lookup"><span data-stu-id="51ae2-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/educationassignment_publish-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/educationassignment-getresourcesfolderurl.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationassignment-getresourcesfolderurl.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
