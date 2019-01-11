---
title: Обновление фотографии
description: Обновление свойств объекта фотографии.
localization_priority: Normal
ms.openlocfilehash: 80c866eab74307d3001887110e050aa438cdde9f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883785"
---
# <a name="update-photo"></a><span data-ttu-id="6c67c-103">Обновление фотографии</span><span class="sxs-lookup"><span data-stu-id="6c67c-103">Update photo</span></span>

<span data-ttu-id="6c67c-104">Обновление свойств объекта фотографии.</span><span class="sxs-lookup"><span data-stu-id="6c67c-104">Update the properties of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6c67c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c67c-105">Permissions</span></span>
<span data-ttu-id="6c67c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c67c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c67c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c67c-108">Permission type</span></span>      | <span data-ttu-id="6c67c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c67c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c67c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c67c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6c67c-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c67c-111">Not supported.</span></span>    |
|<span data-ttu-id="6c67c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c67c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c67c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c67c-113">Not supported.</span></span>    |
|<span data-ttu-id="6c67c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c67c-114">Application</span></span> | <span data-ttu-id="6c67c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c67c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c67c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c67c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="6c67c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c67c-117">Request headers</span></span>
| <span data-ttu-id="6c67c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="6c67c-118">Name</span></span>       | <span data-ttu-id="6c67c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="6c67c-119">Type</span></span> | <span data-ttu-id="6c67c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6c67c-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6c67c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c67c-121">Authorization</span></span>  | <span data-ttu-id="6c67c-122">string</span><span class="sxs-lookup"><span data-stu-id="6c67c-122">string</span></span>  | <span data-ttu-id="6c67c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c67c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c67c-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6c67c-125">Request body</span></span>
<span data-ttu-id="6c67c-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="6c67c-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6c67c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c67c-129">Property</span></span>     | <span data-ttu-id="6c67c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6c67c-130">Type</span></span>   |<span data-ttu-id="6c67c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6c67c-131">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="6c67c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c67c-132">Response</span></span>

<span data-ttu-id="6c67c-133">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [photo](../resources/photo.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6c67c-133">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6c67c-134">Пример</span><span class="sxs-lookup"><span data-stu-id="6c67c-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6c67c-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c67c-135">Request</span></span>
<span data-ttu-id="6c67c-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c67c-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_photo"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
##### <a name="response"></a><span data-ttu-id="6c67c-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="6c67c-137">Response</span></span>
<span data-ttu-id="6c67c-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6c67c-138">Here is an example of the response.</span></span>
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
