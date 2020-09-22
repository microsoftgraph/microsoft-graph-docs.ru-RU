---
title: Список Интерналспонсорс
description: Получение списка Интерналспонсорс Коннектедорганизатион.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 54fb11c521784cc4f91054df2358c7a663fae5ac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996523"
---
# <a name="list-internalsponsors"></a><span data-ttu-id="3f65d-103">Список Интерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="3f65d-103">List internalSponsors</span></span>

<span data-ttu-id="3f65d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f65d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f65d-105">Получение списка внутренних спонсоров [коннектедорганизатион](../resources/connectedorganization.md).</span><span class="sxs-lookup"><span data-stu-id="3f65d-105">Retrieve a list of a [connectedOrganization](../resources/connectedorganization.md)'s internal sponsors.</span></span>  <span data-ttu-id="3f65d-106">Внутренние спонсоры — это набор пользователей, которые могут утверждать запросы от имени других пользователей из этой подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="3f65d-106">The internal sponsors are a set of users who can approve requests on behalf of other users from that connected organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f65d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3f65d-107">Permissions</span></span>

<span data-ttu-id="3f65d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f65d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f65d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f65d-110">Permission type</span></span>|<span data-ttu-id="3f65d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f65d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="3f65d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f65d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3f65d-113">Ентитлементманажемент. Read. ALL, Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3f65d-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="3f65d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f65d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f65d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f65d-115">Not supported.</span></span> |
| <span data-ttu-id="3f65d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3f65d-116">Application</span></span>                            | <span data-ttu-id="3f65d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f65d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f65d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f65d-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/connectedOrganizations/{id}/internalSponsors
```

## <a name="request-headers"></a><span data-ttu-id="3f65d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3f65d-119">Request headers</span></span>
|<span data-ttu-id="3f65d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="3f65d-120">Name</span></span>|<span data-ttu-id="3f65d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3f65d-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3f65d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3f65d-122">Authorization</span></span>|<span data-ttu-id="3f65d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f65d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f65d-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3f65d-125">Request body</span></span>
<span data-ttu-id="3f65d-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3f65d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f65d-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f65d-127">Response</span></span>

<span data-ttu-id="3f65d-128">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3f65d-128">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3f65d-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="3f65d-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3f65d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f65d-130">Request</span></span>

<span data-ttu-id="3f65d-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f65d-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3f65d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f65d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "connectedorganization_get_internalSponsors"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}/internalSponsors
```
# <a name="c"></a>[<span data-ttu-id="3f65d-133">C#</span><span class="sxs-lookup"><span data-stu-id="3f65d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connectedorganization-get-internalsponsors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f65d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f65d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connectedorganization-get-internalsponsors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f65d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f65d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connectedorganization-get-internalsponsors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3f65d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f65d-136">Response</span></span>

<span data-ttu-id="3f65d-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3f65d-137">The following is an example of the response.</span></span>

<span data-ttu-id="3f65d-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3f65d-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "cd3709c6-be6a-4725-bd07-50f90ccca93f"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List internalSponsors",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


