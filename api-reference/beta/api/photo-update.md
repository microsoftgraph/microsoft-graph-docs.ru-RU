---
title: Обновление фотографии
description: Обновление свойств объекта фотографии.
localization_priority: Normal
ms.openlocfilehash: f9e64aed22308736ff08d6297a9f8823aa7e2de1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332594"
---
# <a name="update-photo"></a><span data-ttu-id="2105a-103">Обновление фотографии</span><span class="sxs-lookup"><span data-stu-id="2105a-103">Update photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2105a-104">Обновление свойств объекта фотографии.</span><span class="sxs-lookup"><span data-stu-id="2105a-104">Update the properties of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2105a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2105a-105">Permissions</span></span>
<span data-ttu-id="2105a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2105a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2105a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2105a-108">Permission type</span></span>      | <span data-ttu-id="2105a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2105a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2105a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2105a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2105a-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2105a-111">Not supported.</span></span>    |
|<span data-ttu-id="2105a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2105a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2105a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2105a-113">Not supported.</span></span>    |
|<span data-ttu-id="2105a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2105a-114">Application</span></span> | <span data-ttu-id="2105a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2105a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2105a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2105a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="2105a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2105a-117">Request headers</span></span>
| <span data-ttu-id="2105a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2105a-118">Name</span></span>       | <span data-ttu-id="2105a-119">Тип</span><span class="sxs-lookup"><span data-stu-id="2105a-119">Type</span></span> | <span data-ttu-id="2105a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2105a-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2105a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2105a-121">Authorization</span></span>  | <span data-ttu-id="2105a-122">string</span><span class="sxs-lookup"><span data-stu-id="2105a-122">string</span></span>  | <span data-ttu-id="2105a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2105a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2105a-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2105a-125">Request body</span></span>
<span data-ttu-id="2105a-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="2105a-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2105a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2105a-129">Property</span></span>     | <span data-ttu-id="2105a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2105a-130">Type</span></span>   |<span data-ttu-id="2105a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2105a-131">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="2105a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="2105a-132">Response</span></span>

<span data-ttu-id="2105a-133">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [photo](../resources/photo.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2105a-133">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2105a-134">Пример</span><span class="sxs-lookup"><span data-stu-id="2105a-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2105a-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="2105a-135">Request</span></span>
<span data-ttu-id="2105a-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2105a-136">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="2105a-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2105a-137">Response</span></span>
<span data-ttu-id="2105a-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2105a-138">Here is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
