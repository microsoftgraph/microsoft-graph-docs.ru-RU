---
title: Список вложений
description: Получение списка объектов вложений, вложенных в задачу Outlook.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 13c989da0a0553f3991abf9fd0aa8fd4159d9da6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43413754"
---
# <a name="list-attachments"></a><span data-ttu-id="0d30e-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="0d30e-103">List attachments</span></span>

<span data-ttu-id="0d30e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d30e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d30e-105">Получение списка объектов [вложений](../resources/attachment.md) , вложенных в задачу Outlook.</span><span class="sxs-lookup"><span data-stu-id="0d30e-105">Get a list of [attachment](../resources/attachment.md) objects attached to an Outlook task.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d30e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0d30e-106">Permissions</span></span>

<span data-ttu-id="0d30e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d30e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d30e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d30e-109">Permission type</span></span>      | <span data-ttu-id="0d30e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d30e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d30e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d30e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0d30e-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="0d30e-112">Tasks.Read</span></span>    |
|<span data-ttu-id="0d30e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d30e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d30e-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="0d30e-114">Tasks.Read</span></span>    |
|<span data-ttu-id="0d30e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d30e-115">Application</span></span> | <span data-ttu-id="0d30e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d30e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d30e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d30e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}/attachments
GET /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0d30e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0d30e-118">Optional query parameters</span></span>

<span data-ttu-id="0d30e-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0d30e-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0d30e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d30e-120">Request headers</span></span>

| <span data-ttu-id="0d30e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0d30e-121">Name</span></span>      |<span data-ttu-id="0d30e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0d30e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0d30e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0d30e-123">Authorization</span></span>  | <span data-ttu-id="0d30e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d30e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d30e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d30e-126">Request body</span></span>

<span data-ttu-id="0d30e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0d30e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d30e-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d30e-128">Response</span></span>

<span data-ttu-id="0d30e-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [вложений](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0d30e-129">If successful, this method returns a `200 OK` response code and collection of [attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d30e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0d30e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d30e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d30e-131">Request</span></span>

<span data-ttu-id="0d30e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d30e-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0d30e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d30e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "outlook_task_get_attachments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/outlook/tasks/{id}/attachments
```
# <a name="c"></a>[<span data-ttu-id="0d30e-134">C#</span><span class="sxs-lookup"><span data-stu-id="0d30e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/outlook-task-get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d30e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d30e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/outlook-task-get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d30e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d30e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/outlook-task-get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0d30e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d30e-137">Response</span></span>

<span data-ttu-id="0d30e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0d30e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "lastModifiedDateTime": "datetime-value",
      "name": "name-value",
      "contentType": "contentType-value",
      "size": 99,
      "isInline": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
