---
title: 'educationAssignment: getResourcesFolderUrl'
description: 'Эта функция возвращает URL-адрес OneDrive, где требуется отправить все файловым ресурсам (Word, Excel и т. д.).  '
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 43bef729d2cf37561d0742ebb3adfb21fe4f486e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512033"
---
# <a name="educationassignment-getresourcesfolderurl"></a><span data-ttu-id="71f9b-103">educationAssignment: getResourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="71f9b-103">educationAssignment: getResourcesFolderUrl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71f9b-104">Эта функция возвращает URL-адрес OneDrive, где требуется отправить все файловым ресурсам (Word, Excel и т. д.).</span><span class="sxs-lookup"><span data-stu-id="71f9b-104">This function returns the OneDrive URL where all file-based resources (Word, Excel, and so on) should be uploaded.</span></span>  
<span data-ttu-id="71f9b-105">Обратите внимание на то, что файлы должны быть расположены в этой папке быть добавлен в качестве ресурсов.</span><span class="sxs-lookup"><span data-stu-id="71f9b-105">Note that files must be located in this folder in order to be added as resources.</span></span> <span data-ttu-id="71f9b-106">Только преподаватель в классе можно определить, какие файлы для загрузки.</span><span class="sxs-lookup"><span data-stu-id="71f9b-106">Only a teacher in the class can determine what files to upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="71f9b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71f9b-107">Permissions</span></span>
<span data-ttu-id="71f9b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71f9b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71f9b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71f9b-110">Permission type</span></span>      | <span data-ttu-id="71f9b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71f9b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71f9b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71f9b-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="71f9b-113">EduAssignments.ReadBasic EduAssignments.Read</span><span class="sxs-lookup"><span data-stu-id="71f9b-113">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="71f9b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71f9b-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="71f9b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71f9b-115">Not supported.</span></span>  |
|<span data-ttu-id="71f9b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71f9b-116">Application</span></span> | <span data-ttu-id="71f9b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71f9b-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="71f9b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71f9b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/getResourcesFolderUrl

```
## <a name="request-headers"></a><span data-ttu-id="71f9b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71f9b-119">Request headers</span></span>
| <span data-ttu-id="71f9b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="71f9b-120">Header</span></span>       | <span data-ttu-id="71f9b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="71f9b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="71f9b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71f9b-122">Authorization</span></span>  | <span data-ttu-id="71f9b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71f9b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="71f9b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71f9b-125">Request body</span></span>
<span data-ttu-id="71f9b-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71f9b-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="71f9b-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="71f9b-127">Response</span></span>
<span data-ttu-id="71f9b-128">В случае успешного выполнения этот метод возвращает код отклика `200 Ok`.</span><span class="sxs-lookup"><span data-stu-id="71f9b-128">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="71f9b-129">Текст будет содержать OneDrive URL-адрес папки для размещения всех файловым ресурсам.</span><span class="sxs-lookup"><span data-stu-id="71f9b-129">The body will contain the OneDrive URL of a folder in which to put all file-based resources.</span></span>

## <a name="example"></a><span data-ttu-id="71f9b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="71f9b-130">Example</span></span>
<span data-ttu-id="71f9b-131">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="71f9b-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="71f9b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="71f9b-132">Request</span></span>
<span data-ttu-id="71f9b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71f9b-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/getResourcesFolderUrl
```

##### <a name="response"></a><span data-ttu-id="71f9b-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="71f9b-134">Response</span></span>
<span data-ttu-id="71f9b-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="71f9b-135">The following is an example of a response.</span></span> 

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
    "Error: /api-reference/beta/api/educationassignment-getresourcesfolderurl.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
