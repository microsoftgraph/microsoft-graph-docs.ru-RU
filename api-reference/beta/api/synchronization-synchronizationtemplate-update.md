---
title: Обновление Синчронизатионтемплате
description: Update (переопределить) шаблон синхронизации, связанный с заданным приложением.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 132bc669122cae84acbd85163c80bb035520a8a8
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409639"
---
# <a name="update-synchronizationtemplate"></a><span data-ttu-id="2a880-103">Обновление Синчронизатионтемплате</span><span class="sxs-lookup"><span data-stu-id="2a880-103">Update synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a880-104">Update (переопределить) шаблон синхронизации, связанный с заданным приложением.</span><span class="sxs-lookup"><span data-stu-id="2a880-104">Update (override) the synchronization template associated with a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a880-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a880-105">Permissions</span></span>
<span data-ttu-id="2a880-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a880-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a880-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a880-108">Permission type</span></span>                        | <span data-ttu-id="2a880-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a880-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a880-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a880-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="2a880-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a880-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="2a880-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a880-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="2a880-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a880-113">Not supported.</span></span>|
|<span data-ttu-id="2a880-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a880-114">Application</span></span>                            |<span data-ttu-id="2a880-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a880-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="2a880-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a880-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT application/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="2a880-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a880-117">Request headers</span></span>

| <span data-ttu-id="2a880-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2a880-118">Name</span></span>           | <span data-ttu-id="2a880-119">Тип</span><span class="sxs-lookup"><span data-stu-id="2a880-119">Type</span></span>    | <span data-ttu-id="2a880-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2a880-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="2a880-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a880-121">Authorization</span></span>  | <span data-ttu-id="2a880-122">string</span><span class="sxs-lookup"><span data-stu-id="2a880-122">string</span></span>  | <span data-ttu-id="2a880-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a880-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a880-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2a880-125">Request body</span></span>

<span data-ttu-id="2a880-126">В теле запроса добавьте объект [синчронизатионтемплате](../resources/synchronization-synchronizationtemplate.md) для замены существующего шаблона.</span><span class="sxs-lookup"><span data-stu-id="2a880-126">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to replace the existing template.</span></span> <span data-ttu-id="2a880-127">Убедитесь, что все свойства предоставлены.</span><span class="sxs-lookup"><span data-stu-id="2a880-127">Make sure all properties are provided.</span></span> <span data-ttu-id="2a880-128">Отсутствующие свойства будут удалены.</span><span class="sxs-lookup"><span data-stu-id="2a880-128">Missing properties will be erased.</span></span>

### <a name="response"></a><span data-ttu-id="2a880-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a880-129">Response</span></span>

<span data-ttu-id="2a880-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2a880-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="examples"></a><span data-ttu-id="2a880-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="2a880-132">Examples</span></span>

##### <a name="request"></a><span data-ttu-id="2a880-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a880-133">Request</span></span>
<span data-ttu-id="2a880-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a880-134">The following is an example of a request.</span></span> 

><span data-ttu-id="2a880-135">**Примечание:** Объект Request, показанный здесь, сокращается для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2a880-135">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="2a880-136">Включает все свойства в фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2a880-136">Include all the properties in an actual call.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2a880-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a880-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_synchronizationtemplate"
}-->
```http
PUT https://graph.microsoft.com/beta/applications/{id}/synchronization/templates/{templateId}
Authorization: Bearer <token>
Content-type: application/json

{
    "id": "Slack",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2a880-138">C#</span><span class="sxs-lookup"><span data-stu-id="2a880-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-synchronizationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2a880-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a880-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-synchronizationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2a880-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2a880-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-synchronizationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2a880-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a880-141">Response</span></span>
<span data-ttu-id="2a880-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2a880-142">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update synchronizationtemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
