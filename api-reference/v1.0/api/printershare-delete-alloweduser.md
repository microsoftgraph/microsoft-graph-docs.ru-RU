---
title: Удаление allowedUser из printerShare
description: Отзовет доступ указанного пользователя к отправке заданий печати в связанную долю принтера.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 453fd853c7631ccb84c8b5709a33a787fc859444
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771745"
---
# <a name="delete-alloweduser-from-printershare"></a><span data-ttu-id="43297-103">Удаление allowedUser из printerShare</span><span class="sxs-lookup"><span data-stu-id="43297-103">Delete allowedUser from printerShare</span></span>

<span data-ttu-id="43297-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43297-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="43297-105">Отзовет доступ указанного пользователя для отправки заданий печати в связанный [принтерShare.](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="43297-105">Revoke the specified user's access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="43297-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="43297-106">Permissions</span></span>
<span data-ttu-id="43297-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43297-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="43297-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="43297-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="43297-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="43297-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="43297-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43297-111">Permission type</span></span> | <span data-ttu-id="43297-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="43297-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="43297-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43297-113">Delegated (work or school account)</span></span>| <span data-ttu-id="43297-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43297-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="43297-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43297-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43297-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43297-116">Not Supported.</span></span>|
|<span data-ttu-id="43297-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43297-117">Application</span></span>|<span data-ttu-id="43297-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43297-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43297-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43297-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/shares/{printerShareId}/allowedUsers/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="43297-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43297-120">Request headers</span></span>
| <span data-ttu-id="43297-121">Имя</span><span class="sxs-lookup"><span data-stu-id="43297-121">Name</span></span>          | <span data-ttu-id="43297-122">Описание</span><span class="sxs-lookup"><span data-stu-id="43297-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="43297-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="43297-123">Authorization</span></span> | <span data-ttu-id="43297-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43297-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="43297-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="43297-126">Request body</span></span>
<span data-ttu-id="43297-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="43297-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43297-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="43297-128">Response</span></span>
<span data-ttu-id="43297-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="43297-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43297-131">Пример</span><span class="sxs-lookup"><span data-stu-id="43297-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="43297-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="43297-132">Request</span></span>
<span data-ttu-id="43297-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43297-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="43297-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="43297-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_alloweduser"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/allowedUsers/{userId}/$ref
```
# <a name="c"></a>[<span data-ttu-id="43297-135">C#</span><span class="sxs-lookup"><span data-stu-id="43297-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-alloweduser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="43297-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="43297-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-alloweduser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="43297-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="43297-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-alloweduser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="43297-138">Java</span><span class="sxs-lookup"><span data-stu-id="43297-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-alloweduser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="43297-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="43297-139">Response</span></span>
<span data-ttu-id="43297-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="43297-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
