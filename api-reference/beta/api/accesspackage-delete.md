---
title: Удаление accessPackage
description: Удаление accessPackage.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 710bbd3e015af5109b95905d6db68061de1506f5
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52868870"
---
# <a name="delete-accesspackage"></a><span data-ttu-id="ebc62-103">Удаление accessPackage</span><span class="sxs-lookup"><span data-stu-id="ebc62-103">Delete accessPackage</span></span>

<span data-ttu-id="ebc62-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebc62-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebc62-105">Удаление [объекта accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="ebc62-105">Delete an [accessPackage](../resources/accesspackage.md) object.</span></span>

<span data-ttu-id="ebc62-106">Нельзя удалить пакет доступа, если у него есть **какой-либо accessPackageAssignment.**</span><span class="sxs-lookup"><span data-stu-id="ebc62-106">You cannot delete an access package if it has any **accessPackageAssignment**.</span></span> <span data-ttu-id="ebc62-107">Чтобы удалить пакет доступа, сначала запросите, если есть назначения с фильтром, чтобы указать определенный пакет доступа, например: [](accesspackageassignment-list.md) `$filter=accessPackage/id eq 'a914b616-e04e-476b-aa37-91038f0b165b'` .</span><span class="sxs-lookup"><span data-stu-id="ebc62-107">To delete the access package, first [query if there are any assignments](accesspackageassignment-list.md) with a filter to indicate the specific access package, such as: `$filter=accessPackage/id eq 'a914b616-e04e-476b-aa37-91038f0b165b'`.</span></span> <span data-ttu-id="ebc62-108">Дополнительные сведения о том, как удалить назначения, которые по-прежнему находятся в доставленных состояниях, см. в статью [Удалить назначение.](accesspackageassignmentrequest-post.md#example-4-remove-an-assignment)</span><span class="sxs-lookup"><span data-stu-id="ebc62-108">For more information on how to remove assignments that are still in the delivered state, see [Remove an assignment](accesspackageassignmentrequest-post.md#example-4-remove-an-assignment).</span></span>


## <a name="permissions"></a><span data-ttu-id="ebc62-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ebc62-109">Permissions</span></span>

<span data-ttu-id="ebc62-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebc62-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ebc62-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ebc62-112">Permission type</span></span>                        | <span data-ttu-id="ebc62-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ebc62-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ebc62-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ebc62-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="ebc62-115">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebc62-115">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="ebc62-116">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ebc62-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebc62-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebc62-117">Not supported.</span></span> |
| <span data-ttu-id="ebc62-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="ebc62-118">Application</span></span>                            | <span data-ttu-id="ebc62-119">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebc62-119">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebc62-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ebc62-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ebc62-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ebc62-121">Request headers</span></span>

| <span data-ttu-id="ebc62-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ebc62-122">Name</span></span>          | <span data-ttu-id="ebc62-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ebc62-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ebc62-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ebc62-124">Authorization</span></span> | <span data-ttu-id="ebc62-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ebc62-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ebc62-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ebc62-127">Request body</span></span>

<span data-ttu-id="ebc62-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ebc62-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebc62-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebc62-129">Response</span></span>

<span data-ttu-id="ebc62-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ebc62-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ebc62-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="ebc62-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ebc62-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ebc62-133">Request</span></span>

<span data-ttu-id="ebc62-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ebc62-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ebc62-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ebc62-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accesspackage"
}-->

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}
```
# <a name="c"></a>[<span data-ttu-id="ebc62-136">C#</span><span class="sxs-lookup"><span data-stu-id="ebc62-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ebc62-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ebc62-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ebc62-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ebc62-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ebc62-139">Java</span><span class="sxs-lookup"><span data-stu-id="ebc62-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-accesspackage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ebc62-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebc62-140">Response</span></span>

<span data-ttu-id="ebc62-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ebc62-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete accessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


