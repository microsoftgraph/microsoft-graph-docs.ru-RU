---
title: Перечисление объектов teamsApp
description: Список приложений Teams, опубликованных в каталоге приложений клиента.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e2980d91ae22764c8879df03d52bc5d0b120f1a3
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819780"
---
# <a name="list-teamsapp"></a><span data-ttu-id="900e1-103">Перечисление объектов teamsApp</span><span class="sxs-lookup"><span data-stu-id="900e1-103">List teamsApp</span></span>

<span data-ttu-id="900e1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="900e1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="900e1-105">Список [приложений,](../resources/teamsapp.md) опубликованных в каталоге приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="900e1-105">List [apps](../resources/teamsapp.md) published in the Microsoft Teams app catalog.</span></span> <span data-ttu-id="900e1-106">Сюда входят приложения из магазина Microsoft Teams, а также приложения из каталога приложений организации (каталога приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="900e1-106">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="900e1-107">Чтобы получать приложения только из каталога приложений организации, укажите `organization` **в качестве метода distributionMethod** в запросе.</span><span class="sxs-lookup"><span data-stu-id="900e1-107">To get apps from your organization's app catalog only, specify `organization` as the **distributionMethod** in the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="900e1-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="900e1-108">Permissions</span></span>

<span data-ttu-id="900e1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="900e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> <span data-ttu-id="900e1-111">**Примечание.** Этот API может вызывать только глобальные администраторы.</span><span class="sxs-lookup"><span data-stu-id="900e1-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="900e1-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="900e1-112">Permission Type</span></span>                        | <span data-ttu-id="900e1-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="900e1-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="900e1-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="900e1-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="900e1-115">AppCatalog.Read.All, AppCatalog.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="900e1-115">AppCatalog.Read.All, AppCatalog.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="900e1-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="900e1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="900e1-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="900e1-117">Not supported</span></span>                       |
| <span data-ttu-id="900e1-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="900e1-118">Application</span></span>                            | <span data-ttu-id="900e1-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="900e1-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="900e1-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="900e1-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="900e1-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="900e1-121">Optional query parameters</span></span>

<span data-ttu-id="900e1-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$filter`, `$select` и `$expand` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="900e1-122">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="900e1-123">При использовании возвращается дополнительная информация о состоянии приложения, например `$expand=AppDefinitions` **publishingState,** отражающем состояние проверки отправки приложения и возвращает сведения об утверждении, отклонении или остальном отзыве приложения.</span><span class="sxs-lookup"><span data-stu-id="900e1-123">Using `$expand=AppDefinitions` will return more information about the state of the app, such as the **publishingState**, which reflects the app submission review status and returns whether an app has been approved, rejected, or remains under review.</span></span> 

> <span data-ttu-id="900e1-124">**Примечание.** Вы можете отфильтровать любое из полей [объекта teamsApp,](../resources/teamsapp.md) чтобы сократить список результатов.</span><span class="sxs-lookup"><span data-stu-id="900e1-124">**Note:** You can filter on any of the fields of the [teamsApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="900e1-125">Можно использовать любую из следующих операций фильтрации: равное, не равно или нет.</span><span class="sxs-lookup"><span data-stu-id="900e1-125">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="request-headers"></a><span data-ttu-id="900e1-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="900e1-126">Request headers</span></span>

| <span data-ttu-id="900e1-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="900e1-127">Header</span></span>        | <span data-ttu-id="900e1-128">Значение</span><span class="sxs-lookup"><span data-stu-id="900e1-128">Value</span></span>                     |
|:--------------|:--------------------------|
| <span data-ttu-id="900e1-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="900e1-129">Authorization</span></span> | <span data-ttu-id="900e1-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="900e1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="900e1-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="900e1-132">Request body</span></span>

<span data-ttu-id="900e1-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="900e1-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="900e1-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="900e1-134">Response</span></span>

<span data-ttu-id="900e1-135">При успешном выполнении этот метод возвращает `200 OK` код ответа и список [объектов teamsApp](../resources/teamsapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="900e1-135">If successful, this method returns a `200 OK` response code and a list of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="900e1-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="900e1-136">Examples</span></span>

### <a name="example-1-list-all-applications-in-your-tenant"></a><span data-ttu-id="900e1-137">Пример 1. Перечисление всех приложений в клиенте</span><span class="sxs-lookup"><span data-stu-id="900e1-137">Example 1: List all applications in your tenant</span></span>

<span data-ttu-id="900e1-138">В примере ниже перечислены все приложения, характерные для вашего клиента.</span><span class="sxs-lookup"><span data-stu-id="900e1-138">The following example lists all apps that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="900e1-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="900e1-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```http
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApp?$filter=distributionMethod eq 'organization'
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="900e1-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="900e1-140">Response</span></span>

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

### <a name="example-2-list-applications-with-a-given-id"></a><span data-ttu-id="900e1-141">Пример 2. Перечисление приложений с данным идентификатором</span><span class="sxs-lookup"><span data-stu-id="900e1-141">Example 2: List applications with a given ID</span></span>

<span data-ttu-id="900e1-142">В следующем примере перечисляются приложения с заданным идентификатором.</span><span class="sxs-lookup"><span data-stu-id="900e1-142">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="900e1-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="900e1-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="900e1-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="900e1-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```
# <a name="c"></a>[<span data-ttu-id="900e1-145">C#</span><span class="sxs-lookup"><span data-stu-id="900e1-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="900e1-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="900e1-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="900e1-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="900e1-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="900e1-148">Java</span><span class="sxs-lookup"><span data-stu-id="900e1-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="900e1-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="900e1-149">Response</span></span>

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

### <a name="example-3-list-applications-with-a-given-id-and-return-the-submission-review-state"></a><span data-ttu-id="900e1-150">Пример 3. Перечисление приложений с данным идентификатором и возвращение состояния проверки отправки</span><span class="sxs-lookup"><span data-stu-id="900e1-150">Example 3: List applications with a given ID, and return the submission review state</span></span>

<span data-ttu-id="900e1-151">В следующем примере перечислены приложения с заданным идентификатором и **расширение appDefinitions** для **возвращения publishingState,** что отражает состояние проверки отправки приложения.</span><span class="sxs-lookup"><span data-stu-id="900e1-151">The following example lists applications with a given ID, and expands **appDefinitions** to return the **publishingState**, which reflects the app's submission review state.</span></span> <span data-ttu-id="900e1-152">`Submitted` означает, что отзыв ожидал, означает, что приложение было утверждено `published` администратором, а также отклонено `rejected` приложением администратором.</span><span class="sxs-lookup"><span data-stu-id="900e1-152">`Submitted` means the review is pending, `published` means the app was approved by the admin, and `rejected` means the app was rejected by the admin.</span></span>

#### <a name="request"></a><span data-ttu-id="900e1-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="900e1-153">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="900e1-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="900e1-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```msgraph-interactive
GET  https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=id eq '876df28f-2e78-423b-94a5-44181bd0e225'&$expand=appDefinitions
```
# <a name="c"></a>[<span data-ttu-id="900e1-155">C#</span><span class="sxs-lookup"><span data-stu-id="900e1-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="900e1-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="900e1-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="900e1-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="900e1-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="900e1-158">Java</span><span class="sxs-lookup"><span data-stu-id="900e1-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="900e1-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="900e1-159">Response</span></span>

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
