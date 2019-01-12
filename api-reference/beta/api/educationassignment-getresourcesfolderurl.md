---
title: 'educationAssignment: getResourcesFolderUrl'
description: 'Эта функция возвращает URL-адрес OneDrive, где требуется отправить все файловым ресурсам (Word, Excel и т. д.).  '
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: f46bbf9c47ca9cd4396883d106599f94374aad4a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984460"
---
# <a name="educationassignment-getresourcesfolderurl"></a><span data-ttu-id="4dfe3-103">educationAssignment: getResourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="4dfe3-103">educationAssignment: getResourcesFolderUrl</span></span>

> <span data-ttu-id="4dfe3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4dfe3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4dfe3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dfe3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4dfe3-106">Эта функция возвращает URL-адрес OneDrive, где требуется отправить все файловым ресурсам (Word, Excel и т. д.).</span><span class="sxs-lookup"><span data-stu-id="4dfe3-106">This function returns the OneDrive URL where all file-based resources (Word, Excel, and so on) should be uploaded.</span></span>  
<span data-ttu-id="4dfe3-107">Обратите внимание на то, что файлы должны быть расположены в этой папке быть добавлен в качестве ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4dfe3-107">Note that files must be located in this folder in order to be added as resources.</span></span> <span data-ttu-id="4dfe3-108">Только преподаватель в классе можно определить, какие файлы для загрузки.</span><span class="sxs-lookup"><span data-stu-id="4dfe3-108">Only a teacher in the class can determine what files to upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="4dfe3-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4dfe3-109">Permissions</span></span>
<span data-ttu-id="4dfe3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4dfe3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dfe3-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4dfe3-112">Permission type</span></span>      | <span data-ttu-id="4dfe3-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4dfe3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4dfe3-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4dfe3-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="4dfe3-115">EduAssignments.ReadBasic EduAssignments.Read</span><span class="sxs-lookup"><span data-stu-id="4dfe3-115">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="4dfe3-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4dfe3-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4dfe3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dfe3-117">Not supported.</span></span>  |
|<span data-ttu-id="4dfe3-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4dfe3-118">Application</span></span> | <span data-ttu-id="4dfe3-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dfe3-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4dfe3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4dfe3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/getResourcesFolderUrl

```
## <a name="request-headers"></a><span data-ttu-id="4dfe3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4dfe3-121">Request headers</span></span>
| <span data-ttu-id="4dfe3-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4dfe3-122">Header</span></span>       | <span data-ttu-id="4dfe3-123">Значение</span><span class="sxs-lookup"><span data-stu-id="4dfe3-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4dfe3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4dfe3-124">Authorization</span></span>  | <span data-ttu-id="4dfe3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4dfe3-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4dfe3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4dfe3-127">Request body</span></span>
<span data-ttu-id="4dfe3-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4dfe3-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4dfe3-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="4dfe3-129">Response</span></span>
<span data-ttu-id="4dfe3-130">В случае успешного выполнения этот метод возвращает код отклика `200 Ok`.</span><span class="sxs-lookup"><span data-stu-id="4dfe3-130">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="4dfe3-131">Текст будет содержать OneDrive URL-адрес папки для размещения всех файловым ресурсам.</span><span class="sxs-lookup"><span data-stu-id="4dfe3-131">The body will contain the OneDrive URL of a folder in which to put all file-based resources.</span></span>

## <a name="example"></a><span data-ttu-id="4dfe3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4dfe3-132">Example</span></span>
<span data-ttu-id="4dfe3-133">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="4dfe3-133">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4dfe3-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4dfe3-134">Request</span></span>
<span data-ttu-id="4dfe3-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4dfe3-135">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/getResourcesFolderUrl
```

##### <a name="response"></a><span data-ttu-id="4dfe3-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="4dfe3-136">Response</span></span>
<span data-ttu-id="4dfe3-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4dfe3-137">The following is an example of a response.</span></span> 

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
