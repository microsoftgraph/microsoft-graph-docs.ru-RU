---
title: Удаление printConnector
description: Удаление (отрегистрации) printConnector.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 71edae5cf61e9e3ab7e9d8ec8b36ed679d0c04f6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772158"
---
# <a name="delete-printconnector"></a><span data-ttu-id="f6ec8-103">Удаление printConnector</span><span class="sxs-lookup"><span data-stu-id="f6ec8-103">Delete printConnector</span></span>
<span data-ttu-id="f6ec8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6ec8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="f6ec8-105">Удаление (незарегистрированного) **printConnector**.</span><span class="sxs-lookup"><span data-stu-id="f6ec8-105">Delete (unregister) a **printConnector**.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6ec8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6ec8-106">Permissions</span></span>
<span data-ttu-id="f6ec8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6ec8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f6ec8-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="f6ec8-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="f6ec8-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="f6ec8-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="f6ec8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6ec8-111">Permission type</span></span> | <span data-ttu-id="f6ec8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6ec8-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="f6ec8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6ec8-113">Delegated (work or school account)</span></span>| <span data-ttu-id="f6ec8-114">PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6ec8-114">PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="f6ec8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6ec8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6ec8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6ec8-116">Not Supported.</span></span>|
|<span data-ttu-id="f6ec8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6ec8-117">Application</span></span>|<span data-ttu-id="f6ec8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6ec8-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6ec8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6ec8-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /print/connectors/{printConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="f6ec8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6ec8-120">Request headers</span></span>
|<span data-ttu-id="f6ec8-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f6ec8-121">Name</span></span>|<span data-ttu-id="f6ec8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f6ec8-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f6ec8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f6ec8-123">Authorization</span></span>|<span data-ttu-id="f6ec8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6ec8-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6ec8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f6ec8-126">Request body</span></span>
<span data-ttu-id="f6ec8-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f6ec8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6ec8-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6ec8-128">Response</span></span>
<span data-ttu-id="f6ec8-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f6ec8-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="error-conditions-and-messages"></a><span data-ttu-id="f6ec8-131">Условия ошибки и сообщения</span><span class="sxs-lookup"><span data-stu-id="f6ec8-131">Error conditions and messages</span></span>

|<span data-ttu-id="f6ec8-132">Сценарий</span><span class="sxs-lookup"><span data-stu-id="f6ec8-132">Scenario</span></span>|<span data-ttu-id="f6ec8-133">Метод</span><span class="sxs-lookup"><span data-stu-id="f6ec8-133">Method</span></span>|<span data-ttu-id="f6ec8-134">Код</span><span class="sxs-lookup"><span data-stu-id="f6ec8-134">Code</span></span>|<span data-ttu-id="f6ec8-135">Сообщение</span><span class="sxs-lookup"><span data-stu-id="f6ec8-135">Message</span></span>|
|--------|------|----|-------|
|<span data-ttu-id="f6ec8-136">Пользователь пытается удалить соединителя, который имеет один или несколько принтеров зарегистрированы</span><span class="sxs-lookup"><span data-stu-id="f6ec8-136">User attempts to delete a connector that has one or more printers registered</span></span>|<span data-ttu-id="f6ec8-137">DELETE</span><span class="sxs-lookup"><span data-stu-id="f6ec8-137">DELETE</span></span>|<span data-ttu-id="f6ec8-138">409</span><span class="sxs-lookup"><span data-stu-id="f6ec8-138">409</span></span>|<span data-ttu-id="f6ec8-139">Перед удалением соединителя удаляйте связанные принтеры.</span><span class="sxs-lookup"><span data-stu-id="f6ec8-139">Before deleting the connector, please unregister the associated printers.</span></span>|

## <a name="examples"></a><span data-ttu-id="f6ec8-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="f6ec8-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f6ec8-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6ec8-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f6ec8-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6ec8-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printconnector"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/connectors/{printConnectorId}
```
# <a name="c"></a>[<span data-ttu-id="f6ec8-143">C#</span><span class="sxs-lookup"><span data-stu-id="f6ec8-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6ec8-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6ec8-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6ec8-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6ec8-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f6ec8-146">Java</span><span class="sxs-lookup"><span data-stu-id="f6ec8-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-printconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f6ec8-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6ec8-147">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

