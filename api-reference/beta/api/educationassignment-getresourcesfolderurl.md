---
title: 'educationAssignment: getResourcesFolderUrl'
description: 'Эта функция возвращает URL-адрес OneDrive, куда должны быть загружены все ресурсы на основе файлов (Word, Excel и так далее).  '
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ce5f35560a25f2a57742d93293788038e13cb179
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951852"
---
# <a name="educationassignment-getresourcesfolderurl"></a><span data-ttu-id="51f48-103">educationAssignment: getResourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="51f48-103">educationAssignment: getResourcesFolderUrl</span></span>

<span data-ttu-id="51f48-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51f48-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51f48-105">Эта функция возвращает URL-адрес OneDrive, куда должны быть загружены все ресурсы на основе файлов (Word, Excel и так далее).</span><span class="sxs-lookup"><span data-stu-id="51f48-105">This function returns the OneDrive URL where all file-based resources (Word, Excel, and so on) should be uploaded.</span></span>  
<span data-ttu-id="51f48-106">Обратите внимание, что файлы должны быть размещены в этой папке, чтобы они были добавлены в качестве ресурсов.</span><span class="sxs-lookup"><span data-stu-id="51f48-106">Note that files must be located in this folder in order to be added as resources.</span></span> <span data-ttu-id="51f48-107">Только учитель в классе может определить, какие файлы загрузить.</span><span class="sxs-lookup"><span data-stu-id="51f48-107">Only a teacher in the class can determine what files to upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="51f48-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51f48-108">Permissions</span></span>
<span data-ttu-id="51f48-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51f48-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51f48-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51f48-111">Permission type</span></span>      | <span data-ttu-id="51f48-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51f48-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51f48-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51f48-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="51f48-114">EduAssignments.ReadBasic, EduAssignments.Read</span><span class="sxs-lookup"><span data-stu-id="51f48-114">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="51f48-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51f48-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="51f48-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51f48-116">Not supported.</span></span>  |
|<span data-ttu-id="51f48-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51f48-117">Application</span></span> | <span data-ttu-id="51f48-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51f48-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="51f48-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51f48-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/getResourcesFolderUrl

```
## <a name="request-headers"></a><span data-ttu-id="51f48-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51f48-120">Request headers</span></span>
| <span data-ttu-id="51f48-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51f48-121">Header</span></span>       | <span data-ttu-id="51f48-122">Значение</span><span class="sxs-lookup"><span data-stu-id="51f48-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="51f48-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51f48-123">Authorization</span></span>  | <span data-ttu-id="51f48-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51f48-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="51f48-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51f48-126">Request body</span></span>
<span data-ttu-id="51f48-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51f48-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="51f48-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="51f48-128">Response</span></span>
<span data-ttu-id="51f48-129">В случае успешного выполнения этот метод возвращает код отклика `200 Ok`.</span><span class="sxs-lookup"><span data-stu-id="51f48-129">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="51f48-130">В теле будет содержаться URL-адрес папки OneDrive, в который будут помещаться все ресурсы на основе файлов.</span><span class="sxs-lookup"><span data-stu-id="51f48-130">The body will contain the OneDrive URL of a folder in which to put all file-based resources.</span></span>

## <a name="example"></a><span data-ttu-id="51f48-131">Пример</span><span class="sxs-lookup"><span data-stu-id="51f48-131">Example</span></span>
<span data-ttu-id="51f48-132">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="51f48-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="51f48-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="51f48-133">Request</span></span>
<span data-ttu-id="51f48-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51f48-134">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="51f48-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="51f48-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/getResourcesFolderUrl
```
# <a name="c"></a>[<span data-ttu-id="51f48-136">C#</span><span class="sxs-lookup"><span data-stu-id="51f48-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-publish-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51f48-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51f48-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-publish-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51f48-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51f48-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-publish-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51f48-139">Java</span><span class="sxs-lookup"><span data-stu-id="51f48-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationassignment-publish-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="51f48-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="51f48-140">Response</span></span>
<span data-ttu-id="51f48-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="51f48-141">The following is an example of a response.</span></span> 

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


