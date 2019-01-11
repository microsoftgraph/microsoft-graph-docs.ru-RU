---
title: 'educationAssignment: getResourcesFolderUrl'
description: 'Эта функция возвращает URL-адрес OneDrive, где требуется отправить все файловым ресурсам (Word, Excel и т. д.).  '
localization_priority: Normal
ms.openlocfilehash: 4352fb051573f91ef93e781a1a06ba984b17a9ed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887390"
---
# <a name="educationassignment-getresourcesfolderurl"></a><span data-ttu-id="46efa-103">educationAssignment: getResourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="46efa-103">educationAssignment: getResourcesFolderUrl</span></span>

> <span data-ttu-id="46efa-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="46efa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46efa-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46efa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="46efa-106">Эта функция возвращает URL-адрес OneDrive, где требуется отправить все файловым ресурсам (Word, Excel и т. д.).</span><span class="sxs-lookup"><span data-stu-id="46efa-106">This function returns the OneDrive URL where all file-based resources (Word, Excel, and so on) should be uploaded.</span></span>  
<span data-ttu-id="46efa-107">Обратите внимание на то, что файлы должны быть расположены в этой папке быть добавлен в качестве ресурсов.</span><span class="sxs-lookup"><span data-stu-id="46efa-107">Note that files must be located in this folder in order to be added as resources.</span></span> <span data-ttu-id="46efa-108">Только преподаватель в классе можно определить, какие файлы для загрузки.</span><span class="sxs-lookup"><span data-stu-id="46efa-108">Only a teacher in the class can determine what files to upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="46efa-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="46efa-109">Permissions</span></span>
<span data-ttu-id="46efa-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46efa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46efa-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46efa-112">Permission type</span></span>      | <span data-ttu-id="46efa-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="46efa-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46efa-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46efa-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="46efa-115">EduAssignments.ReadBasic EduAssignments.Read</span><span class="sxs-lookup"><span data-stu-id="46efa-115">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="46efa-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46efa-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="46efa-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46efa-117">Not supported.</span></span>  |
|<span data-ttu-id="46efa-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46efa-118">Application</span></span> | <span data-ttu-id="46efa-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46efa-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="46efa-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46efa-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/getResourcesFolderUrl

```
## <a name="request-headers"></a><span data-ttu-id="46efa-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46efa-121">Request headers</span></span>
| <span data-ttu-id="46efa-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46efa-122">Header</span></span>       | <span data-ttu-id="46efa-123">Значение</span><span class="sxs-lookup"><span data-stu-id="46efa-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="46efa-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46efa-124">Authorization</span></span>  | <span data-ttu-id="46efa-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46efa-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="46efa-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="46efa-127">Request body</span></span>
<span data-ttu-id="46efa-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="46efa-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="46efa-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="46efa-129">Response</span></span>
<span data-ttu-id="46efa-130">В случае успешного выполнения этот метод возвращает код отклика `200 Ok`.</span><span class="sxs-lookup"><span data-stu-id="46efa-130">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="46efa-131">Текст будет содержать OneDrive URL-адрес папки для размещения всех файловым ресурсам.</span><span class="sxs-lookup"><span data-stu-id="46efa-131">The body will contain the OneDrive URL of a folder in which to put all file-based resources.</span></span>

## <a name="example"></a><span data-ttu-id="46efa-132">Пример</span><span class="sxs-lookup"><span data-stu-id="46efa-132">Example</span></span>
<span data-ttu-id="46efa-133">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="46efa-133">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="46efa-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="46efa-134">Request</span></span>
<span data-ttu-id="46efa-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46efa-135">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/getResourcesFolderUrl
```

##### <a name="response"></a><span data-ttu-id="46efa-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="46efa-136">Response</span></span>
<span data-ttu-id="46efa-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="46efa-137">The following is an example of a response.</span></span> 

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
