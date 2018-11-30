---
title: Обновление фотографии
description: Обновление свойств объекта фотографии.
ms.openlocfilehash: 8071c9e331f9af72c9a288239206f396d9ad3fcb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075088"
---
# <a name="update-photo"></a><span data-ttu-id="0d842-103">Обновление фотографии</span><span class="sxs-lookup"><span data-stu-id="0d842-103">Update photo</span></span>

> <span data-ttu-id="0d842-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0d842-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d842-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d842-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0d842-106">Обновление свойств объекта фотографии.</span><span class="sxs-lookup"><span data-stu-id="0d842-106">Update the properties of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0d842-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0d842-107">Permissions</span></span>
<span data-ttu-id="0d842-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d842-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d842-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d842-110">Permission type</span></span>      | <span data-ttu-id="0d842-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d842-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d842-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d842-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0d842-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d842-113">Not supported.</span></span>    |
|<span data-ttu-id="0d842-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d842-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d842-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d842-115">Not supported.</span></span>    |
|<span data-ttu-id="0d842-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d842-116">Application</span></span> | <span data-ttu-id="0d842-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d842-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d842-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d842-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="0d842-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d842-119">Request headers</span></span>
| <span data-ttu-id="0d842-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0d842-120">Name</span></span>       | <span data-ttu-id="0d842-121">Тип</span><span class="sxs-lookup"><span data-stu-id="0d842-121">Type</span></span> | <span data-ttu-id="0d842-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0d842-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0d842-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d842-123">Authorization</span></span>  | <span data-ttu-id="0d842-124">string</span><span class="sxs-lookup"><span data-stu-id="0d842-124">string</span></span>  | <span data-ttu-id="0d842-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d842-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d842-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d842-127">Request body</span></span>
<span data-ttu-id="0d842-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0d842-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0d842-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d842-131">Property</span></span>     | <span data-ttu-id="0d842-132">Тип</span><span class="sxs-lookup"><span data-stu-id="0d842-132">Type</span></span>   |<span data-ttu-id="0d842-133">Описание</span><span class="sxs-lookup"><span data-stu-id="0d842-133">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="0d842-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d842-134">Response</span></span>

<span data-ttu-id="0d842-135">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [photo](../resources/photo.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0d842-135">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0d842-136">Пример</span><span class="sxs-lookup"><span data-stu-id="0d842-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0d842-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d842-137">Request</span></span>
<span data-ttu-id="0d842-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d842-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_photo"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
##### <a name="response"></a><span data-ttu-id="0d842-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d842-139">Response</span></span>
<span data-ttu-id="0d842-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0d842-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
