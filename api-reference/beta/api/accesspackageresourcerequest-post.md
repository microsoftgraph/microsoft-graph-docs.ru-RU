---
title: Создание Акцесспаккажересаурцерекуест
description: Создание нового Акцесспаккажересаурцерекуест.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 46b40c4650890db6a506fce0c8422cea07a4f5c1
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871901"
---
# <a name="create-accesspackageresourcerequest"></a><span data-ttu-id="ab4df-103">Создание Акцесспаккажересаурцерекуест</span><span class="sxs-lookup"><span data-stu-id="ab4df-103">Create accessPackageResourceRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab4df-104">Создайте новый объект [акцесспаккажересаурцерекуест](../resources/accesspackageresourcerequest.md) , чтобы запросить Добавление ресурса в каталог пакетов Access.</span><span class="sxs-lookup"><span data-stu-id="ab4df-104">Create a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object to request the addition of a resource to an access package catalog.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab4df-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ab4df-105">Permissions</span></span>

<span data-ttu-id="ab4df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab4df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ab4df-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab4df-108">Permission type</span></span>                        | <span data-ttu-id="ab4df-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab4df-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ab4df-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab4df-110">Delegated (work or school account)</span></span>     |  <span data-ttu-id="ab4df-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab4df-111">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="ab4df-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab4df-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab4df-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab4df-113">Not supported.</span></span> |
| <span data-ttu-id="ab4df-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab4df-114">Application</span></span>                            | <span data-ttu-id="ab4df-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab4df-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab4df-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab4df-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageResourceRequests
```

## <a name="request-headers"></a><span data-ttu-id="ab4df-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab4df-117">Request headers</span></span>

| <span data-ttu-id="ab4df-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ab4df-118">Name</span></span>          | <span data-ttu-id="ab4df-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ab4df-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ab4df-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab4df-120">Authorization</span></span> | <span data-ttu-id="ab4df-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab4df-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ab4df-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ab4df-123">Content-Type</span></span>  | <span data-ttu-id="ab4df-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab4df-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ab4df-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab4df-126">Request body</span></span>

<span data-ttu-id="ab4df-127">В тексте запроса добавьте представление объекта [акцесспаккажересаурцерекуест](../resources/accesspackageresourcerequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab4df-127">In the request body, supply a JSON representation of an [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.</span></span> <span data-ttu-id="ab4df-128">Включение `accessPackageResource` связи с объектом [акцесспаккажересаурце](../resources/accesspackageresource.md) в составе запроса.</span><span class="sxs-lookup"><span data-stu-id="ab4df-128">Include the `accessPackageResource` relationship with an [accessPackageResource](../resources/accesspackageresource.md) object as part of the request.</span></span>

<span data-ttu-id="ab4df-129">Чтобы добавить группу Azure AD в качестве ресурса в каталог, значение свойства **оригинсистем** в `accessPackageResource` параметре должно иметь значение **аадграуп** , а значение **оригинид** — идентификатор группы.</span><span class="sxs-lookup"><span data-stu-id="ab4df-129">To add an Azure AD group as a resource to a catalog, the value of the **originSystem** property within the `accessPackageResource` should be **AadGroup** and the value of the **originId** is the identifier of the group.</span></span>


## <a name="response"></a><span data-ttu-id="ab4df-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab4df-130">Response</span></span>

<span data-ttu-id="ab4df-131">В случае успешного выполнения этот метод возвращает код ответа серии 200 и новый объект [акцесспаккажересаурцерекуест](../resources/accesspackageresourcerequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ab4df-131">If successful, this method returns a 200-series response code and a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ab4df-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="ab4df-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ab4df-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab4df-133">Request</span></span>

<span data-ttu-id="ab4df-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab4df-134">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ab4df-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab4df-135">Response</span></span>

<span data-ttu-id="ab4df-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ab4df-136">The following is an example of the response.</span></span>

> <span data-ttu-id="ab4df-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ab4df-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
