---
title: Создание allowedGroup для принтераShare
description: Предоставление указанной группе доступа для отправки заданий печати на связанный принтер.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 35f949929da692160a1671ab75945038e46f8a27
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771472"
---
# <a name="create-allowedgroup-for-printershare"></a><span data-ttu-id="c1ab1-103">Создание allowedGroup для принтераShare</span><span class="sxs-lookup"><span data-stu-id="c1ab1-103">Create allowedGroup for printerShare</span></span>
<span data-ttu-id="c1ab1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1ab1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="c1ab1-105">Предоставление указанной группе доступа для отправки заданий печати в связанный [принтерShare.](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="c1ab1-105">Grant the specified group access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c1ab1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c1ab1-106">Permissions</span></span>
<span data-ttu-id="c1ab1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1ab1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c1ab1-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="c1ab1-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="c1ab1-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="c1ab1-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="c1ab1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1ab1-111">Permission type</span></span> | <span data-ttu-id="c1ab1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1ab1-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c1ab1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1ab1-113">Delegated (work or school account)</span></span>| <span data-ttu-id="c1ab1-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1ab1-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="c1ab1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1ab1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1ab1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1ab1-116">Not Supported.</span></span>|
|<span data-ttu-id="c1ab1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1ab1-117">Application</span></span>|<span data-ttu-id="c1ab1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1ab1-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1ab1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1ab1-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/shares/{printerShareId}/allowedGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="c1ab1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1ab1-120">Request headers</span></span>
|<span data-ttu-id="c1ab1-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c1ab1-121">Name</span></span>|<span data-ttu-id="c1ab1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c1ab1-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c1ab1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1ab1-123">Authorization</span></span>|<span data-ttu-id="c1ab1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1ab1-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c1ab1-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c1ab1-126">Content-Type</span></span>|<span data-ttu-id="c1ab1-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1ab1-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1ab1-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1ab1-129">Request body</span></span>
<span data-ttu-id="c1ab1-130">В теле запроса укажи ссылку на объект группы с помощью формата, как показано `@odata.id` в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="c1ab1-130">In the request body, supply a reference to a group entity by using the `@odata.id` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="c1ab1-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1ab1-131">Response</span></span>

<span data-ttu-id="c1ab1-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c1ab1-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c1ab1-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="c1ab1-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c1ab1-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1ab1-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c1ab1-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1ab1-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_group_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/allowedGroups/$ref
Content-Type: application/json
Content-length: 47

{
  "@odata.id": "https://graph.microsoft.com/v1.0/groups/{groupId}"
}
```
# <a name="c"></a>[<span data-ttu-id="c1ab1-136">C#</span><span class="sxs-lookup"><span data-stu-id="c1ab1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1ab1-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1ab1-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1ab1-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1ab1-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c1ab1-139">Java</span><span class="sxs-lookup"><span data-stu-id="c1ab1-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-group-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c1ab1-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1ab1-140">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
}
-->
``` http
HTTP/1.1 204 No Content
```

