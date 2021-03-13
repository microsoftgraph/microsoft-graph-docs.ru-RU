---
title: Список accessPackageResourceEnvironments
description: Извлечение списка объектов accessPackageResourceEnvironment.
author: hanki-microsoft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 823abc8a71cfce4ac7872f4e6e86ae7d08e92411
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759414"
---
# <a name="list-accesspackageresourceenvironments"></a><span data-ttu-id="671a2-103">Список accessPackageResourceEnvironments</span><span class="sxs-lookup"><span data-stu-id="671a2-103">List accessPackageResourceEnvironments</span></span>
<span data-ttu-id="671a2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="671a2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="671a2-105">Извлечение списка [объектов accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="671a2-105">Retrieve a list of [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="671a2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="671a2-106">Permissions</span></span>
<span data-ttu-id="671a2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="671a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="671a2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="671a2-109">Permission type</span></span>|<span data-ttu-id="671a2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="671a2-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="671a2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="671a2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="671a2-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="671a2-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>|
|<span data-ttu-id="671a2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="671a2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="671a2-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="671a2-114">Not supported</span></span>|
|<span data-ttu-id="671a2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="671a2-115">Application</span></span>|<span data-ttu-id="671a2-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="671a2-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="671a2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="671a2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET identityGovernance/entitlementManagement/accessPackageResourceEnvironments?$filter=originSystem eq 'SharePointOnline'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="671a2-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="671a2-118">Optional query parameters</span></span>
<span data-ttu-id="671a2-119">Этот метод требует `$filter` [параметра запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="671a2-119">This method requires the `$filter` [OData query parameter](/graph/query-parameters).</span></span> <span data-ttu-id="671a2-120">Необходимо подать `$filter` заявление на набор **originSystem** для `eq` () `SharePointOnline` .</span><span class="sxs-lookup"><span data-stu-id="671a2-120">You must apply `$filter` for an **originSystem** set to (`eq`) `SharePointOnline`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="671a2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="671a2-121">Request headers</span></span>
|<span data-ttu-id="671a2-122">Имя</span><span class="sxs-lookup"><span data-stu-id="671a2-122">Name</span></span>|<span data-ttu-id="671a2-123">Описание</span><span class="sxs-lookup"><span data-stu-id="671a2-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="671a2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="671a2-124">Authorization</span></span>|<span data-ttu-id="671a2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="671a2-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="671a2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="671a2-127">Request body</span></span>
<span data-ttu-id="671a2-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="671a2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="671a2-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="671a2-129">Response</span></span>

<span data-ttu-id="671a2-130">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="671a2-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="671a2-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="671a2-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="671a2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="671a2-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="671a2-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="671a2-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accesspackageresourceenvironment"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceEnvironments?$filter=originSystem eq 'SharePointOnline'
```
# <a name="c"></a>[<span data-ttu-id="671a2-134">C#</span><span class="sxs-lookup"><span data-stu-id="671a2-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accesspackageresourceenvironment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="671a2-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="671a2-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accesspackageresourceenvironment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="671a2-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="671a2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accesspackageresourceenvironment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="671a2-137">Java</span><span class="sxs-lookup"><span data-stu-id="671a2-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accesspackageresourceenvironment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="671a2-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="671a2-138">Response</span></span>
<span data-ttu-id="671a2-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="671a2-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageResourceEnvironment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageResourceEnvironments",
  "value": [
    {
      "id": "615f2218-678f-471f-a60a-02c2f4f80c57",
      "displayName": "https://contoso.sharepoint.com/",
      "description": "https://contoso.sharepoint.com/",
      "originSystem": "SharePointOnline",
      "originId": "https://contoso-admin.sharepoint.com/",
      "isDefaultEnvironment": false,
      "connectionInfo": {
        "url": "https://contoso-admin.sharepoint.com/"
      }
    }
  ]
}
```

