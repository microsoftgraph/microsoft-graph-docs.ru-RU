---
title: Создание записной книжки
description: Создание записной книжки OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: deeb775f19ba2378cd15ffcbd72ef2caafd23b83
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514826"
---
# <a name="create-notebook"></a><span data-ttu-id="7f44b-103">Создание записной книжки</span><span class="sxs-lookup"><span data-stu-id="7f44b-103">Create notebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f44b-104">Создание [записной книжки](../resources/notebook.md) OneNote.</span><span class="sxs-lookup"><span data-stu-id="7f44b-104">Create a new OneNote [notebook](../resources/notebook.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="7f44b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f44b-105">Permissions</span></span>
<span data-ttu-id="7f44b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f44b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f44b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f44b-108">Permission type</span></span>      | <span data-ttu-id="7f44b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f44b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f44b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f44b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7f44b-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f44b-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="7f44b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f44b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f44b-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f44b-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="7f44b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f44b-114">Application</span></span> | <span data-ttu-id="7f44b-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f44b-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f44b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f44b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks
POST /users/{id | userPrincipalName}/onenote/notebooks
POST /groups/{id}/onenote/notebooks
POST /sites/{id}/onenote/notebooks
```
## <a name="request-headers"></a><span data-ttu-id="7f44b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f44b-117">Request headers</span></span>
| <span data-ttu-id="7f44b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7f44b-118">Name</span></span>       | <span data-ttu-id="7f44b-119">Тип</span><span class="sxs-lookup"><span data-stu-id="7f44b-119">Type</span></span> | <span data-ttu-id="7f44b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7f44b-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7f44b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f44b-121">Authorization</span></span>  | <span data-ttu-id="7f44b-122">строка</span><span class="sxs-lookup"><span data-stu-id="7f44b-122">string</span></span>  | <span data-ttu-id="7f44b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f44b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7f44b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7f44b-125">Content-Type</span></span> | <span data-ttu-id="7f44b-126">string</span><span class="sxs-lookup"><span data-stu-id="7f44b-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="7f44b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7f44b-127">Request body</span></span>
<span data-ttu-id="7f44b-128">В теле запроса укажите имя записной книжки.</span><span class="sxs-lookup"><span data-stu-id="7f44b-128">In the request body, supply a name for the notebook.</span></span> 

<span data-ttu-id="7f44b-p103">Имена записных книжек должны быть уникальными. Имя должно содержать не более 128 символов, в нем не должно быть следующих знаков:  ?\*\/:<>|'"</span><span class="sxs-lookup"><span data-stu-id="7f44b-p103">Notebook names must be unique. The name cannot contain more than 128 characters or contain the following characters:  ?\*\/:<>|'"</span></span>

## <a name="response"></a><span data-ttu-id="7f44b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f44b-131">Response</span></span>

<span data-ttu-id="7f44b-132">При успешном выполнении этот метод возвращает код отклика `201 Created` и новый объект [notebook](../resources/notebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7f44b-132">If successful, this method returns a `201 Created` response code and the new [notebook](../resources/notebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f44b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="7f44b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f44b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f44b-134">Request</span></span>
<span data-ttu-id="7f44b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f44b-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_notebook_from_onenote"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks
Content-type: application/json
Content-length: 30

{
  "displayName": "Notebook name"
}
```

##### <a name="response"></a><span data-ttu-id="7f44b-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f44b-136">Response</span></span>
<span data-ttu-id="7f44b-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7f44b-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 284

{
  "isDefault": true,
  "userRole": {
  },
  "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
  "isShared": true,
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/onenote-post-notebooks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
