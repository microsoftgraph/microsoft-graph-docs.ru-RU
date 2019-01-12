---
title: Создание sectionGroup
description: Создание группы разделов в указанной группе разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 2236cdcf832d3fd0ea496c5b4c4634b38803c303
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932968"
---
# <a name="create-sectiongroup"></a><span data-ttu-id="5c8c3-103">Создание sectionGroup</span><span class="sxs-lookup"><span data-stu-id="5c8c3-103">Create sectionGroup</span></span>

> <span data-ttu-id="5c8c3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5c8c3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c8c3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c8c3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5c8c3-106">Создание [группы разделов](../resources/sectiongroup.md) в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="5c8c3-106">Create a new [section group](../resources/sectiongroup.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="5c8c3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5c8c3-107">Permissions</span></span>
<span data-ttu-id="5c8c3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c8c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c8c3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c8c3-110">Permission type</span></span>      | <span data-ttu-id="5c8c3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c8c3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c8c3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c8c3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5c8c3-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c8c3-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="5c8c3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c8c3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c8c3-115">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c8c3-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="5c8c3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c8c3-116">Application</span></span> | <span data-ttu-id="5c8c3-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c8c3-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c8c3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c8c3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
POST /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
POST /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="5c8c3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c8c3-119">Request headers</span></span>
| <span data-ttu-id="5c8c3-120">Имя</span><span class="sxs-lookup"><span data-stu-id="5c8c3-120">Name</span></span>       | <span data-ttu-id="5c8c3-121">Тип</span><span class="sxs-lookup"><span data-stu-id="5c8c3-121">Type</span></span> | <span data-ttu-id="5c8c3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5c8c3-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5c8c3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c8c3-123">Authorization</span></span>  | <span data-ttu-id="5c8c3-124">string</span><span class="sxs-lookup"><span data-stu-id="5c8c3-124">string</span></span>  | <span data-ttu-id="5c8c3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c8c3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5c8c3-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5c8c3-127">Content-Type</span></span> | <span data-ttu-id="5c8c3-128">string</span><span class="sxs-lookup"><span data-stu-id="5c8c3-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="5c8c3-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5c8c3-129">Request body</span></span>
<span data-ttu-id="5c8c3-130">В теле запроса укажите имя группы разделов.</span><span class="sxs-lookup"><span data-stu-id="5c8c3-130">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="5c8c3-p104">В рамках одного и того же уровня иерархии имя каждой группы разделов должно быть уникальным. Имя должно содержать не более 50 символов, в нем не должно быть следующих знаков:  ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="5c8c3-p104">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="5c8c3-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c8c3-133">Response</span></span>

<span data-ttu-id="5c8c3-134">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [sectionGroup](../resources/sectiongroup.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5c8c3-134">If successful, this method returns a `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c8c3-135">Пример</span><span class="sxs-lookup"><span data-stu-id="5c8c3-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c8c3-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c8c3-136">Request</span></span>
<span data-ttu-id="5c8c3-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c8c3-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_sectiongroup_from_sectiongroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}/sectionGroups
Content-type: application/json
Content-length: 30

{
  "displayName": "Section group name"
}
```
##### <a name="response"></a><span data-ttu-id="5c8c3-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c8c3-138">Response</span></span>
<span data-ttu-id="5c8c3-p105">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c8c3-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectiongroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "displayName": "name-value",  
  "createdBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "lastModifiedBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create SectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
