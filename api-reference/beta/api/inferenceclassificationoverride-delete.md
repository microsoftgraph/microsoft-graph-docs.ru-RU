---
title: Удаление объекта inferenceClassificationOverride
description: Удаление отсортированного переопределения папки "Входящие", указанного с помощью идентификатора.
localization_priority: Normal
doc_type: apiPageType
author: svpsiva
ms.prod: ''
ms.openlocfilehash: 7565fadfa68bca6c61b8d268f36a93f95c48a2a1
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807222"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="1bdc6-103">Удаление объекта inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="1bdc6-103">Delete inferenceClassificationOverride</span></span>

<span data-ttu-id="1bdc6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bdc6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bdc6-105">Удаление [отсортированного переопределения папки "Входящие"](../resources/manage-focused-inbox.md) , указанного с помощью идентификатора.</span><span class="sxs-lookup"><span data-stu-id="1bdc6-105">Delete a [Focused Inbox](../resources/manage-focused-inbox.md) override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="1bdc6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1bdc6-106">Permissions</span></span>
<span data-ttu-id="1bdc6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bdc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bdc6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1bdc6-109">Permission type</span></span>      | <span data-ttu-id="1bdc6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1bdc6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bdc6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1bdc6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1bdc6-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1bdc6-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1bdc6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1bdc6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bdc6-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1bdc6-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1bdc6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1bdc6-115">Application</span></span> | <span data-ttu-id="1bdc6-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1bdc6-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1bdc6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1bdc6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1bdc6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1bdc6-118">Request headers</span></span>
| <span data-ttu-id="1bdc6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1bdc6-119">Name</span></span>       | <span data-ttu-id="1bdc6-120">Тип</span><span class="sxs-lookup"><span data-stu-id="1bdc6-120">Type</span></span> | <span data-ttu-id="1bdc6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1bdc6-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1bdc6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bdc6-122">Authorization</span></span>  | <span data-ttu-id="1bdc6-123">string</span><span class="sxs-lookup"><span data-stu-id="1bdc6-123">string</span></span>  | <span data-ttu-id="1bdc6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bdc6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1bdc6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1bdc6-126">Request body</span></span>
<span data-ttu-id="1bdc6-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1bdc6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bdc6-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bdc6-128">Response</span></span>

<span data-ttu-id="1bdc6-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1bdc6-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bdc6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1bdc6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1bdc6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bdc6-132">Request</span></span>
<span data-ttu-id="1bdc6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1bdc6-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1bdc6-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1bdc6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
# <a name="c"></a>[<span data-ttu-id="1bdc6-135">C#</span><span class="sxs-lookup"><span data-stu-id="1bdc6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-inferenceclassificationoverride-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1bdc6-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1bdc6-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-inferenceclassificationoverride-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1bdc6-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1bdc6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-inferenceclassificationoverride-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1bdc6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bdc6-138">Response</span></span>
<span data-ttu-id="1bdc6-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1bdc6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
