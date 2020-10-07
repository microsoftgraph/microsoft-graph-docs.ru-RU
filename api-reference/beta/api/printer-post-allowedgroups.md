---
title: Создание Алловедграуп для принтера
description: Предоставление указанному групповому доступу на отправку заданий печати на связанный принтер.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: f7d11e7c7ea3a87b9bfcc42f2334ff1139fc8823
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2020
ms.locfileid: "48372868"
---
# <a name="create-allowedgroup-for-printer"></a><span data-ttu-id="2a3b2-103">Создание Алловедграуп для принтера</span><span class="sxs-lookup"><span data-stu-id="2a3b2-103">Create allowedGroup for printer</span></span>

<span data-ttu-id="2a3b2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a3b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a3b2-105">Предоставление указанному групповому доступу на отправку **заданий печати** на связанный [принтер](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="2a3b2-105">Grant the specified group access to submit **print jobs** to the associated [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2a3b2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a3b2-106">Permissions</span></span>
<span data-ttu-id="2a3b2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a3b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="2a3b2-109">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать в дополнение к разрешениям, приведенным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="2a3b2-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="2a3b2-110">Пользователь, вошедшего в систему, должен быть [администратором принтера](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="2a3b2-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="2a3b2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a3b2-111">Permission type</span></span> | <span data-ttu-id="2a3b2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a3b2-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="2a3b2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a3b2-113">Delegated (work or school account)</span></span>| <span data-ttu-id="2a3b2-114">Printer. ReadWrite. ALL, Printer. FullControl. ALL</span><span class="sxs-lookup"><span data-stu-id="2a3b2-114">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="2a3b2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a3b2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a3b2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a3b2-116">Not Supported.</span></span>|
|<span data-ttu-id="2a3b2-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2a3b2-117">Application</span></span>| <span data-ttu-id="2a3b2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a3b2-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a3b2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a3b2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/allowedGroups/$ref
```
## <a name="request-headers"></a><span data-ttu-id="2a3b2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a3b2-120">Request headers</span></span>
| <span data-ttu-id="2a3b2-121">Имя</span><span class="sxs-lookup"><span data-stu-id="2a3b2-121">Name</span></span>          | <span data-ttu-id="2a3b2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2a3b2-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2a3b2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a3b2-123">Authorization</span></span> | <span data-ttu-id="2a3b2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a3b2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2a3b2-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2a3b2-126">Content-type</span></span>  | <span data-ttu-id="2a3b2-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a3b2-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a3b2-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a3b2-129">Request body</span></span>
<span data-ttu-id="2a3b2-130">В теле запроса добавьте ссылку на объект Group с помощью `@odata.id` формата, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="2a3b2-130">In the request body, supply a reference to a group entity by using the `@odata.id` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="2a3b2-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a3b2-131">Response</span></span>
<span data-ttu-id="2a3b2-132">В случае успешного выполнения этот метод возвращает код отклика `201 Created`.</span><span class="sxs-lookup"><span data-stu-id="2a3b2-132">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2a3b2-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2a3b2-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2a3b2-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a3b2-134">Request</span></span>
<span data-ttu-id="2a3b2-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a3b2-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2a3b2-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a3b2-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_allowedgroup_from_printers"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/allowedGroups/$ref
Content-type: application/json
Content-length: 67

{
  "@odata.id": "https://graph.microsoft.com/beta/groups/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="2a3b2-137">C#</span><span class="sxs-lookup"><span data-stu-id="2a3b2-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-allowedgroup-from-printers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a3b2-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a3b2-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-allowedgroup-from-printers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a3b2-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a3b2-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-allowedgroup-from-printers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="2a3b2-140">В теле запроса добавьте ссылку на объект Group, указав URI Microsoft Graph в `@odata.id` поле тела JSON.</span><span class="sxs-lookup"><span data-stu-id="2a3b2-140">In the request body, supply a reference to a group entity by including the group's Microsoft Graph URI in the `@odata.id` field of the JSON body.</span></span>

##### <a name="response"></a><span data-ttu-id="2a3b2-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a3b2-141">Response</span></span>
<span data-ttu-id="2a3b2-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2a3b2-142">The following is an example of the response.</span></span> 
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
