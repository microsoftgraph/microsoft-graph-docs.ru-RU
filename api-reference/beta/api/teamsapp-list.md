---
title: Список teamsApp
description: 'Перечисление приложений из каталога приложений Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3fa9e49c35101cd151b18c4af9066d371b729bfc
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806306"
---
# <a name="list-teamsapp"></a><span data-ttu-id="889e6-103">Список teamsApp</span><span class="sxs-lookup"><span data-stu-id="889e6-103">List teamsApp</span></span>

<span data-ttu-id="889e6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="889e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="889e6-105">Перечисление [приложений](../resources/teamsapp.md) из каталога приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="889e6-105">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="889e6-106">Сюда входят приложения из магазина Microsoft Teams, а также приложения из каталога приложений организации (Каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="889e6-106">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="889e6-107">Чтобы получить доступ к приложениям только из каталога приложений вашей организации, укажите в `organization` качестве **distributionMethod** в запросе.</span><span class="sxs-lookup"><span data-stu-id="889e6-107">To get apps from your organization's app catalog only, specify `organization` as the **distributionMethod** in the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="889e6-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="889e6-108">Permissions</span></span>

<span data-ttu-id="889e6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="889e6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="889e6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="889e6-111">Permission Type</span></span>                        | <span data-ttu-id="889e6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="889e6-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="889e6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="889e6-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="889e6-114">CamlQuery. Read. ALL, CamlQuery. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="889e6-114">AppCatalog.Read.All, AppCatalog.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="889e6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="889e6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="889e6-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="889e6-116">Not supported</span></span>                       |
| <span data-ttu-id="889e6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="889e6-117">Application</span></span>                            | <span data-ttu-id="889e6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="889e6-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="889e6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="889e6-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="889e6-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="889e6-120">Optional query parameters</span></span>

<span data-ttu-id="889e6-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$filter`, `$select` и `$expand` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="889e6-121">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="889e6-122">Использование `$expand=AppDefinitions` возвращает дополнительные сведения о состоянии приложения, такие как **публишингстате**, которое отражает состояние проверки отправки приложения и возвращает сведения о том, утверждено ли приложение, отклонено или находится в процессе рассмотрения.</span><span class="sxs-lookup"><span data-stu-id="889e6-122">Using `$expand=AppDefinitions` will return more information about the state of the app, such as the **publishingState**, which reflects the app submission review status and returns whether an app has been approved, rejected, or remains under review.</span></span> 

> <span data-ttu-id="889e6-123">**Примечание:** Можно выполнить фильтрацию по любому полю объекта [teamsApp](../resources/teamsapp.md) для сокращения списка результатов.</span><span class="sxs-lookup"><span data-stu-id="889e6-123">**Note:** You can filter on any of the fields of the [teamsApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="889e6-124">Вы можете использовать любую из следующих операций фильтрации: EQUAL, Not Equals, and, OR и not.</span><span class="sxs-lookup"><span data-stu-id="889e6-124">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="request-headers"></a><span data-ttu-id="889e6-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="889e6-125">Request headers</span></span>

| <span data-ttu-id="889e6-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="889e6-126">Header</span></span>        | <span data-ttu-id="889e6-127">Значение</span><span class="sxs-lookup"><span data-stu-id="889e6-127">Value</span></span>                     |
|:--------------|:--------------------------|
| <span data-ttu-id="889e6-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="889e6-128">Authorization</span></span> | <span data-ttu-id="889e6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="889e6-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="889e6-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="889e6-131">Request body</span></span>

<span data-ttu-id="889e6-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="889e6-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="889e6-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="889e6-133">Response</span></span>

<span data-ttu-id="889e6-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список объектов [teamsApp](../resources/teamsapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="889e6-134">If successful, this method returns a `200 OK` response code and a list of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="889e6-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="889e6-135">Examples</span></span>

### <a name="example-1-list-all-applications-in-a-tenant"></a><span data-ttu-id="889e6-136">Пример 1: список всех приложений в клиенте</span><span class="sxs-lookup"><span data-stu-id="889e6-136">Example 1: List all applications in a tenant</span></span>

<span data-ttu-id="889e6-137">В приведенном ниже примере выводится список всех приложений, относящихся к вашему клиенту.</span><span class="sxs-lookup"><span data-stu-id="889e6-137">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="889e6-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="889e6-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="889e6-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="889e6-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```
# <a name="c"></a>[<span data-ttu-id="889e6-140">C#</span><span class="sxs-lookup"><span data-stu-id="889e6-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="889e6-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="889e6-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="889e6-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="889e6-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="889e6-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="889e6-143">Response</span></span>

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

### <a name="example-2-list-applications-with-a-given-id"></a><span data-ttu-id="889e6-144">Пример 2: список приложений с заданным ИДЕНТИФИКАТОРом</span><span class="sxs-lookup"><span data-stu-id="889e6-144">Example 2: List applications with a given ID</span></span>

<span data-ttu-id="889e6-145">В следующем примере перечисляются приложения с указанным ИДЕНТИФИКАТОРом.</span><span class="sxs-lookup"><span data-stu-id="889e6-145">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="889e6-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="889e6-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="889e6-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="889e6-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```
# <a name="c"></a>[<span data-ttu-id="889e6-148">C#</span><span class="sxs-lookup"><span data-stu-id="889e6-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="889e6-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="889e6-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="889e6-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="889e6-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="889e6-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="889e6-151">Response</span></span>

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

### <a name="example-3-list-applications-with-a-given-id-and-return-the-submission-review-state"></a><span data-ttu-id="889e6-152">Пример 3: перечисление приложений с заданным ИДЕНТИФИКАТОРом и возврат состояния проверки отправки</span><span class="sxs-lookup"><span data-stu-id="889e6-152">Example 3: List applications with a given ID, and return the submission review state</span></span>

<span data-ttu-id="889e6-153">В приведенном ниже примере перечисляются приложения с заданным ИДЕНТИФИКАТОРом, а затем **аппдефинитионс** возвращается значение **публишингстате**, которое отражает состояние проверки отправки приложения.</span><span class="sxs-lookup"><span data-stu-id="889e6-153">The following example lists applications with a given ID, and expands **appDefinitions** to return the **publishingState**, which reflects the app's submission review state.</span></span> <span data-ttu-id="889e6-154">`Submitted` означает, что проверка находится в состоянии ожидания, `published` означает, что приложение было утверждено администратором и `rejected` означает, что оно было отклонено администратором.</span><span class="sxs-lookup"><span data-stu-id="889e6-154">`Submitted` means the review is pending, `published` means the app was approved by the admin, and `rejected` means the app was rejected by the admin.</span></span>

#### <a name="request"></a><span data-ttu-id="889e6-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="889e6-155">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```http
GET  https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id eq '876df28f-2e78-423b-94a5-44181bd0e225'&$expand=appDefinitions
```

#### <a name="response"></a><span data-ttu-id="889e6-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="889e6-156">Response</span></span>

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
