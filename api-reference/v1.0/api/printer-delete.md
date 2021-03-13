---
title: Удаление принтера
description: Удаление (незарегистрированного) принтера.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 94841d1668363ffeb98d8416527c06d53bb7c517
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776930"
---
# <a name="delete-printer"></a><span data-ttu-id="c971f-103">Удаление принтера</span><span class="sxs-lookup"><span data-stu-id="c971f-103">Delete printer</span></span>
<span data-ttu-id="c971f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c971f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="c971f-105">Удаление (незарегистрированного) [принтера.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="c971f-105">Delete (unregister) a [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c971f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c971f-106">Permissions</span></span>
<span data-ttu-id="c971f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c971f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c971f-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="c971f-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="c971f-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="c971f-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="c971f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c971f-111">Permission type</span></span> | <span data-ttu-id="c971f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c971f-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c971f-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c971f-113">Delegated (work or school account)</span></span>| <span data-ttu-id="c971f-114">Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="c971f-114">Printer.FullControl.All</span></span> |
|<span data-ttu-id="c971f-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c971f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c971f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c971f-116">Not Supported.</span></span>|
|<span data-ttu-id="c971f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c971f-117">Application</span></span>|<span data-ttu-id="c971f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c971f-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c971f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c971f-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /print/printers/{printerId}
```

## <a name="request-headers"></a><span data-ttu-id="c971f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c971f-120">Request headers</span></span>
|<span data-ttu-id="c971f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c971f-121">Name</span></span>|<span data-ttu-id="c971f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c971f-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c971f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c971f-123">Authorization</span></span>|<span data-ttu-id="c971f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c971f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c971f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c971f-126">Request body</span></span>
<span data-ttu-id="c971f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c971f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c971f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c971f-128">Response</span></span>

<span data-ttu-id="c971f-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c971f-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c971f-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="c971f-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c971f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c971f-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c971f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c971f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printer"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/printers/{printerId}
```
# <a name="c"></a>[<span data-ttu-id="c971f-133">C#</span><span class="sxs-lookup"><span data-stu-id="c971f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c971f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c971f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c971f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c971f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c971f-136">Java</span><span class="sxs-lookup"><span data-stu-id="c971f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-printer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c971f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c971f-137">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

