---
title: Список teamsApp
description: 'Перечисление приложений из каталога приложений Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bd9dbcd409647f7597e6dc6bf57db81ae9d2e089
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981153"
---
# <a name="list-teamsapp"></a><span data-ttu-id="f36ca-103">Список teamsApp</span><span class="sxs-lookup"><span data-stu-id="f36ca-103">List teamsApp</span></span>

<span data-ttu-id="f36ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f36ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f36ca-105">Перечисление [приложений](../resources/teamsapp.md) из каталога приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f36ca-105">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="f36ca-106">Сюда входят приложения из магазина Microsoft Teams, а также приложения из каталога приложений организации (Каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="f36ca-106">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="f36ca-107">Чтобы получить доступ к приложениям только из каталога приложений вашей организации, укажите в `organization` качестве **distributionMethod** в запросе.</span><span class="sxs-lookup"><span data-stu-id="f36ca-107">To get apps from your organization's app catalog only, specify `organization` as the **distributionMethod** in the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="f36ca-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f36ca-108">Permissions</span></span>

<span data-ttu-id="f36ca-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f36ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f36ca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f36ca-111">Permission Type</span></span>                        | <span data-ttu-id="f36ca-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f36ca-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="f36ca-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f36ca-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f36ca-114">CamlQuery. Read. ALL, CamlQuery. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f36ca-114">AppCatalog.Read.All, AppCatalog.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="f36ca-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f36ca-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f36ca-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f36ca-116">Not supported</span></span>                       |
| <span data-ttu-id="f36ca-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f36ca-117">Application</span></span>                            | <span data-ttu-id="f36ca-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f36ca-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f36ca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f36ca-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f36ca-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f36ca-120">Optional query parameters</span></span>

<span data-ttu-id="f36ca-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$filter`, `$select` и `$expand` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f36ca-121">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="f36ca-122">Использование `$expand=AppDefinitions` возвращает дополнительные сведения о состоянии приложения, такие как **публишингстате** , которое отражает состояние проверки отправки приложения и возвращает сведения о том, утверждено ли приложение, отклонено или находится в процессе рассмотрения.</span><span class="sxs-lookup"><span data-stu-id="f36ca-122">Using `$expand=AppDefinitions` will return more information about the state of the app, such as the **publishingState** , which reflects the app submission review status and returns whether an app has been approved, rejected, or remains under review.</span></span> 

