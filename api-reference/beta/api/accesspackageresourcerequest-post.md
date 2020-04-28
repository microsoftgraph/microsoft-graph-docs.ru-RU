---
title: Создание Акцесспаккажересаурцерекуест
description: Создание нового Акцесспаккажересаурцерекуест.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3f5087b313f21fdce39d67d93d814ac1e0a1ee61
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441951"
---
# <a name="create-accesspackageresourcerequest"></a><span data-ttu-id="182ef-103">Создание Акцесспаккажересаурцерекуест</span><span class="sxs-lookup"><span data-stu-id="182ef-103">Create accessPackageResourceRequest</span></span>

<span data-ttu-id="182ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="182ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="182ef-105">Создайте новый объект [акцесспаккажересаурцерекуест](../resources/accesspackageresourcerequest.md) , чтобы запросить Добавление ресурса в каталог пакетов Access.</span><span class="sxs-lookup"><span data-stu-id="182ef-105">Create a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object to request the addition of a resource to an access package catalog.</span></span>

## <a name="permissions"></a><span data-ttu-id="182ef-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="182ef-106">Permissions</span></span>

<span data-ttu-id="182ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="182ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="182ef-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="182ef-109">Permission type</span></span>                        | <span data-ttu-id="182ef-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="182ef-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="182ef-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="182ef-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="182ef-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="182ef-112">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="182ef-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="182ef-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="182ef-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="182ef-114">Not supported.</span></span> |
| <span data-ttu-id="182ef-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="182ef-115">Application</span></span>                            | <span data-ttu-id="182ef-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="182ef-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="182ef-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="182ef-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageResourceRequests
```

## <a name="request-headers"></a><span data-ttu-id="182ef-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="182ef-118">Request headers</span></span>

| <span data-ttu-id="182ef-119">Имя</span><span class="sxs-lookup"><span data-stu-id="182ef-119">Name</span></span>          | <span data-ttu-id="182ef-120">Описание</span><span class="sxs-lookup"><span data-stu-id="182ef-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="182ef-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="182ef-121">Authorization</span></span> | <span data-ttu-id="182ef-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="182ef-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="182ef-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="182ef-124">Content-Type</span></span>  | <span data-ttu-id="182ef-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="182ef-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="182ef-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="182ef-127">Request body</span></span>

<span data-ttu-id="182ef-128">В тексте запроса добавьте представление объекта [акцесспаккажересаурцерекуест](../resources/accesspackageresourcerequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="182ef-128">In the request body, supply a JSON representation of an [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.</span></span> <span data-ttu-id="182ef-129">Включение `accessPackageResource` связи с объектом [акцесспаккажересаурце](../resources/accesspackageresource.md) в составе запроса.</span><span class="sxs-lookup"><span data-stu-id="182ef-129">Include the `accessPackageResource` relationship with an [accessPackageResource](../resources/accesspackageresource.md) object as part of the request.</span></span>

<span data-ttu-id="182ef-130">Чтобы добавить группу Azure AD в качестве ресурса в каталог, значение свойства **оригинсистем** в `accessPackageResource` параметре должно иметь значение **аадграуп** , а значение **оригинид** — идентификатор группы.</span><span class="sxs-lookup"><span data-stu-id="182ef-130">To add an Azure AD group as a resource to a catalog, the value of the **originSystem** property within the `accessPackageResource` should be **AadGroup** and the value of the **originId** is the identifier of the group.</span></span>


## <a name="response"></a><span data-ttu-id="182ef-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="182ef-131">Response</span></span>

<span data-ttu-id="182ef-132">В случае успешного выполнения этот метод возвращает код ответа серии 200 и новый объект [акцесспаккажересаурцерекуест](../resources/accesspackageresourcerequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="182ef-132">If successful, this method returns a 200-series response code and a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="182ef-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="182ef-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="182ef-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="182ef-134">Request</span></span>

<span data-ttu-id="182ef-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="182ef-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="182ef-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="182ef-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerequest_from_accesspackageresourcerequests"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
Content-type: application/json

{
  "catalogId":"26ac0c0a-08bc-4a7b-a313-839f58044ba5",
  "requestType": "AdminAdd",
  "justification": "",
  "accessPackageResource": {
     "displayName": "Sales",
     "description": "https://contoso.sharepoint.com/sites/Sales",
     "url": "https://contoso.sharepoint.com/sites/Sales",
     "resourceType": "SharePoint Online Site",
     "originId": "https://contoso.sharepoint.com/sites/Sales",
     "originSystem": "SharePointOnline"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="182ef-137">C#</span><span class="sxs-lookup"><span data-stu-id="182ef-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="182ef-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="182ef-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="182ef-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="182ef-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="182ef-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="182ef-140">Response</span></span>

<span data-ttu-id="182ef-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="182ef-141">The following is an example of the response.</span></span>

> <span data-ttu-id="182ef-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="182ef-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "catalogId": "26ac0c0a-08bc-4a7b-a313-839f58044ba5",
  "id": "1fe272f0-d463-42aa-a9a8-b07ab50a1c4d",
  "isValidationOnly": false,
  "justification": "",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled",
  "requestType": "AdminAdd"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageResourceRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
