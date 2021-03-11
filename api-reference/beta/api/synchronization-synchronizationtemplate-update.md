---
title: Обновление синхронизацииTemplate
description: Обновление (переопределение) шаблона синхронизации, связанного с заданным приложением.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 133f503ee6361619581cea058fbf3a47a8c7de01
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722024"
---
# <a name="update-synchronizationtemplate"></a><span data-ttu-id="d0d09-103">Обновление синхронизацииTemplate</span><span class="sxs-lookup"><span data-stu-id="d0d09-103">Update synchronizationTemplate</span></span>

<span data-ttu-id="d0d09-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0d09-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0d09-105">Обновление (переопределение) шаблона синхронизации, связанного с заданным приложением.</span><span class="sxs-lookup"><span data-stu-id="d0d09-105">Update (override) the synchronization template associated with a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0d09-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d0d09-106">Permissions</span></span>
<span data-ttu-id="d0d09-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0d09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0d09-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0d09-109">Permission type</span></span>                        | <span data-ttu-id="d0d09-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0d09-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0d09-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0d09-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="d0d09-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0d09-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="d0d09-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0d09-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="d0d09-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0d09-114">Not supported.</span></span>|
|<span data-ttu-id="d0d09-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0d09-115">Application</span></span>                            |<span data-ttu-id="d0d09-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0d09-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

### <a name="http-request"></a><span data-ttu-id="d0d09-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0d09-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH applications/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="d0d09-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d0d09-118">Request headers</span></span>

| <span data-ttu-id="d0d09-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d0d09-119">Name</span></span>           | <span data-ttu-id="d0d09-120">Тип</span><span class="sxs-lookup"><span data-stu-id="d0d09-120">Type</span></span>    | <span data-ttu-id="d0d09-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d0d09-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="d0d09-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0d09-122">Authorization</span></span>  | <span data-ttu-id="d0d09-123">string</span><span class="sxs-lookup"><span data-stu-id="d0d09-123">string</span></span>  | <span data-ttu-id="d0d09-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0d09-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0d09-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d0d09-126">Request body</span></span>

<span data-ttu-id="d0d09-127">В теле запроса поставляем объект [синхронизацииTemplate](../resources/synchronization-synchronizationtemplate.md) для замены существующего шаблона.</span><span class="sxs-lookup"><span data-stu-id="d0d09-127">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to replace the existing template.</span></span> <span data-ttu-id="d0d09-128">Убедитесь, что все свойства предоставлены.</span><span class="sxs-lookup"><span data-stu-id="d0d09-128">Make sure all properties are provided.</span></span> <span data-ttu-id="d0d09-129">Отсутствующие свойства будут стерт.</span><span class="sxs-lookup"><span data-stu-id="d0d09-129">Missing properties will be erased.</span></span>

### <a name="response"></a><span data-ttu-id="d0d09-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0d09-130">Response</span></span>

<span data-ttu-id="d0d09-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d0d09-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="examples"></a><span data-ttu-id="d0d09-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="d0d09-133">Examples</span></span>

##### <a name="request"></a><span data-ttu-id="d0d09-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0d09-134">Request</span></span>
<span data-ttu-id="d0d09-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0d09-135">The following is an example of a request.</span></span> 

><span data-ttu-id="d0d09-136">**Примечание:** Показанный здесь объект запроса сокращается для читаемости.</span><span class="sxs-lookup"><span data-stu-id="d0d09-136">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="d0d09-137">Включай все свойства в фактический вызов.</span><span class="sxs-lookup"><span data-stu-id="d0d09-137">Include all the properties in an actual call.</span></span>

# <a name="http"></a>[<span data-ttu-id="d0d09-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0d09-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d0d09-139">C#</span><span class="sxs-lookup"><span data-stu-id="d0d09-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-synchronizationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0d09-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0d09-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-synchronizationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0d09-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0d09-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-synchronizationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d0d09-142">Java</span><span class="sxs-lookup"><span data-stu-id="d0d09-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-synchronizationtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d0d09-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0d09-143">Response</span></span>
<span data-ttu-id="d0d09-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d0d09-144">The following is an example of a response.</span></span>
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