> <span data-ttu-id="f36ca-123">**Примечание:** Можно выполнить фильтрацию по любому полю объекта [teamsApp](../resources/teamsapp.md) для сокращения списка результатов.</span><span class="sxs-lookup"><span data-stu-id="f36ca-123">**Note:** You can filter on any of the fields of the [teamsApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="f36ca-124">Вы можете использовать любую из следующих операций фильтрации: EQUAL, Not Equals, and, OR и not.</span><span class="sxs-lookup"><span data-stu-id="f36ca-124">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f36ca-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f36ca-125">Request headers</span></span>

| <span data-ttu-id="f36ca-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f36ca-126">Header</span></span>        | <span data-ttu-id="f36ca-127">Значение</span><span class="sxs-lookup"><span data-stu-id="f36ca-127">Value</span></span>                     |
|:--------------|:--------------------------|
| <span data-ttu-id="f36ca-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f36ca-128">Authorization</span></span> | <span data-ttu-id="f36ca-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f36ca-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f36ca-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f36ca-131">Request body</span></span>

<span data-ttu-id="f36ca-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f36ca-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f36ca-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f36ca-133">Response</span></span>

<span data-ttu-id="f36ca-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список объектов [teamsApp](../resources/teamsapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f36ca-134">If successful, this method returns a `200 OK` response code and a list of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f36ca-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="f36ca-135">Examples</span></span>

### <a name="example-1-list-all-applications-in-a-tenant"></a><span data-ttu-id="f36ca-136">Пример 1: список всех приложений в клиенте</span><span class="sxs-lookup"><span data-stu-id="f36ca-136">Example 1: List all applications in a tenant</span></span>

<span data-ttu-id="f36ca-137">В приведенном ниже примере выводится список всех приложений, относящихся к вашему клиенту.</span><span class="sxs-lookup"><span data-stu-id="f36ca-137">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="f36ca-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="f36ca-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f36ca-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="f36ca-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```
# <a name="c"></a>[<span data-ttu-id="f36ca-140">C#</span><span class="sxs-lookup"><span data-stu-id="f36ca-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f36ca-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f36ca-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f36ca-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f36ca-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f36ca-143">Java</span><span class="sxs-lookup"><span data-stu-id="f36ca-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="f36ca-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="f36ca-144">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization"
    }
  ]
}
```

### <a name="example-2-list-applications-with-a-given-id"></a><span data-ttu-id="f36ca-145">Пример 2: список приложений с заданным ИДЕНТИФИКАТОРом</span><span class="sxs-lookup"><span data-stu-id="f36ca-145">Example 2: List applications with a given ID</span></span>

<span data-ttu-id="f36ca-146">В следующем примере перечисляются приложения с указанным ИДЕНТИФИКАТОРом.</span><span class="sxs-lookup"><span data-stu-id="f36ca-146">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="f36ca-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="f36ca-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f36ca-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="f36ca-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```
# <a name="c"></a>[<span data-ttu-id="f36ca-149">C#</span><span class="sxs-lookup"><span data-stu-id="f36ca-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f36ca-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f36ca-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f36ca-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f36ca-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f36ca-152">Java</span><span class="sxs-lookup"><span data-stu-id="f36ca-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f36ca-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="f36ca-153">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization"
    }
  ]
}
```

### <a name="example-3-list-applications-with-a-given-id-and-return-the-submission-review-state"></a><span data-ttu-id="f36ca-154">Пример 3: перечисление приложений с заданным ИДЕНТИФИКАТОРом и возврат состояния проверки отправки</span><span class="sxs-lookup"><span data-stu-id="f36ca-154">Example 3: List applications with a given ID, and return the submission review state</span></span>

<span data-ttu-id="f36ca-155">В приведенном ниже примере перечисляются приложения с заданным ИДЕНТИФИКАТОРом, а затем **аппдефинитионс** возвращается значение **публишингстате** , которое отражает состояние проверки отправки приложения.</span><span class="sxs-lookup"><span data-stu-id="f36ca-155">The following example lists applications with a given ID, and expands **appDefinitions** to return the **publishingState** , which reflects the app's submission review state.</span></span> <span data-ttu-id="f36ca-156">`Submitted` означает, что проверка находится в состоянии ожидания, `published` означает, что приложение было утверждено администратором и `rejected` означает, что оно было отклонено администратором.</span><span class="sxs-lookup"><span data-stu-id="f36ca-156">`Submitted` means the review is pending, `published` means the app was approved by the admin, and `rejected` means the app was rejected by the admin.</span></span>

#### <a name="request"></a><span data-ttu-id="f36ca-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="f36ca-157">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f36ca-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="f36ca-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```msgraph-interactive
GET  https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id eq '876df28f-2e78-423b-94a5-44181bd0e225'&$expand=appDefinitions
```
# <a name="c"></a>[<span data-ttu-id="f36ca-159">C#</span><span class="sxs-lookup"><span data-stu-id="f36ca-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f36ca-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f36ca-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f36ca-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f36ca-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f36ca-162">Java</span><span class="sxs-lookup"><span data-stu-id="f36ca-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f36ca-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="f36ca-163">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "876df28f-2e78-423b-94a5-44181bd0e225",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization",
      "appDefinitions": [
                {

                    "id": "NGQyMGNiNDUtZWViYS00ZTEyLWE3YzktMGQ0NDgzYjYxNzU2IyMxLjAuMA==",

                    "teamsAppId": "876df28f-2e78-423b-94a5-44181bd0e225",

                    "azureADAppId": null,

                    "displayName": "Test App",

                    "version": "1.0.1",

                    "requiredResourceSpecificApplicationPermissions": [],

                    "publishingState": "published"

                  }
            ]
      }
    ]
  }
```


