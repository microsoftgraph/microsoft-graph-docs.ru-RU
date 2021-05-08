---
title: Список oAuth2PermissionGrants
description: Получение списка объектов oauth2PermissionGrant, представляющих делегированную дотации разрешений.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 3936c820e939032b456b60f8bd591c298ebc3c44
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231957"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="b2f92-103">Перечисление oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="b2f92-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="b2f92-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2f92-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b2f92-105">Получение списка [объектов oAuth2PermissionGrant,](../resources/oauth2permissiongrant.md) представляющих делегированную лицензию, выданную для клиентских приложений для доступа к API от имени пользователей, входиющих в нее.</span><span class="sxs-lookup"><span data-stu-id="b2f92-105">Retrieve a list of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects, representing delegated permissions which have been granted for client applications to access APIs on behalf of signed-in users.</span></span>

> [!NOTE]
> <span data-ttu-id="b2f92-106">Этот запрос может иметь задержки репликации для делегирования разрешений, которые были недавно созданы, обновлены или удалены.</span><span class="sxs-lookup"><span data-stu-id="b2f92-106">This request might have replication delays for delegated permission grants that were recently created, updated, or deleted.</span></span> <span data-ttu-id="b2f92-107">При указании фильтра эта задержка будет сведена `clientId` к минимуму.</span><span class="sxs-lookup"><span data-stu-id="b2f92-107">This delay will be minimized if a filter on `clientId` is specified.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2f92-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b2f92-108">Permissions</span></span>

<span data-ttu-id="b2f92-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2f92-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2f92-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2f92-111">Permission type</span></span>      | <span data-ttu-id="b2f92-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2f92-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2f92-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2f92-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b2f92-114">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b2f92-114">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b2f92-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2f92-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2f92-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2f92-116">Not supported.</span></span>    |
|<span data-ttu-id="b2f92-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2f92-117">Application</span></span> | <span data-ttu-id="b2f92-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2f92-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2f92-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2f92-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b2f92-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b2f92-120">Optional query parameters</span></span>

<span data-ttu-id="b2f92-121">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b2f92-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b2f92-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2f92-122">Request headers</span></span>

| <span data-ttu-id="b2f92-123">Имя</span><span class="sxs-lookup"><span data-stu-id="b2f92-123">Name</span></span>          | <span data-ttu-id="b2f92-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b2f92-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b2f92-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2f92-125">Authorization</span></span> | <span data-ttu-id="b2f92-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2f92-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2f92-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2f92-128">Request body</span></span>

<span data-ttu-id="b2f92-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b2f92-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2f92-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2f92-130">Response</span></span>

<span data-ttu-id="b2f92-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b2f92-131">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2f92-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b2f92-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2f92-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2f92-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b2f92-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2f92-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_oauth2permissiongrants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/oauth2PermissionGrants
```
# <a name="c"></a>[<span data-ttu-id="b2f92-135">C#</span><span class="sxs-lookup"><span data-stu-id="b2f92-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b2f92-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2f92-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b2f92-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2f92-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b2f92-138">Java</span><span class="sxs-lookup"><span data-stu-id="b2f92-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-oauth2permissiongrants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b2f92-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2f92-139">Response</span></span>

> <span data-ttu-id="b2f92-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b2f92-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "value": [
    {
      "id": "id-value",
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value",
      "scope": "scope-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oauth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

