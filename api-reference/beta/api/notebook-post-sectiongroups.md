---
title: Создание sectionGroup
description: Создание группы разделов в указанной записной книжке.
author: Jewan-microsoft
ms.openlocfilehash: 7bdf81023cea5738ac434add597124151740a6e0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360251"
---
# <a name="create-sectiongroup"></a><span data-ttu-id="bcfde-103">Создание sectionGroup</span><span class="sxs-lookup"><span data-stu-id="bcfde-103">Create sectionGroup</span></span>

> <span data-ttu-id="bcfde-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bcfde-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bcfde-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcfde-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bcfde-106">Создание [группы разделов](../resources/sectiongroup.md) в указанной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="bcfde-106">Create a new [section group](../resources/sectiongroup.md) in the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="bcfde-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bcfde-107">Permissions</span></span>
<span data-ttu-id="bcfde-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcfde-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcfde-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcfde-110">Permission type</span></span>      | <span data-ttu-id="bcfde-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcfde-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcfde-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcfde-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bcfde-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcfde-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="bcfde-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcfde-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcfde-115">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bcfde-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="bcfde-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bcfde-116">Application</span></span> | <span data-ttu-id="bcfde-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcfde-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcfde-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcfde-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/sectionGroups
POST /groups/{id}/onenote/notebooks/{id}/sectionGroups
POST /sites/{id}/onenote/notebooks/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="bcfde-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bcfde-119">Request headers</span></span>
| <span data-ttu-id="bcfde-120">Имя</span><span class="sxs-lookup"><span data-stu-id="bcfde-120">Name</span></span>       | <span data-ttu-id="bcfde-121">Тип</span><span class="sxs-lookup"><span data-stu-id="bcfde-121">Type</span></span> | <span data-ttu-id="bcfde-122">Описание</span><span class="sxs-lookup"><span data-stu-id="bcfde-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bcfde-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcfde-123">Authorization</span></span>  | <span data-ttu-id="bcfde-124">string</span><span class="sxs-lookup"><span data-stu-id="bcfde-124">string</span></span>  | <span data-ttu-id="bcfde-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bcfde-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bcfde-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bcfde-127">Content-Type</span></span> | <span data-ttu-id="bcfde-128">string</span><span class="sxs-lookup"><span data-stu-id="bcfde-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="bcfde-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bcfde-129">Request body</span></span>
<span data-ttu-id="bcfde-130">В теле запроса укажите имя группы разделов.</span><span class="sxs-lookup"><span data-stu-id="bcfde-130">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="bcfde-p104">В рамках одного и того же уровня иерархии имя каждой группы разделов должно быть уникальным. Имя должно содержать не более 50 символов, в нем не должно быть следующих знаков:  ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="bcfde-p104">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="bcfde-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcfde-133">Response</span></span>

<span data-ttu-id="bcfde-134">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [sectionGroup](../resources/sectiongroup.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bcfde-134">If successful, this method returns `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcfde-135">Пример</span><span class="sxs-lookup"><span data-stu-id="bcfde-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bcfde-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcfde-136">Request</span></span>
<span data-ttu-id="bcfde-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bcfde-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_sectiongroup_from_notebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/sectionGroups
Content-type: application/json
Content-length: 30

{
  "displayName": "Section group name"
}
```

##### <a name="response"></a><span data-ttu-id="bcfde-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcfde-138">Response</span></span>
<span data-ttu-id="bcfde-p105">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bcfde-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
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
