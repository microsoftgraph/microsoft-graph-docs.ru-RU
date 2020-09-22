---
title: Обновление Синчронизатионтемплате
description: Update (переопределить) шаблон синхронизации, связанный с заданным приложением.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 10d7792306750d82e19e01f0f1089d5693395977
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087847"
---
# <a name="update-synchronizationtemplate"></a><span data-ttu-id="121ec-103">Обновление Синчронизатионтемплате</span><span class="sxs-lookup"><span data-stu-id="121ec-103">Update synchronizationTemplate</span></span>

<span data-ttu-id="121ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="121ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="121ec-105">Update (переопределить) шаблон синхронизации, связанный с заданным приложением.</span><span class="sxs-lookup"><span data-stu-id="121ec-105">Update (override) the synchronization template associated with a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="121ec-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="121ec-106">Permissions</span></span>
<span data-ttu-id="121ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="121ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="121ec-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="121ec-109">Permission type</span></span>                        | <span data-ttu-id="121ec-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="121ec-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="121ec-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="121ec-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="121ec-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="121ec-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="121ec-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="121ec-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="121ec-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="121ec-114">Not supported.</span></span>|
|<span data-ttu-id="121ec-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="121ec-115">Application</span></span>                            |<span data-ttu-id="121ec-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="121ec-116">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="121ec-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="121ec-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH application/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="121ec-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="121ec-118">Request headers</span></span>

| <span data-ttu-id="121ec-119">Имя</span><span class="sxs-lookup"><span data-stu-id="121ec-119">Name</span></span>           | <span data-ttu-id="121ec-120">Тип</span><span class="sxs-lookup"><span data-stu-id="121ec-120">Type</span></span>    | <span data-ttu-id="121ec-121">Описание</span><span class="sxs-lookup"><span data-stu-id="121ec-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="121ec-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="121ec-122">Authorization</span></span>  | <span data-ttu-id="121ec-123">string</span><span class="sxs-lookup"><span data-stu-id="121ec-123">string</span></span>  | <span data-ttu-id="121ec-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="121ec-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="121ec-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="121ec-126">Request body</span></span>

<span data-ttu-id="121ec-127">В теле запроса добавьте объект [синчронизатионтемплате](../resources/synchronization-synchronizationtemplate.md) для замены существующего шаблона.</span><span class="sxs-lookup"><span data-stu-id="121ec-127">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to replace the existing template.</span></span> <span data-ttu-id="121ec-128">Убедитесь, что все свойства предоставлены.</span><span class="sxs-lookup"><span data-stu-id="121ec-128">Make sure all properties are provided.</span></span> <span data-ttu-id="121ec-129">Отсутствующие свойства будут удалены.</span><span class="sxs-lookup"><span data-stu-id="121ec-129">Missing properties will be erased.</span></span>

### <a name="response"></a><span data-ttu-id="121ec-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="121ec-130">Response</span></span>

<span data-ttu-id="121ec-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="121ec-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="examples"></a><span data-ttu-id="121ec-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="121ec-133">Examples</span></span>

##### <a name="request"></a><span data-ttu-id="121ec-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="121ec-134">Request</span></span>
<span data-ttu-id="121ec-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="121ec-135">The following is an example of a request.</span></span> 

><span data-ttu-id="121ec-136">**Примечание:** Объект Request, показанный здесь, сокращается для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="121ec-136">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="121ec-137">Включает все свойства в фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="121ec-137">Include all the properties in an actual call.</span></span>

# <a name="http"></a>[<span data-ttu-id="121ec-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="121ec-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="121ec-139">C#</span><span class="sxs-lookup"><span data-stu-id="121ec-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-synchronizationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="121ec-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="121ec-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-synchronizationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="121ec-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="121ec-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-synchronizationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="121ec-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="121ec-142">Response</span></span>
<span data-ttu-id="121ec-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="121ec-143">The following is an example of a response.</span></span>
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


