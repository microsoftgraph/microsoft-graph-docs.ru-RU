---
title: Удаление printerShare
description: Удаление доли принтера (стереть связанный принтер). Это действие невозможно отменить. Если принтер будет снова открыт в будущем, пользователям Windows, которые ранее установили принтер, потребуется его обнаружить и повторно установить.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 95a907f18693165304894fab41da36e28b551f35
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771668"
---
# <a name="delete-printershare"></a><span data-ttu-id="b9a3a-105">Удаление printerShare</span><span class="sxs-lookup"><span data-stu-id="b9a3a-105">Delete printerShare</span></span>
<span data-ttu-id="b9a3a-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9a3a-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="b9a3a-107">Удаление доли принтера (удалить связанный [принтер).](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="b9a3a-107">Delete a printer share (unshare the associated [printer](../resources/printer.md)).</span></span> <span data-ttu-id="b9a3a-108">Это действие невозможно отменить.</span><span class="sxs-lookup"><span data-stu-id="b9a3a-108">This action cannot be undone.</span></span> <span data-ttu-id="b9a3a-109">Если принтер [будет](../resources/printer.md) снова открыт в будущем, пользователям Windows, которые ранее установили принтер, потребуется его обнаружить и переустановить. [](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="b9a3a-109">If the [printer](../resources/printer.md) is shared again in the future, any Windows users who had previously installed the [printer](../resources/printer.md) will need to discover and reinstall it.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9a3a-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9a3a-110">Permissions</span></span>
<span data-ttu-id="b9a3a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9a3a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b9a3a-113">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="b9a3a-113">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="b9a3a-114">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="b9a3a-114">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="b9a3a-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9a3a-115">Permission type</span></span> | <span data-ttu-id="b9a3a-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9a3a-116">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="b9a3a-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9a3a-117">Delegated (work or school account)</span></span>| <span data-ttu-id="b9a3a-118">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9a3a-118">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="b9a3a-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9a3a-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9a3a-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9a3a-120">Not Supported.</span></span>|
|<span data-ttu-id="b9a3a-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9a3a-121">Application</span></span>|<span data-ttu-id="b9a3a-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9a3a-122">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9a3a-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9a3a-123">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /print/shares/{printerShareId}
```

## <a name="request-headers"></a><span data-ttu-id="b9a3a-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9a3a-124">Request headers</span></span>
|<span data-ttu-id="b9a3a-125">Имя</span><span class="sxs-lookup"><span data-stu-id="b9a3a-125">Name</span></span>|<span data-ttu-id="b9a3a-126">Описание</span><span class="sxs-lookup"><span data-stu-id="b9a3a-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b9a3a-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9a3a-127">Authorization</span></span>|<span data-ttu-id="b9a3a-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9a3a-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9a3a-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9a3a-130">Request body</span></span>
<span data-ttu-id="b9a3a-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b9a3a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9a3a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9a3a-132">Response</span></span>

<span data-ttu-id="b9a3a-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b9a3a-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b9a3a-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="b9a3a-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b9a3a-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9a3a-136">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b9a3a-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9a3a-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printershare"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/shares/{printerShareId}
```
# <a name="c"></a>[<span data-ttu-id="b9a3a-138">C#</span><span class="sxs-lookup"><span data-stu-id="b9a3a-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9a3a-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9a3a-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9a3a-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9a3a-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9a3a-141">Java</span><span class="sxs-lookup"><span data-stu-id="b9a3a-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-printershare-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b9a3a-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9a3a-142">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

