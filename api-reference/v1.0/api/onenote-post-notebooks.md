---
title: Создание записной книжки
description: Создание записной книжки OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 2dec1f425c16a69ca0f1389975c0f250c67b2992
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473117"
---
# <a name="create-notebook"></a><span data-ttu-id="b7de6-103">Создание записной книжки</span><span class="sxs-lookup"><span data-stu-id="b7de6-103">Create notebook</span></span>

<span data-ttu-id="b7de6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7de6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b7de6-105">Создание новой записной [](../resources/notebook.md)книжки OneNote.</span><span class="sxs-lookup"><span data-stu-id="b7de6-105">Create a new OneNote [notebook](../resources/notebook.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="b7de6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b7de6-106">Permissions</span></span>
<span data-ttu-id="b7de6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7de6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7de6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7de6-109">Permission type</span></span>      | <span data-ttu-id="b7de6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7de6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7de6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7de6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b7de6-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7de6-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="b7de6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7de6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7de6-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7de6-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="b7de6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7de6-115">Application</span></span> | <span data-ttu-id="b7de6-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7de6-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7de6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7de6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks
POST /users/{id | userPrincipalName}/onenote/notebooks
POST /groups/{id}/onenote/notebooks
POST /sites/{id}/onenote/notebooks
```
## <a name="request-headers"></a><span data-ttu-id="b7de6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7de6-118">Request headers</span></span>
| <span data-ttu-id="b7de6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b7de6-119">Name</span></span>       | <span data-ttu-id="b7de6-120">Тип</span><span class="sxs-lookup"><span data-stu-id="b7de6-120">Type</span></span> | <span data-ttu-id="b7de6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b7de6-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b7de6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7de6-122">Authorization</span></span>  | <span data-ttu-id="b7de6-123">string</span><span class="sxs-lookup"><span data-stu-id="b7de6-123">string</span></span>  | <span data-ttu-id="b7de6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7de6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b7de6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b7de6-126">Content-Type</span></span> | <span data-ttu-id="b7de6-127">string</span><span class="sxs-lookup"><span data-stu-id="b7de6-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="b7de6-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b7de6-128">Request body</span></span>
<span data-ttu-id="b7de6-129">В теле запроса укажи имя записной книжки.</span><span class="sxs-lookup"><span data-stu-id="b7de6-129">In the request body, supply a name for the notebook.</span></span> 

<span data-ttu-id="b7de6-130">Имена записных записей должны быть уникальными.</span><span class="sxs-lookup"><span data-stu-id="b7de6-130">Notebook names must be unique.</span></span> <span data-ttu-id="b7de6-131">Имя не может содержать более 128 символов или содержать следующие символы: ?\* \/ :<>|'"</span><span class="sxs-lookup"><span data-stu-id="b7de6-131">The name cannot contain more than 128 characters or contain the following characters:  ?\*\/:<>|'"</span></span>

## <a name="response"></a><span data-ttu-id="b7de6-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7de6-132">Response</span></span>

<span data-ttu-id="b7de6-133">В случае успешной работы этот метод возвращает код отклика и новый объект `201 Created` [записной](../resources/notebook.md) книжки в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b7de6-133">If successful, this method returns a `201 Created` response code and the new [notebook](../resources/notebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7de6-134">Пример</span><span class="sxs-lookup"><span data-stu-id="b7de6-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="b7de6-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7de6-135">Request</span></span>
<span data-ttu-id="b7de6-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7de6-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_notebook_from_onenote"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks
Content-type: application/json

{
    "displayName": "My Private notebook"
}
```

### <a name="response"></a><span data-ttu-id="b7de6-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7de6-137">Response</span></span>
<span data-ttu-id="b7de6-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7de6-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('7d54cb02-aaa3-4016-9f9c-a4b49422dd9b')/onenote/notebooks/$entity",
    "id": "1-10143016-70dc-4449-b92a-3015225f800d",
    "self": "https://graph.microsoft.com/v1.0/users/7d54cb02-aaa3-4016-9f9c-a4b49422dd9b/onenote/notebooks/1-10143016-70dc-4449-b92a-3015225f800d",
    "displayName": "My Private notebook",
    "userRole": "Owner",
    "isShared": false,
    "sectionsUrl": "https://graph.microsoft.com/v1.0/users/7d54cb02-aaa3-4016-9f9c-a4b49422dd9b/onenote/notebooks/1-10143016-70dc-4449-b92a-3015225f800d/sections",
    "sectionGroupsUrl": "https://graph.microsoft.com/v1.0/users/7d54cb02-aaa3-4016-9f9c-a4b49422dd9b/onenote/notebooks/1-10143016-70dc-4449-b92a-3015225f800d/sectionGroups",
    "links": {
        "oneNoteClientUrl": {
            "href": "onenote:https://contoso-my.sharepoint.com/personal/admin_m365x841051_onmicrosoft_com/Documents/Notebooks/My%20Private%20notebook"
        },
        "oneNoteWebUrl": {
            "href": "https://contoso-my.sharepoint.com/personal/admin_m365x841051_onmicrosoft_com/Documents/Notebooks/My%20Private%20notebook"
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
  "tocPath": "",
  "suppressions": [
  ]
}-->

