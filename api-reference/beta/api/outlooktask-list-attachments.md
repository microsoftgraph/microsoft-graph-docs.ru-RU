---
title: Список вложений
description: Получение списка объектов вложений, вложенных в задачу Outlook.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0f8e0b76f84cbacee562493937998ebfbc6423f6
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459020"
---
# <a name="list-attachments-deprecated"></a><span data-ttu-id="8e061-103">Список вложений (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="8e061-103">List attachments (deprecated)</span></span>

<span data-ttu-id="8e061-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e061-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="8e061-105">Получение списка объектов [вложений](../resources/attachment.md) , вложенных в задачу Outlook.</span><span class="sxs-lookup"><span data-stu-id="8e061-105">Get a list of [attachment](../resources/attachment.md) objects attached to an Outlook task.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e061-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e061-106">Permissions</span></span>

<span data-ttu-id="8e061-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e061-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e061-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e061-109">Permission type</span></span>      | <span data-ttu-id="8e061-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e061-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e061-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e061-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8e061-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="8e061-112">Tasks.Read</span></span>    |
|<span data-ttu-id="8e061-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e061-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e061-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="8e061-114">Tasks.Read</span></span>    |
|<span data-ttu-id="8e061-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e061-115">Application</span></span> | <span data-ttu-id="8e061-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e061-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e061-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e061-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}/attachments
GET /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8e061-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8e061-118">Optional query parameters</span></span>

<span data-ttu-id="8e061-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8e061-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e061-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e061-120">Request headers</span></span>

| <span data-ttu-id="8e061-121">Имя</span><span class="sxs-lookup"><span data-stu-id="8e061-121">Name</span></span>      |<span data-ttu-id="8e061-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8e061-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8e061-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e061-123">Authorization</span></span>  | <span data-ttu-id="8e061-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e061-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e061-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e061-126">Request body</span></span>

<span data-ttu-id="8e061-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8e061-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e061-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e061-128">Response</span></span>

<span data-ttu-id="8e061-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [вложений](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8e061-129">If successful, this method returns a `200 OK` response code and collection of [attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e061-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8e061-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e061-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e061-131">Request</span></span>

<span data-ttu-id="8e061-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e061-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8e061-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e061-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "outlook_task_get_attachments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/outlook/tasks/{id}/attachments
```
# <a name="c"></a>[<span data-ttu-id="8e061-134">C#</span><span class="sxs-lookup"><span data-stu-id="8e061-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/outlook-task-get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e061-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e061-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/outlook-task-get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e061-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e061-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/outlook-task-get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8e061-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e061-137">Response</span></span>

<span data-ttu-id="8e061-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e061-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
