---
title: Создание allowedGroup для принтераShare
description: Предоставление указанной группе доступа для отправки заданий печати на связанный принтер.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 57f844b98da47f5063ee3aaee7534b5e242ad5d0
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51765995"
---
# <a name="create-allowedgroup-for-printershare"></a><span data-ttu-id="089eb-103">Создание allowedGroup для принтераShare</span><span class="sxs-lookup"><span data-stu-id="089eb-103">Create allowedGroup for printerShare</span></span>

<span data-ttu-id="089eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="089eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="089eb-105">Предоставление указанной группе доступа для отправки заданий печати в связанный [принтерShare.](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="089eb-105">Grant the specified group access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="089eb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="089eb-106">Permissions</span></span>
<span data-ttu-id="089eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="089eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="089eb-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="089eb-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="089eb-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="089eb-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="089eb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="089eb-111">Permission type</span></span> | <span data-ttu-id="089eb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="089eb-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="089eb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="089eb-113">Delegated (work or school account)</span></span>| <span data-ttu-id="089eb-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="089eb-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="089eb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="089eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="089eb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="089eb-116">Not Supported.</span></span>|
|<span data-ttu-id="089eb-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="089eb-117">Application</span></span>|<span data-ttu-id="089eb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="089eb-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="089eb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="089eb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/shares/{id}/allowedGroups/$ref
```
## <a name="request-headers"></a><span data-ttu-id="089eb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="089eb-120">Request headers</span></span>
| <span data-ttu-id="089eb-121">Имя</span><span class="sxs-lookup"><span data-stu-id="089eb-121">Name</span></span>          | <span data-ttu-id="089eb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="089eb-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="089eb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="089eb-123">Authorization</span></span> | <span data-ttu-id="089eb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="089eb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="089eb-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="089eb-126">Content-type</span></span>  | <span data-ttu-id="089eb-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="089eb-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="089eb-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="089eb-129">Request body</span></span>
<span data-ttu-id="089eb-130">В теле запроса укажи ссылку на объект группы с помощью формата, как показано `@odata.id` в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="089eb-130">In the request body, supply a reference to a group entity by using the `@odata.id` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="089eb-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="089eb-131">Response</span></span>
<span data-ttu-id="089eb-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="089eb-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="089eb-133">Пример</span><span class="sxs-lookup"><span data-stu-id="089eb-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="089eb-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="089eb-134">Request</span></span>
<span data-ttu-id="089eb-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="089eb-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="089eb-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="089eb-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_allowedgroup_from_printers"
}-->
```http
POST https://graph.microsoft.com/beta/print/shares/{id}/allowedGroups/$ref
Content-type: application/json
Content-length: 67

{
  "@odata.id": "https://graph.microsoft.com/beta/groups/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="089eb-137">C#</span><span class="sxs-lookup"><span data-stu-id="089eb-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-allowedgroup-from-printers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="089eb-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="089eb-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-allowedgroup-from-printers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="089eb-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="089eb-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-allowedgroup-from-printers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="089eb-140">Java</span><span class="sxs-lookup"><span data-stu-id="089eb-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-allowedgroup-from-printers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="089eb-141">В теле запроса укажи ссылку на объект группы, включив URI Microsoft Graph группы в поле `@odata.id` тела JSON.</span><span class="sxs-lookup"><span data-stu-id="089eb-141">In the request body, supply a reference to a group entity by including the group's Microsoft Graph URI in the `@odata.id` field of the JSON body.</span></span>

### <a name="response"></a><span data-ttu-id="089eb-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="089eb-142">Response</span></span>
<span data-ttu-id="089eb-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="089eb-143">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create allowedGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
