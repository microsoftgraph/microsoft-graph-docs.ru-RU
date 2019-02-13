---
title: 'записная книжка: getNotebookFromWebUrl'
description: Извлечение свойств и связи объекта записной книжки, с помощью его URL-адрес.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 3d14edf5a8992f9f4386e4b50aa74d54986b62f1
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/13/2019
ms.locfileid: "29982064"
---
# <a name="notebook-getnotebookfromweburl"></a><span data-ttu-id="847d3-103">записная книжка: getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="847d3-103">notebook: getNotebookFromWebUrl</span></span>

<span data-ttu-id="847d3-104">Извлечение свойств и связи объекта [записной книжки](../resources/notebook.md) с помощью его URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="847d3-104">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object by using its URL path.</span></span>

<span data-ttu-id="847d3-105">Расположение может быть записных книжек пользователя в Office 365, группа записных книжек или записных книжек размещенного сайта группы SharePoint на Office 365.</span><span class="sxs-lookup"><span data-stu-id="847d3-105">The location can be user notebooks on Office 365, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span>
## <a name="permissions"></a><span data-ttu-id="847d3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="847d3-106">Permissions</span></span>
<span data-ttu-id="847d3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="847d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="847d3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="847d3-109">Permission type</span></span>      | <span data-ttu-id="847d3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="847d3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="847d3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="847d3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="847d3-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="847d3-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="847d3-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="847d3-113">Application</span></span> | <span data-ttu-id="847d3-114">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="847d3-114">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="847d3-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="847d3-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/GetNotebookFromWebUrl
POST /users/{id | userPrincipalName}/onenote/notebooks/GetNotebookFromWebUrl
POST /groups/{id}/onenote/notebooks/GetNotebookFromWebUrl
POST /sites/{id}/onenote/notebooks/GetNotebookFromWebUrl
```
## <a name="request-headers"></a><span data-ttu-id="847d3-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="847d3-116">Request headers</span></span>
| <span data-ttu-id="847d3-117">Имя</span><span class="sxs-lookup"><span data-stu-id="847d3-117">Name</span></span>       | <span data-ttu-id="847d3-118">Тип</span><span class="sxs-lookup"><span data-stu-id="847d3-118">Type</span></span> | <span data-ttu-id="847d3-119">Описание</span><span class="sxs-lookup"><span data-stu-id="847d3-119">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="847d3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="847d3-120">Authorization</span></span>  | <span data-ttu-id="847d3-121">string</span><span class="sxs-lookup"><span data-stu-id="847d3-121">string</span></span>  | <span data-ttu-id="847d3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="847d3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="847d3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="847d3-124">Accept</span></span> | <span data-ttu-id="847d3-125">string</span><span class="sxs-lookup"><span data-stu-id="847d3-125">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="847d3-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="847d3-126">Request body</span></span>
<span data-ttu-id="847d3-127">В тексте запроса укажите JSON, представляющую полный путь URL-адрес к записной книжки, которую требуется получить.</span><span class="sxs-lookup"><span data-stu-id="847d3-127">In the request body, supply a JSON representation of the full URL path to the notebook you want to retrieve.</span></span>

| <span data-ttu-id="847d3-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="847d3-128">Property</span></span>     | <span data-ttu-id="847d3-129">Тип</span><span class="sxs-lookup"><span data-stu-id="847d3-129">Type</span></span>        | <span data-ttu-id="847d3-130">Описание</span><span class="sxs-lookup"><span data-stu-id="847d3-130">Description</span></span> |
|:-------------|:------------|:------------|
| `webUrl`     |`String`     | <span data-ttu-id="847d3-131">Путь к URL-адрес записной книжки для извлечения.</span><span class="sxs-lookup"><span data-stu-id="847d3-131">The URL path of the notebook to retrieve.</span></span> <span data-ttu-id="847d3-132">Он также может содержать «onenote:» префикс.</span><span class="sxs-lookup"><span data-stu-id="847d3-132">It can also contain a "onenote:" prefix.</span></span>|

## <a name="response"></a><span data-ttu-id="847d3-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="847d3-133">Response</span></span>

<span data-ttu-id="847d3-134">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [notebook](../resources/notebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="847d3-134">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="847d3-135">Пример</span><span class="sxs-lookup"><span data-stu-id="847d3-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="847d3-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="847d3-136">Request</span></span>
<span data-ttu-id="847d3-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="847d3-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_fromweburl"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/GetNotebookFromWebUrl
Content-type: application/json

{"webUrl":"webUrl value"}
```
##### <a name="response"></a><span data-ttu-id="847d3-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="847d3-138">Response</span></span>
<span data-ttu-id="847d3-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="847d3-139">Here is an example of the response.</span></span> 

><span data-ttu-id="847d3-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="847d3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
