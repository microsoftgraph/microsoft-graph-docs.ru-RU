---
title: Обновление фотографии
description: Обновление свойств объекта фотографии.
localization_priority: Normal
ms.openlocfilehash: 56a8d892ae92f92f5103dc3d88a2f95a5bbb262b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818384"
---
# <a name="update-photo"></a><span data-ttu-id="d762a-103">Обновление фотографии</span><span class="sxs-lookup"><span data-stu-id="d762a-103">Update photo</span></span>

> <span data-ttu-id="d762a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d762a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d762a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d762a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d762a-106">Обновление свойств объекта фотографии.</span><span class="sxs-lookup"><span data-stu-id="d762a-106">Update the properties of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d762a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d762a-107">Permissions</span></span>
<span data-ttu-id="d762a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d762a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d762a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d762a-110">Permission type</span></span>      | <span data-ttu-id="d762a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d762a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d762a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d762a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d762a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d762a-113">Not supported.</span></span>    |
|<span data-ttu-id="d762a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d762a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d762a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d762a-115">Not supported.</span></span>    |
|<span data-ttu-id="d762a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d762a-116">Application</span></span> | <span data-ttu-id="d762a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d762a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d762a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d762a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="d762a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d762a-119">Request headers</span></span>
| <span data-ttu-id="d762a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d762a-120">Name</span></span>       | <span data-ttu-id="d762a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="d762a-121">Type</span></span> | <span data-ttu-id="d762a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d762a-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d762a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d762a-123">Authorization</span></span>  | <span data-ttu-id="d762a-124">string</span><span class="sxs-lookup"><span data-stu-id="d762a-124">string</span></span>  | <span data-ttu-id="d762a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d762a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d762a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d762a-127">Request body</span></span>
<span data-ttu-id="d762a-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d762a-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d762a-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="d762a-131">Property</span></span>     | <span data-ttu-id="d762a-132">Тип</span><span class="sxs-lookup"><span data-stu-id="d762a-132">Type</span></span>   |<span data-ttu-id="d762a-133">Описание</span><span class="sxs-lookup"><span data-stu-id="d762a-133">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="d762a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d762a-134">Response</span></span>

<span data-ttu-id="d762a-135">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [photo](../resources/photo.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d762a-135">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d762a-136">Пример</span><span class="sxs-lookup"><span data-stu-id="d762a-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d762a-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="d762a-137">Request</span></span>
<span data-ttu-id="d762a-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d762a-138">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="d762a-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="d762a-139">Response</span></span>
<span data-ttu-id="d762a-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d762a-140">Here is an example of the response.</span></span>
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
