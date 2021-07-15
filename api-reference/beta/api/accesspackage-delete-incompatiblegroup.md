---
title: Удаление группы из несовместимых групп
description: Удалите ссылку, которая указывает, что группа несовместима с указанным пакетом доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 403d583aa2b4e4592a4ec0bd9d9f29c3b93a1927
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439444"
---
# <a name="remove-group-from-incompatiblegroups"></a><span data-ttu-id="5d60e-103">Удаление группы из несовместимых групп</span><span class="sxs-lookup"><span data-stu-id="5d60e-103">Remove group from incompatibleGroups</span></span>

<span data-ttu-id="5d60e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d60e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d60e-105">Удалите [группу](../resources/group.md) из списка групп, которые были отмечены как несовместимые в [accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="5d60e-105">Remove a [group](../resources/group.md) from the list of groups that have been marked as incompatible on an [accessPackage](../resources/accesspackage.md).</span></span>  

## <a name="permissions"></a><span data-ttu-id="5d60e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5d60e-106">Permissions</span></span>

<span data-ttu-id="5d60e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d60e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5d60e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d60e-109">Permission type</span></span>                        | <span data-ttu-id="5d60e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d60e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5d60e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d60e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5d60e-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d60e-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="5d60e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d60e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d60e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d60e-114">Not supported.</span></span> |
| <span data-ttu-id="5d60e-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="5d60e-115">Application</span></span>                            | <span data-ttu-id="5d60e-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d60e-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d60e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d60e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleGroups/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="5d60e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d60e-118">Request headers</span></span>

| <span data-ttu-id="5d60e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5d60e-119">Name</span></span>          | <span data-ttu-id="5d60e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5d60e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5d60e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5d60e-121">Authorization</span></span> | <span data-ttu-id="5d60e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d60e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5d60e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5d60e-124">Content-Type</span></span>  | <span data-ttu-id="5d60e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d60e-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5d60e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5d60e-127">Request body</span></span>

<span data-ttu-id="5d60e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5d60e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d60e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d60e-129">Response</span></span>

<span data-ttu-id="5d60e-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5d60e-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5d60e-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="5d60e-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5d60e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d60e-133">Request</span></span>

<span data-ttu-id="5d60e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d60e-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5d60e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d60e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_incompatiblegroup_from_accesspackage"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleGroups/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="5d60e-136">C#</span><span class="sxs-lookup"><span data-stu-id="5d60e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-incompatiblegroup-from-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d60e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d60e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-incompatiblegroup-from-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d60e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d60e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-incompatiblegroup-from-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5d60e-139">Java</span><span class="sxs-lookup"><span data-stu-id="5d60e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-incompatiblegroup-from-accesspackage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5d60e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d60e-140">Response</span></span>

<span data-ttu-id="5d60e-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5d60e-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove incompatibleGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


