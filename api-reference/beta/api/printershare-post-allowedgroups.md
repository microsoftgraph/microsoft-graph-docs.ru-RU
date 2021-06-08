---
title: Создание allowedGroup для принтераShare
description: Предоставление указанной группе доступа для отправки заданий печати на связанный принтер.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 1b6e11b1f4a650755d696e5bc346f4cf369324bb
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787529"
---
# <a name="create-allowedgroup-for-printershare"></a><span data-ttu-id="441a6-103">Создание allowedGroup для принтераShare</span><span class="sxs-lookup"><span data-stu-id="441a6-103">Create allowedGroup for printerShare</span></span>

<span data-ttu-id="441a6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="441a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="441a6-105">Предоставление указанной группе доступа для отправки заданий печати в связанный [принтерShare.](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="441a6-105">Grant the specified group access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="441a6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="441a6-106">Permissions</span></span>
<span data-ttu-id="441a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="441a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="441a6-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="441a6-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="441a6-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="441a6-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="441a6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="441a6-111">Permission type</span></span> | <span data-ttu-id="441a6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="441a6-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="441a6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="441a6-113">Delegated (work or school account)</span></span>| <span data-ttu-id="441a6-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="441a6-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="441a6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="441a6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="441a6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="441a6-116">Not Supported.</span></span>|
|<span data-ttu-id="441a6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="441a6-117">Application</span></span>|<span data-ttu-id="441a6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="441a6-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="441a6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="441a6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/shares/{id}/allowedGroups/$ref
```
## <a name="request-headers"></a><span data-ttu-id="441a6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="441a6-120">Request headers</span></span>
| <span data-ttu-id="441a6-121">Имя</span><span class="sxs-lookup"><span data-stu-id="441a6-121">Name</span></span>          | <span data-ttu-id="441a6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="441a6-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="441a6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="441a6-123">Authorization</span></span> | <span data-ttu-id="441a6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="441a6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="441a6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="441a6-126">Content-type</span></span>  | <span data-ttu-id="441a6-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="441a6-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="441a6-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="441a6-129">Request body</span></span>
<span data-ttu-id="441a6-130">В теле запроса укажи ссылку на объект группы с помощью формата, как показано `@odata.id` в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="441a6-130">In the request body, supply a reference to a group entity by using the `@odata.id` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="441a6-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="441a6-131">Response</span></span>
<span data-ttu-id="441a6-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="441a6-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="441a6-133">Пример</span><span class="sxs-lookup"><span data-stu-id="441a6-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="441a6-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="441a6-134">Request</span></span>
<span data-ttu-id="441a6-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="441a6-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="441a6-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="441a6-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="441a6-137">C#</span><span class="sxs-lookup"><span data-stu-id="441a6-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-allowedgroup-from-printers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="441a6-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="441a6-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-allowedgroup-from-printers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="441a6-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="441a6-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-allowedgroup-from-printers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="441a6-140">Java</span><span class="sxs-lookup"><span data-stu-id="441a6-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-allowedgroup-from-printers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="441a6-141">В теле запроса укажи ссылку на объект группы, включив URI Microsoft Graph группы в поле `@odata.id` тела JSON.</span><span class="sxs-lookup"><span data-stu-id="441a6-141">In the request body, supply a reference to a group entity by including the group's Microsoft Graph URI in the `@odata.id` field of the JSON body.</span></span>

### <a name="response"></a><span data-ttu-id="441a6-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="441a6-142">Response</span></span>
<span data-ttu-id="441a6-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="441a6-143">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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
