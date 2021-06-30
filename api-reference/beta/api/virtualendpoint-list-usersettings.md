---
title: Список userSettings
description: Извлечение списка объектов cloudPcUserSetting.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 2a5665a1e1043296f3814bdc301c8f3c6b339655
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208426"
---
# <a name="list-usersettings"></a><span data-ttu-id="90e61-103">Список userSettings</span><span class="sxs-lookup"><span data-stu-id="90e61-103">List userSettings</span></span>

<span data-ttu-id="90e61-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90e61-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90e61-105">Извлечение списка [объектов cloudPcUserSetting.](../resources/cloudpcusersetting.md)</span><span class="sxs-lookup"><span data-stu-id="90e61-105">Retrieve a list of [cloudPcUserSetting](../resources/cloudpcusersetting.md) objects.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="90e61-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90e61-106">Permissions</span></span>

<span data-ttu-id="90e61-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90e61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90e61-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90e61-109">Permission type</span></span>|<span data-ttu-id="90e61-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90e61-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90e61-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90e61-111">Delegated (work or school account)</span></span>|<span data-ttu-id="90e61-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90e61-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="90e61-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90e61-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90e61-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90e61-114">Not supported.</span></span>|
|<span data-ttu-id="90e61-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="90e61-115">Application</span></span>|<span data-ttu-id="90e61-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90e61-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90e61-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90e61-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/userSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="90e61-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="90e61-118">Optional query parameters</span></span>

<span data-ttu-id="90e61-119">Этот метод поддерживает `$select` и `$filter` `$expand` параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="90e61-119">This method the supports `$select`, `$filter`, and `$expand` OData query parameters to help customize the response.</span></span> <span data-ttu-id="90e61-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="90e61-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="90e61-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90e61-121">Request headers</span></span>

| <span data-ttu-id="90e61-122">Имя</span><span class="sxs-lookup"><span data-stu-id="90e61-122">Name</span></span>          | <span data-ttu-id="90e61-123">Описание</span><span class="sxs-lookup"><span data-stu-id="90e61-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="90e61-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90e61-124">Authorization</span></span> | <span data-ttu-id="90e61-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90e61-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90e61-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90e61-127">Request body</span></span>

<span data-ttu-id="90e61-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90e61-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90e61-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="90e61-129">Response</span></span>

<span data-ttu-id="90e61-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [cloudPcUserSetting](../resources/cloudpcusersetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="90e61-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPcUserSetting](../resources/cloudpcusersetting.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="90e61-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="90e61-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="90e61-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="90e61-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="90e61-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="90e61-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcusersetting"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings
```
# <a name="c"></a>[<span data-ttu-id="90e61-134">C#</span><span class="sxs-lookup"><span data-stu-id="90e61-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcusersetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="90e61-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90e61-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcusersetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90e61-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90e61-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcusersetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="90e61-137">Java</span><span class="sxs-lookup"><span data-stu-id="90e61-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcusersetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="90e61-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="90e61-138">Response</span></span>
><span data-ttu-id="90e61-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="90e61-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPcUserSetting)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPcUserSetting",
      "id": "556092f8-92f8-5560-f892-6055f8926055",
      "displayName": "Test1",
      "selfServiceEnabled": true,
      "localAdminEnabled": false,
      "lastModifiedDateTime": "2021-02-01T10:29:57Z",
      "createdDateTime": "2021-02-01T10:29:57Z"
    }
  ]
}
```
