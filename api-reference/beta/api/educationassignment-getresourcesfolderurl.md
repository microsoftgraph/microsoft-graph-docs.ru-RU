---
title: 'educationAssignment: Жетресаурцесфолдерурл'
description: 'Эта функция возвращает URL-адрес OneDrive, где будут отправляться все файловые ресурсы (Word, Excel и т. д.).  '
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d7520db351be8d9b78506354e14988bd479fda92
ms.sourcegitcommit: fc818699566f03493937be95447eb9f656a1f950
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534415"
---
# <a name="educationassignment-getresourcesfolderurl"></a><span data-ttu-id="dd0b3-103">educationAssignment: Жетресаурцесфолдерурл</span><span class="sxs-lookup"><span data-stu-id="dd0b3-103">educationAssignment: getResourcesFolderUrl</span></span>

<span data-ttu-id="dd0b3-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dd0b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd0b3-105">Эта функция возвращает URL-адрес OneDrive, где будут отправляться все файловые ресурсы (Word, Excel и т. д.).</span><span class="sxs-lookup"><span data-stu-id="dd0b3-105">This function returns the OneDrive URL where all file-based resources (Word, Excel, and so on) should be uploaded.</span></span>  
<span data-ttu-id="dd0b3-106">Обратите внимание, что файлы должны находиться в этой папке, чтобы добавить их в качестве ресурсов.</span><span class="sxs-lookup"><span data-stu-id="dd0b3-106">Note that files must be located in this folder in order to be added as resources.</span></span> <span data-ttu-id="dd0b3-107">Файлы, которые требуется отправить, могут определить только преподаватель в классе.</span><span class="sxs-lookup"><span data-stu-id="dd0b3-107">Only a teacher in the class can determine what files to upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="dd0b3-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd0b3-108">Permissions</span></span>
<span data-ttu-id="dd0b3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd0b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd0b3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd0b3-111">Permission type</span></span>      | <span data-ttu-id="dd0b3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd0b3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd0b3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd0b3-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="dd0b3-114">EduAssignments. ReadBasic, EduAssignments. Read</span><span class="sxs-lookup"><span data-stu-id="dd0b3-114">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="dd0b3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd0b3-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="dd0b3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd0b3-116">Not supported.</span></span>  |
|<span data-ttu-id="dd0b3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd0b3-117">Application</span></span> | <span data-ttu-id="dd0b3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd0b3-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="dd0b3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd0b3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/getResourcesFolderUrl

```
## <a name="request-headers"></a><span data-ttu-id="dd0b3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd0b3-120">Request headers</span></span>
| <span data-ttu-id="dd0b3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dd0b3-121">Header</span></span>       | <span data-ttu-id="dd0b3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dd0b3-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dd0b3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd0b3-123">Authorization</span></span>  | <span data-ttu-id="dd0b3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd0b3-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dd0b3-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd0b3-126">Request body</span></span>
<span data-ttu-id="dd0b3-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dd0b3-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="dd0b3-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd0b3-128">Response</span></span>
<span data-ttu-id="dd0b3-129">В случае успешного выполнения этот метод возвращает код отклика `200 Ok`.</span><span class="sxs-lookup"><span data-stu-id="dd0b3-129">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="dd0b3-130">Основной текст будет содержать URL-адрес OneDrive папки, в которую будут помещены все файловые ресурсы.</span><span class="sxs-lookup"><span data-stu-id="dd0b3-130">The body will contain the OneDrive URL of a folder in which to put all file-based resources.</span></span>

## <a name="example"></a><span data-ttu-id="dd0b3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="dd0b3-131">Example</span></span>
<span data-ttu-id="dd0b3-132">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="dd0b3-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dd0b3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd0b3-133">Request</span></span>
<span data-ttu-id="dd0b3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd0b3-134">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dd0b3-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd0b3-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/getResourcesFolderUrl
```
# <a name="c"></a>[<span data-ttu-id="dd0b3-136">C#</span><span class="sxs-lookup"><span data-stu-id="dd0b3-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-publish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd0b3-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd0b3-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-publish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd0b3-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd0b3-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-publish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dd0b3-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd0b3-139">Response</span></span>
<span data-ttu-id="dd0b3-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dd0b3-140">The following is an example of a response.</span></span> 

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
