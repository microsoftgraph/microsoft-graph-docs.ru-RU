---
title: 'educationAssignment: getResourcesFolderUrl (deprecated)'
description: 'Эта функция возвращает URL OneDrive, где должны быть загружены все ресурсы на основе файлов (Word, Excel и так далее).  '
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 44c7caec25b4d96b225598041f59bfcaa3f5d3ac
ms.sourcegitcommit: 40a8e4b9e344811267025e23c372a6e60e31a1b9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/01/2021
ms.locfileid: "52119007"
---
# <a name="educationassignment-getresourcesfolderurl-deprecated"></a><span data-ttu-id="941c8-103">educationAssignment: getResourcesFolderUrl (deprecated)</span><span class="sxs-lookup"><span data-stu-id="941c8-103">educationAssignment: getResourcesFolderUrl (deprecated)</span></span>

<span data-ttu-id="941c8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="941c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 [!CAUTION] <span data-ttu-id="941c8-105">API getResourcesFolderUrl обесценен и прекратит возвращать данные 31 мая 2021 г.</span><span class="sxs-lookup"><span data-stu-id="941c8-105">The getResourcesFolderUrl API is deprecated and will stop returning data on May 31, 2021.</span></span> <span data-ttu-id="941c8-106">Чтобы получить эту информацию, используйте новое свойство, выставленное на `resourcesFolderUrl` [объекте educationAssignment.](../resources/educationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="941c8-106">Please use the new property `resourcesFolderUrl` exposed on [educationAssignment](../resources/educationassignment.md) entity to fetch this info.</span></span> 

<span data-ttu-id="941c8-107">Эта функция возвращает URL OneDrive, где должны быть загружены все ресурсы на основе файлов (Word, Excel и так далее).</span><span class="sxs-lookup"><span data-stu-id="941c8-107">This function returns the OneDrive URL where all file-based resources (Word, Excel, and so on) should be uploaded.</span></span>  
<span data-ttu-id="941c8-108">Обратите внимание, что файлы должны быть размещены в этой папке, чтобы они были добавлены в качестве ресурсов.</span><span class="sxs-lookup"><span data-stu-id="941c8-108">Note that files must be located in this folder in order to be added as resources.</span></span> <span data-ttu-id="941c8-109">Только учитель в классе может определить, какие файлы загрузить.</span><span class="sxs-lookup"><span data-stu-id="941c8-109">Only a teacher in the class can determine what files to upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="941c8-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="941c8-110">Permissions</span></span>
<span data-ttu-id="941c8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="941c8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="941c8-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="941c8-113">Permission type</span></span>      | <span data-ttu-id="941c8-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="941c8-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="941c8-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="941c8-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="941c8-116">EduAssignments.ReadBasic, EduAssignments.Read</span><span class="sxs-lookup"><span data-stu-id="941c8-116">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="941c8-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="941c8-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="941c8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="941c8-118">Not supported.</span></span>  |
|<span data-ttu-id="941c8-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="941c8-119">Application</span></span> | <span data-ttu-id="941c8-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="941c8-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="941c8-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="941c8-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/getResourcesFolderUrl

```
## <a name="request-headers"></a><span data-ttu-id="941c8-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="941c8-122">Request headers</span></span>
| <span data-ttu-id="941c8-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="941c8-123">Header</span></span>       | <span data-ttu-id="941c8-124">Значение</span><span class="sxs-lookup"><span data-stu-id="941c8-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="941c8-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="941c8-125">Authorization</span></span>  | <span data-ttu-id="941c8-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="941c8-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="941c8-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="941c8-128">Request body</span></span>
<span data-ttu-id="941c8-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="941c8-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="941c8-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="941c8-130">Response</span></span>
<span data-ttu-id="941c8-131">В случае успешного выполнения этот метод возвращает код отклика `200 Ok`.</span><span class="sxs-lookup"><span data-stu-id="941c8-131">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="941c8-132">В теле будет OneDrive URL-адрес папки, в который будут помещаться все ресурсы на основе файлов.</span><span class="sxs-lookup"><span data-stu-id="941c8-132">The body will contain the OneDrive URL of a folder in which to put all file-based resources.</span></span>

## <a name="example"></a><span data-ttu-id="941c8-133">Пример</span><span class="sxs-lookup"><span data-stu-id="941c8-133">Example</span></span>
<span data-ttu-id="941c8-134">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="941c8-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="941c8-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="941c8-135">Request</span></span>
<span data-ttu-id="941c8-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="941c8-136">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="941c8-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="941c8-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/getResourcesFolderUrl
```
# <a name="c"></a>[<span data-ttu-id="941c8-138">C#</span><span class="sxs-lookup"><span data-stu-id="941c8-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-publish-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="941c8-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="941c8-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-publish-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="941c8-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="941c8-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-publish-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="941c8-141">Java</span><span class="sxs-lookup"><span data-stu-id="941c8-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationassignment-publish-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="941c8-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="941c8-142">Response</span></span>
<span data-ttu-id="941c8-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="941c8-143">The following is an example of a response.</span></span> 

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


