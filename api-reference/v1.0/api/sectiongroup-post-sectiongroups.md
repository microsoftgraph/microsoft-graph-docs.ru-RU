---
title: Создание sectionGroup
description: Создание группы разделов в указанной группе разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: a05e61934c8043c0c6a94c6e0785c0e93e4a3e19
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987113"
---
# <a name="create-sectiongroup"></a><span data-ttu-id="654cc-103">Создание sectionGroup</span><span class="sxs-lookup"><span data-stu-id="654cc-103">Create sectionGroup</span></span>

<span data-ttu-id="654cc-104">Создание [группы разделов](../resources/sectiongroup.md) в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="654cc-104">Create a new [section group](../resources/sectiongroup.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="654cc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="654cc-105">Permissions</span></span>
<span data-ttu-id="654cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="654cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="654cc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="654cc-108">Permission type</span></span>      | <span data-ttu-id="654cc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="654cc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="654cc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="654cc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="654cc-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="654cc-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="654cc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="654cc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="654cc-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="654cc-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="654cc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="654cc-114">Application</span></span> | <span data-ttu-id="654cc-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="654cc-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="654cc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="654cc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
POST /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
POST /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="654cc-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="654cc-117">Request headers</span></span>
| <span data-ttu-id="654cc-118">Имя</span><span class="sxs-lookup"><span data-stu-id="654cc-118">Name</span></span>       | <span data-ttu-id="654cc-119">Тип</span><span class="sxs-lookup"><span data-stu-id="654cc-119">Type</span></span> | <span data-ttu-id="654cc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="654cc-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="654cc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="654cc-121">Authorization</span></span>  | <span data-ttu-id="654cc-122">строка</span><span class="sxs-lookup"><span data-stu-id="654cc-122">string</span></span>  | <span data-ttu-id="654cc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="654cc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="654cc-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="654cc-125">Content-Type</span></span> | <span data-ttu-id="654cc-126">строка</span><span class="sxs-lookup"><span data-stu-id="654cc-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="654cc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="654cc-127">Request body</span></span>
<span data-ttu-id="654cc-128">В теле запроса укажите имя группы разделов.</span><span class="sxs-lookup"><span data-stu-id="654cc-128">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="654cc-p103">В рамках одного и того же уровня иерархии имя каждой группы разделов должно быть уникальным. Имя должно содержать не более 50 символов, в нем не должно быть следующих знаков:  ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="654cc-p103">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="654cc-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="654cc-131">Response</span></span>

<span data-ttu-id="654cc-132">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [sectionGroup](../resources/sectiongroup.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="654cc-132">If successful, this method returns a `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="654cc-133">Пример</span><span class="sxs-lookup"><span data-stu-id="654cc-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="654cc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="654cc-134">Request</span></span>
<span data-ttu-id="654cc-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="654cc-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_sectiongroup_from_sectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}/sectionGroups
Content-type: application/json
Content-length: 30

{
  "displayName": "Section group name"
}
```
##### <a name="response"></a><span data-ttu-id="654cc-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="654cc-136">Response</span></span>
<span data-ttu-id="654cc-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="654cc-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectionGroup"
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
