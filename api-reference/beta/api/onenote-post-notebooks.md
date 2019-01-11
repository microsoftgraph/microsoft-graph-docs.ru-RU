---
title: Создание записной книжки
description: Создание записной книжки OneNote.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 8ad8f2f68989796c2c041fdd758017044f0c73e9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826588"
---
# <a name="create-notebook"></a><span data-ttu-id="c9ade-103">Создание записной книжки</span><span class="sxs-lookup"><span data-stu-id="c9ade-103">Create notebook</span></span>

> <span data-ttu-id="c9ade-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c9ade-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9ade-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9ade-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c9ade-106">Создание [записной книжки](../resources/notebook.md) OneNote.</span><span class="sxs-lookup"><span data-stu-id="c9ade-106">Create a new OneNote [notebook](../resources/notebook.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="c9ade-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9ade-107">Permissions</span></span>
<span data-ttu-id="c9ade-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9ade-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9ade-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9ade-110">Permission type</span></span>      | <span data-ttu-id="c9ade-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9ade-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9ade-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9ade-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c9ade-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9ade-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="c9ade-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9ade-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9ade-115">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9ade-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="c9ade-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9ade-116">Application</span></span> | <span data-ttu-id="c9ade-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9ade-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9ade-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9ade-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks
POST /users/{id | userPrincipalName}/onenote/notebooks
POST /groups/{id}/onenote/notebooks
POST /sites/{id}/onenote/notebooks
```
## <a name="request-headers"></a><span data-ttu-id="c9ade-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9ade-119">Request headers</span></span>
| <span data-ttu-id="c9ade-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c9ade-120">Name</span></span>       | <span data-ttu-id="c9ade-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c9ade-121">Type</span></span> | <span data-ttu-id="c9ade-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c9ade-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c9ade-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9ade-123">Authorization</span></span>  | <span data-ttu-id="c9ade-124">string</span><span class="sxs-lookup"><span data-stu-id="c9ade-124">string</span></span>  | <span data-ttu-id="c9ade-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9ade-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c9ade-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c9ade-127">Content-Type</span></span> | <span data-ttu-id="c9ade-128">string</span><span class="sxs-lookup"><span data-stu-id="c9ade-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="c9ade-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c9ade-129">Request body</span></span>
<span data-ttu-id="c9ade-130">В теле запроса укажите имя записной книжки.</span><span class="sxs-lookup"><span data-stu-id="c9ade-130">In the request body, supply a name for the notebook.</span></span> 

<span data-ttu-id="c9ade-p104">Имена записных книжек должны быть уникальными. Имя должно содержать не более 128 символов, в нем не должно быть следующих знаков:  ?\*\/:<>|'"</span><span class="sxs-lookup"><span data-stu-id="c9ade-p104">Notebook names must be unique. The name cannot contain more than 128 characters or contain the following characters:  ?\*\/:<>|'"</span></span>

## <a name="response"></a><span data-ttu-id="c9ade-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9ade-133">Response</span></span>

<span data-ttu-id="c9ade-134">При успешном выполнении этот метод возвращает код отклика `201 Created` и новый объект [notebook](../resources/notebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c9ade-134">If successful, this method returns a `201 Created` response code and the new [notebook](../resources/notebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9ade-135">Пример</span><span class="sxs-lookup"><span data-stu-id="c9ade-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c9ade-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9ade-136">Request</span></span>
<span data-ttu-id="c9ade-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9ade-137">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c9ade-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9ade-138">Response</span></span>
<span data-ttu-id="c9ade-p105">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9ade-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
