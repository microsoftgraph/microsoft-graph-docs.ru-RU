---
title: Удаление Алловедусер с принтера
description: Отозвать доступ указанного пользователя, чтобы послать задания печати на связанный принтер.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 23968799ef0ac02a65e47293018dc8ba21d86cf8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035796"
---
# <a name="delete-alloweduser-from-printer"></a><span data-ttu-id="be5a9-103">Удаление Алловедусер с принтера</span><span class="sxs-lookup"><span data-stu-id="be5a9-103">Delete allowedUser from printer</span></span>

<span data-ttu-id="be5a9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be5a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be5a9-105">Отозвать доступ указанного пользователя, чтобы послать задания печати на связанный [принтер](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="be5a9-105">Revoke the specified user's access to submit print jobs to the associated [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="be5a9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="be5a9-106">Permissions</span></span>
<span data-ttu-id="be5a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be5a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="be5a9-109">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать в дополнение к разрешениям, приведенным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="be5a9-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="be5a9-110">Пользователь, вошедшего в систему, должен быть [администратором принтера](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="be5a9-110">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="be5a9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be5a9-111">Permission type</span></span> | <span data-ttu-id="be5a9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="be5a9-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="be5a9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be5a9-113">Delegated (work or school account)</span></span>| <span data-ttu-id="be5a9-114">Printer. ReadWrite. ALL, Printer. FullControl. ALL</span><span class="sxs-lookup"><span data-stu-id="be5a9-114">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="be5a9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be5a9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be5a9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be5a9-116">Not Supported.</span></span>|
|<span data-ttu-id="be5a9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be5a9-117">Application</span></span>| <span data-ttu-id="be5a9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be5a9-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be5a9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be5a9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printers/{id}/allowedUsers/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="be5a9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be5a9-120">Request headers</span></span>
| <span data-ttu-id="be5a9-121">Имя</span><span class="sxs-lookup"><span data-stu-id="be5a9-121">Name</span></span>          | <span data-ttu-id="be5a9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="be5a9-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="be5a9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be5a9-123">Authorization</span></span> | <span data-ttu-id="be5a9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be5a9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be5a9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="be5a9-126">Request body</span></span>
<span data-ttu-id="be5a9-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="be5a9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be5a9-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="be5a9-128">Response</span></span>
<span data-ttu-id="be5a9-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="be5a9-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be5a9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="be5a9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be5a9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="be5a9-132">Request</span></span>
<span data-ttu-id="be5a9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be5a9-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="be5a9-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="be5a9-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_alloweduser"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/printers/{id}/allowedUsers/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="be5a9-135">C#</span><span class="sxs-lookup"><span data-stu-id="be5a9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-alloweduser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be5a9-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be5a9-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-alloweduser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be5a9-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be5a9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-alloweduser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="be5a9-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="be5a9-138">Response</span></span>
<span data-ttu-id="be5a9-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="be5a9-139">The following is an example of the response.</span></span>
><span data-ttu-id="be5a9-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="be5a9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete allowedUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


