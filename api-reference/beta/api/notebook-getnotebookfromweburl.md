---
title: 'записная книжка: getNotebookFromWebUrl'
description: Извлечение свойств и связи объекта записной книжки, с помощью его URL-адрес.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 226cbd70343feaf8fe5404aac6077f9b2438aba8
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/13/2019
ms.locfileid: "29982071"
---
# <a name="notebook-getnotebookfromweburl"></a><span data-ttu-id="5319f-103">записная книжка: getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="5319f-103">notebook: getNotebookFromWebUrl</span></span>

[! ВКЛЮЧИТЬ бета-версии-заявление об отказе]

<span data-ttu-id="5319f-105">Извлечение свойств и связи объекта [записной книжки](../resources/notebook.md) с помощью его URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="5319f-105">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object by using its URL path.</span></span>

<span data-ttu-id="5319f-106">Расположение может быть записных книжек пользователя в Office 365, группа записных книжек или записных книжек размещенного сайта группы SharePoint на Office 365.</span><span class="sxs-lookup"><span data-stu-id="5319f-106">The location can be user notebooks on Office 365, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span>
## <a name="permissions"></a><span data-ttu-id="5319f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5319f-107">Permissions</span></span>
<span data-ttu-id="5319f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5319f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5319f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5319f-110">Permission type</span></span>      | <span data-ttu-id="5319f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5319f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5319f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5319f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5319f-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5319f-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="5319f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5319f-114">Application</span></span> | <span data-ttu-id="5319f-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5319f-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5319f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5319f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/GetNotebookFromWebUrl
POST /users/{id | userPrincipalName}/onenote/notebooks/GetNotebookFromWebUrl
POST /groups/{id}/onenote/notebooks/GetNotebookFromWebUrl
POST /sites/{id}/onenote/notebooks/GetNotebookFromWebUrl
```
## <a name="request-headers"></a><span data-ttu-id="5319f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5319f-117">Request headers</span></span>
| <span data-ttu-id="5319f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="5319f-118">Name</span></span>       | <span data-ttu-id="5319f-119">Тип</span><span class="sxs-lookup"><span data-stu-id="5319f-119">Type</span></span> | <span data-ttu-id="5319f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5319f-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5319f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5319f-121">Authorization</span></span>  | <span data-ttu-id="5319f-122">string</span><span class="sxs-lookup"><span data-stu-id="5319f-122">string</span></span>  | <span data-ttu-id="5319f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5319f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5319f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5319f-125">Accept</span></span> | <span data-ttu-id="5319f-126">string</span><span class="sxs-lookup"><span data-stu-id="5319f-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="5319f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5319f-127">Request body</span></span>
<span data-ttu-id="5319f-128">В тексте запроса укажите JSON, представляющую полный путь URL-адрес к записной книжки, которую требуется получить.</span><span class="sxs-lookup"><span data-stu-id="5319f-128">In the request body, supply a JSON representation of the full URL path to the notebook you want to retrieve.</span></span>

| <span data-ttu-id="5319f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5319f-129">Property</span></span>     | <span data-ttu-id="5319f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5319f-130">Type</span></span>        | <span data-ttu-id="5319f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5319f-131">Description</span></span> |
|:-------------|:------------|:------------|
| `webUrl`     |`String`     | <span data-ttu-id="5319f-132">Путь к URL-адрес записной книжки для извлечения.</span><span class="sxs-lookup"><span data-stu-id="5319f-132">The URL path of the notebook to retrieve.</span></span> <span data-ttu-id="5319f-133">Он также может содержать «onenote:» префикс.</span><span class="sxs-lookup"><span data-stu-id="5319f-133">It can also contain a "onenote:" prefix.</span></span>|

## <a name="response"></a><span data-ttu-id="5319f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5319f-134">Response</span></span>

<span data-ttu-id="5319f-135">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [notebook](../resources/notebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5319f-135">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5319f-136">Пример</span><span class="sxs-lookup"><span data-stu-id="5319f-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5319f-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="5319f-137">Request</span></span>
<span data-ttu-id="5319f-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5319f-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_fromweburl"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/GetNotebookFromWebUrl
Content-type: application/json

{"webUrl":"webUrl value"}
```
##### <a name="response"></a><span data-ttu-id="5319f-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="5319f-139">Response</span></span>
<span data-ttu-id="5319f-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5319f-140">Here is an example of the response.</span></span> 

><span data-ttu-id="5319f-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5319f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json; odata.metadata=minimal
Content-Length: 544

{
    "isDefault": true,
    "userRole": "userRole-value",
    "isShared": true,
    "sectionsUrl": "sectionUrl-value",
    "sectionGroupsUrl": "sectionGroupUrl-value",
    "links": {
        "oneNoteClientUrl": {
            "href": "href-value"
        },
        "oneNoteWebUrl": {
            "href": "href-value"
        }
    },
    "id": "id-value",
    "self": "self-value",
}
```
<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error:{notebook-getnotebookfromweburl.md}:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
