---
title: Список teamsApp
description: Список приложений Teams, опубликованных в каталоге приложений клиента.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 35a922e2ed7fd3ccd4c41d19173199d243bb3192
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690393"
---
# <a name="list-teamsapp"></a><span data-ttu-id="079d4-103">Список teamsApp</span><span class="sxs-lookup"><span data-stu-id="079d4-103">List teamsApp</span></span>

<span data-ttu-id="079d4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="079d4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="079d4-105">Список [приложений,](../resources/teamsapp.md) опубликованных в каталоге приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="079d4-105">List [apps](../resources/teamsapp.md) published in the Microsoft Teams app catalog.</span></span> <span data-ttu-id="079d4-106">К ним относятся приложения из Магазина Microsoft Teams, а также приложения из каталога приложений вашей организации (каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="079d4-106">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="079d4-107">Чтобы получить приложения только из каталога приложений организации, укажите `organization` в качестве **distributionMethod** в запросе.</span><span class="sxs-lookup"><span data-stu-id="079d4-107">To get apps from your organization's app catalog only, specify `organization` as the **distributionMethod** in the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="079d4-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="079d4-108">Permissions</span></span>

<span data-ttu-id="079d4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="079d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> <span data-ttu-id="079d4-111">**Примечание.** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="079d4-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="079d4-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="079d4-112">Permission Type</span></span>                        | <span data-ttu-id="079d4-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="079d4-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="079d4-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="079d4-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="079d4-115">AppCatalog.Read.All, AppCatalog.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="079d4-115">AppCatalog.Read.All, AppCatalog.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="079d4-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="079d4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="079d4-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="079d4-117">Not supported</span></span>                       |
| <span data-ttu-id="079d4-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="079d4-118">Application</span></span>                            | <span data-ttu-id="079d4-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="079d4-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="079d4-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="079d4-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="079d4-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="079d4-121">Optional query parameters</span></span>

<span data-ttu-id="079d4-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$filter`, `$select` и `$expand` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="079d4-122">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="079d4-123">При `$expand=AppDefinitions` использовании будут возвращены дополнительные сведения о состоянии приложения.</span><span class="sxs-lookup"><span data-stu-id="079d4-123">Using `$expand=AppDefinitions` will return more information about the state of the app.</span></span> 

> <span data-ttu-id="079d4-124">**Примечание.** Можно отфильтровать любые поля объекта [teamsApp,](../resources/teamsapp.md) чтобы сократить список результатов.</span><span class="sxs-lookup"><span data-stu-id="079d4-124">**Note:** You can filter on any of the fields of the [teamsApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="079d4-125">Можно использовать любую из следующих операций фильтра: "Равно", "не равно" и "или" или "нет".</span><span class="sxs-lookup"><span data-stu-id="079d4-125">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="request-headers"></a><span data-ttu-id="079d4-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="079d4-126">Request headers</span></span>

| <span data-ttu-id="079d4-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="079d4-127">Header</span></span>        | <span data-ttu-id="079d4-128">Значение</span><span class="sxs-lookup"><span data-stu-id="079d4-128">Value</span></span>                     |
|:--------------|:--------------------------|
| <span data-ttu-id="079d4-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="079d4-129">Authorization</span></span> | <span data-ttu-id="079d4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="079d4-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="079d4-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="079d4-132">Request body</span></span>

<span data-ttu-id="079d4-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="079d4-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="079d4-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="079d4-134">Response</span></span>

<span data-ttu-id="079d4-135">В случае успеха этот метод возвращает код отклика и список объектов `200 OK` [teamsApp](../resources/teamsapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="079d4-135">If successful, this method returns a `200 OK` response code and a list of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="079d4-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="079d4-136">Examples</span></span>

### <a name="example-1-list-all-applications-specific-to-the-tenant"></a><span data-ttu-id="079d4-137">Пример 1. Список всех приложений, характерных для клиента</span><span class="sxs-lookup"><span data-stu-id="079d4-137">Example 1: List all applications specific to the tenant</span></span>

<span data-ttu-id="079d4-138">В следующем примере перечислены все приложения, которые являются специфическими для вашего клиента.</span><span class="sxs-lookup"><span data-stu-id="079d4-138">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="079d4-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="079d4-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="079d4-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="079d4-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapps_filter_distributionMethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```
# <a name="c"></a>[<span data-ttu-id="079d4-141">C#</span><span class="sxs-lookup"><span data-stu-id="079d4-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapps-filter-distributionmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="079d4-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="079d4-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapps-filter-distributionmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="079d4-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="079d4-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapps-filter-distributionmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="079d4-144">Java</span><span class="sxs-lookup"><span data-stu-id="079d4-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapps-filter-distributionmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="079d4-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="079d4-145">Response</span></span>

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

### <a name="example-2-list-applications-with-a-given-id"></a><span data-ttu-id="079d4-146">Пример 2. Список приложений с заданным ИД</span><span class="sxs-lookup"><span data-stu-id="079d4-146">Example 2: List applications with a given ID</span></span>

<span data-ttu-id="079d4-147">В следующем примере перечислены приложения с заданным ИД.</span><span class="sxs-lookup"><span data-stu-id="079d4-147">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="079d4-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="079d4-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="079d4-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="079d4-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp_filter_id"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```
# <a name="c"></a>[<span data-ttu-id="079d4-150">C#</span><span class="sxs-lookup"><span data-stu-id="079d4-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-filter-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="079d4-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="079d4-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-filter-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="079d4-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="079d4-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-filter-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="079d4-153">Java</span><span class="sxs-lookup"><span data-stu-id="079d4-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapp-filter-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="079d4-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="079d4-154">Response</span></span>

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
### <a name="example-3-find-application-based-on-the-teams-app-manifest-id"></a><span data-ttu-id="079d4-155">Пример 3. Поиск приложения на основе ИД манифеста приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="079d4-155">Example 3: Find application based on the Teams app manifest ID.</span></span>

<span data-ttu-id="079d4-156">В следующем примере перечислены приложения, которые соответствуют "id", указанному в манифесте приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="079d4-156">The following example lists applications that match the 'id' specified in the Teams app manifest.</span></span> <span data-ttu-id="079d4-157">В этом примере идентификатор манифеста приложения Teams — 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'.</span><span class="sxs-lookup"><span data-stu-id="079d4-157">In the example, the manifest ID of the Teams app is 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'.</span></span>

#### <a name="request"></a><span data-ttu-id="079d4-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="079d4-158">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="079d4-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="079d4-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp_filter_externalid"
}-->

```msgraph-interactive
GET  https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'
```
# <a name="c"></a>[<span data-ttu-id="079d4-160">C#</span><span class="sxs-lookup"><span data-stu-id="079d4-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-filter-externalid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="079d4-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="079d4-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-filter-externalid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="079d4-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="079d4-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-filter-externalid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="079d4-163">Java</span><span class="sxs-lookup"><span data-stu-id="079d4-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapp-filter-externalid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="079d4-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="079d4-164">Response</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#appCatalogs/teamsApps",
    "value": [
        {
            "id": "22f73bbe-f67a-4dea-bd54-54cac718cb2b",
            "externalId": "cf1ba4c7-f94e-4d80-ba90-5594b641a8ee",
            "displayName": "YPA",
            "distributionMethod": "organization"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="079d4-165">См. также</span><span class="sxs-lookup"><span data-stu-id="079d4-165">See also</span></span>

- [<span data-ttu-id="079d4-166">Список приложений, установленных в команде</span><span class="sxs-lookup"><span data-stu-id="079d4-166">List apps installed in a team</span></span>](team-list-installedapps.md)
- [<span data-ttu-id="079d4-167">Список приложений, установленных в личной области пользователя</span><span class="sxs-lookup"><span data-stu-id="079d4-167">List apps installed in the personal scope of a user</span></span>](userteamwork-list-installedapps.md)

