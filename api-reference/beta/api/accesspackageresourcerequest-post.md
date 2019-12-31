---
title: Создание Акцесспаккажересаурцерекуест
description: Создание нового Акцесспаккажересаурцерекуест.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d8e881cf57a7081b2967f2796c2b7d6de0c5ee11
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40911839"
---
# <a name="create-accesspackageresourcerequest"></a><span data-ttu-id="2321b-103">Создание Акцесспаккажересаурцерекуест</span><span class="sxs-lookup"><span data-stu-id="2321b-103">Create accessPackageResourceRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2321b-104">Создайте новый объект [акцесспаккажересаурцерекуест](../resources/accesspackageresourcerequest.md) , чтобы запросить Добавление ресурса в каталог пакетов Access.</span><span class="sxs-lookup"><span data-stu-id="2321b-104">Create a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object to request the addition of a resource to an access package catalog.</span></span>

## <a name="permissions"></a><span data-ttu-id="2321b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2321b-105">Permissions</span></span>

<span data-ttu-id="2321b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2321b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2321b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2321b-108">Permission type</span></span>                        | <span data-ttu-id="2321b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2321b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2321b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2321b-110">Delegated (work or school account)</span></span>     |  <span data-ttu-id="2321b-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2321b-111">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="2321b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2321b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2321b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2321b-113">Not supported.</span></span> |
| <span data-ttu-id="2321b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2321b-114">Application</span></span>                            | <span data-ttu-id="2321b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2321b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2321b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2321b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageResourceRequests
```

## <a name="request-headers"></a><span data-ttu-id="2321b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2321b-117">Request headers</span></span>

| <span data-ttu-id="2321b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2321b-118">Name</span></span>          | <span data-ttu-id="2321b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2321b-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2321b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2321b-120">Authorization</span></span> | <span data-ttu-id="2321b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2321b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2321b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2321b-123">Content-Type</span></span>  | <span data-ttu-id="2321b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2321b-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2321b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2321b-126">Request body</span></span>

<span data-ttu-id="2321b-127">В тексте запроса добавьте представление объекта [акцесспаккажересаурцерекуест](../resources/accesspackageresourcerequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2321b-127">In the request body, supply a JSON representation of an [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.</span></span> <span data-ttu-id="2321b-128">Включение `accessPackageResource` связи с объектом [акцесспаккажересаурце](../resources/accesspackageresource.md) в составе запроса.</span><span class="sxs-lookup"><span data-stu-id="2321b-128">Include the `accessPackageResource` relationship with an [accessPackageResource](../resources/accesspackageresource.md) object as part of the request.</span></span>

<span data-ttu-id="2321b-129">Чтобы добавить группу Azure AD в качестве ресурса в каталог, значение свойства **оригинсистем** в `accessPackageResource` параметре должно иметь значение **аадграуп** , а значение **оригинид** — идентификатор группы.</span><span class="sxs-lookup"><span data-stu-id="2321b-129">To add an Azure AD group as a resource to a catalog, the value of the **originSystem** property within the `accessPackageResource` should be **AadGroup** and the value of the **originId** is the identifier of the group.</span></span>


## <a name="response"></a><span data-ttu-id="2321b-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="2321b-130">Response</span></span>

<span data-ttu-id="2321b-131">В случае успешного выполнения этот метод возвращает код ответа серии 200 и новый объект [акцесспаккажересаурцерекуест](../resources/accesspackageresourcerequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2321b-131">If successful, this method returns a 200-series response code and a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2321b-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="2321b-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2321b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2321b-133">Request</span></span>

<span data-ttu-id="2321b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2321b-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2321b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="2321b-135">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="2321b-136">C#</span><span class="sxs-lookup"><span data-stu-id="2321b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2321b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2321b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2321b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2321b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2321b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="2321b-139">Response</span></span>

<span data-ttu-id="2321b-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2321b-140">The following is an example of the response.</span></span>

> <span data-ttu-id="2321b-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2321b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
