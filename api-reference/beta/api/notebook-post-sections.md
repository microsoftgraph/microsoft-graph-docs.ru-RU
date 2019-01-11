---
title: Создание раздела
description: Создание раздела в указанной записной книжке.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: c6c091d399ae2b9fc69d249a3e2a34f3051c1611
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892465"
---
# <a name="create-section"></a><span data-ttu-id="368be-103">Создание раздела</span><span class="sxs-lookup"><span data-stu-id="368be-103">Create section</span></span>

> <span data-ttu-id="368be-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="368be-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="368be-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="368be-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="368be-106">Создание [раздела](../resources/section.md) в указанной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="368be-106">Create a new [section](../resources/section.md) in the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="368be-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="368be-107">Permissions</span></span>
<span data-ttu-id="368be-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="368be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="368be-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="368be-110">Permission type</span></span>      | <span data-ttu-id="368be-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="368be-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="368be-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="368be-112">Delegated (work or school account)</span></span> | <span data-ttu-id="368be-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="368be-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="368be-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="368be-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="368be-115">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="368be-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="368be-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="368be-116">Application</span></span> | <span data-ttu-id="368be-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="368be-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="368be-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="368be-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/sections
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/sections
POST /groups/{id}/onenote/notebooks/{id}/sections
POST /sites/{id}/onenote/notebooks/{id}/sections
```
## <a name="request-headers"></a><span data-ttu-id="368be-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="368be-119">Request headers</span></span>
| <span data-ttu-id="368be-120">Имя</span><span class="sxs-lookup"><span data-stu-id="368be-120">Name</span></span>       | <span data-ttu-id="368be-121">Тип</span><span class="sxs-lookup"><span data-stu-id="368be-121">Type</span></span> | <span data-ttu-id="368be-122">Описание</span><span class="sxs-lookup"><span data-stu-id="368be-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="368be-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="368be-123">Authorization</span></span>  | <span data-ttu-id="368be-124">string</span><span class="sxs-lookup"><span data-stu-id="368be-124">string</span></span>  | <span data-ttu-id="368be-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="368be-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="368be-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="368be-127">Content-Type</span></span> | <span data-ttu-id="368be-128">string</span><span class="sxs-lookup"><span data-stu-id="368be-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="368be-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="368be-129">Request body</span></span>
<span data-ttu-id="368be-130">В тексте запроса укажите имя раздела.</span><span class="sxs-lookup"><span data-stu-id="368be-130">In the request body, supply a name for the section.</span></span>

<span data-ttu-id="368be-p104">В рамках одного и того же уровня иерархии имена разделов должны быть уникальными. Имя должно содержать не более 50 символов, в нем не должно быть следующих знаков:  ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="368be-p104">Within the same hierarchy level, section names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="368be-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="368be-133">Response</span></span>

<span data-ttu-id="368be-134">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [section](../resources/section.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="368be-134">If successful, this method returns a `201 Created` response code and a [section](../resources/section.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="368be-135">Пример</span><span class="sxs-lookup"><span data-stu-id="368be-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="368be-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="368be-136">Request</span></span>
<span data-ttu-id="368be-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="368be-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_section_from_notebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/sections
Content-type: application/json
Content-length: 27

{
  "displayName": "Section name"
}
```
##### <a name="response"></a><span data-ttu-id="368be-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="368be-138">Response</span></span>
<span data-ttu-id="368be-p105">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="368be-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 272

{
  "isDefault": true,
  "pagesUrl": "pagesUrl-value",
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
  "description": "Create Section",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
