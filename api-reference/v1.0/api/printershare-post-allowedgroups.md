---
title: Создание allowedGroup для принтераShare
description: Предоставление указанной группе доступа для отправки заданий печати на связанный принтер.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: a6a5e2cb69c2ee9ee65ef012108d001312666a74
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787788"
---
# <a name="create-allowedgroup-for-printershare"></a><span data-ttu-id="edb2e-103">Создание allowedGroup для принтераShare</span><span class="sxs-lookup"><span data-stu-id="edb2e-103">Create allowedGroup for printerShare</span></span>
<span data-ttu-id="edb2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edb2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="edb2e-105">Предоставление указанной группе доступа для отправки заданий печати в связанный [принтерShare.](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="edb2e-105">Grant the specified group access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="edb2e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="edb2e-106">Permissions</span></span>
<span data-ttu-id="edb2e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edb2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="edb2e-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="edb2e-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="edb2e-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="edb2e-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="edb2e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="edb2e-111">Permission type</span></span> | <span data-ttu-id="edb2e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="edb2e-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="edb2e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="edb2e-113">Delegated (work or school account)</span></span>| <span data-ttu-id="edb2e-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edb2e-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="edb2e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="edb2e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="edb2e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edb2e-116">Not Supported.</span></span>|
|<span data-ttu-id="edb2e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="edb2e-117">Application</span></span>|<span data-ttu-id="edb2e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edb2e-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="edb2e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="edb2e-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/shares/{printerShareId}/allowedGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="edb2e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="edb2e-120">Request headers</span></span>
|<span data-ttu-id="edb2e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="edb2e-121">Name</span></span>|<span data-ttu-id="edb2e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="edb2e-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="edb2e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="edb2e-123">Authorization</span></span>|<span data-ttu-id="edb2e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="edb2e-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="edb2e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="edb2e-126">Content-Type</span></span>|<span data-ttu-id="edb2e-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="edb2e-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="edb2e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="edb2e-129">Request body</span></span>
<span data-ttu-id="edb2e-130">В теле запроса укажи ссылку на объект группы с помощью формата, как показано `@odata.id` в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="edb2e-130">In the request body, supply a reference to a group entity by using the `@odata.id` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="edb2e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="edb2e-131">Response</span></span>

<span data-ttu-id="edb2e-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="edb2e-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="edb2e-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="edb2e-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="edb2e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="edb2e-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="edb2e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="edb2e-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="edb2e-136">C#</span><span class="sxs-lookup"><span data-stu-id="edb2e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="edb2e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="edb2e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="edb2e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="edb2e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="edb2e-139">Java</span><span class="sxs-lookup"><span data-stu-id="edb2e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-group-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="edb2e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="edb2e-140">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

