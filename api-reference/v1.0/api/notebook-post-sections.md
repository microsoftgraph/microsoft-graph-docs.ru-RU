---
title: Создание раздела
description: Создание нового onenoteSection в указанном записной книжки.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: cec39a64f7405d13efacb1080c5d6c1482dceabb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942495"
---
# <a name="create-section"></a><span data-ttu-id="03b59-103">Создание раздела</span><span class="sxs-lookup"><span data-stu-id="03b59-103">Create section</span></span>

<span data-ttu-id="03b59-104">Создание нового [onenoteSection](../resources/section.md) в указанном записной книжки.</span><span class="sxs-lookup"><span data-stu-id="03b59-104">Create a new [onenoteSection](../resources/section.md) in the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="03b59-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03b59-105">Permissions</span></span>
<span data-ttu-id="03b59-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03b59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03b59-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03b59-108">Permission type</span></span>      | <span data-ttu-id="03b59-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03b59-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03b59-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03b59-110">Delegated (work or school account)</span></span> | <span data-ttu-id="03b59-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03b59-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="03b59-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03b59-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03b59-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03b59-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="03b59-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03b59-114">Application</span></span> | <span data-ttu-id="03b59-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03b59-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="03b59-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03b59-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/sections
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/sections
POST /groups/{id}/onenote/notebooks/{id}/sections
POST /sites/{id}/onenote/notebooks/{id}/sections
```
## <a name="request-headers"></a><span data-ttu-id="03b59-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03b59-117">Request headers</span></span>
| <span data-ttu-id="03b59-118">Имя</span><span class="sxs-lookup"><span data-stu-id="03b59-118">Name</span></span>       | <span data-ttu-id="03b59-119">Тип</span><span class="sxs-lookup"><span data-stu-id="03b59-119">Type</span></span> | <span data-ttu-id="03b59-120">Описание</span><span class="sxs-lookup"><span data-stu-id="03b59-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="03b59-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="03b59-121">Authorization</span></span>  | <span data-ttu-id="03b59-122">string</span><span class="sxs-lookup"><span data-stu-id="03b59-122">string</span></span>  | <span data-ttu-id="03b59-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03b59-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="03b59-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="03b59-125">Content-Type</span></span> | <span data-ttu-id="03b59-126">string</span><span class="sxs-lookup"><span data-stu-id="03b59-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="03b59-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="03b59-127">Request body</span></span>
<span data-ttu-id="03b59-128">В тексте запроса укажите имя раздела.</span><span class="sxs-lookup"><span data-stu-id="03b59-128">In the request body, supply a name for the section.</span></span>

<span data-ttu-id="03b59-p103">В рамках одного и того же уровня иерархии имена разделов должны быть уникальными. Имя должно содержать не более 50 символов, в нем не должно быть следующих знаков:  ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="03b59-p103">Within the same hierarchy level, section names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="03b59-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="03b59-131">Response</span></span>

<span data-ttu-id="03b59-132">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [onenoteSection](../resources/section.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="03b59-132">If successful, this method returns a `201 Created` response code and a [onenoteSection](../resources/section.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03b59-133">Пример</span><span class="sxs-lookup"><span data-stu-id="03b59-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03b59-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="03b59-134">Request</span></span>
<span data-ttu-id="03b59-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03b59-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_section_from_notebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections
Content-type: application/json
Content-length: 27

{
  "displayName": "Section name"
}
```
##### <a name="response"></a><span data-ttu-id="03b59-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="03b59-136">Response</span></span>
<span data-ttu-id="03b59-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03b59-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 272

{
  "isDefault": true,
  "pagesUrl": "pagesUrl-value",
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
  "description": "Create Section",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
