---
title: Список teamsApp
description: Список приложений Teams, опубликованных в каталоге приложений клиента.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 794cb72014d2021b7eec0f46937b1597607a0d64
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904758"
---
# <a name="list-teamsapp"></a><span data-ttu-id="5c5bb-103">Список teamsApp</span><span class="sxs-lookup"><span data-stu-id="5c5bb-103">List teamsApp</span></span>

<span data-ttu-id="5c5bb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c5bb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5c5bb-105">Список [приложений](../resources/teamsapp.md) , опубликованных в каталоге приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="5c5bb-105">List [apps](../resources/teamsapp.md) published in the Microsoft Teams app catalog.</span></span> <span data-ttu-id="5c5bb-106">Сюда входят приложения из магазина Microsoft Teams, а также приложения из каталога приложений организации (Каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="5c5bb-106">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="5c5bb-107">Чтобы получить доступ к приложениям только из каталога приложений вашей организации, укажите в `organization` качестве **distributionMethod** в запросе.</span><span class="sxs-lookup"><span data-stu-id="5c5bb-107">To get apps from your organization's app catalog only, specify `organization` as the **distributionMethod** in the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c5bb-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5c5bb-108">Permissions</span></span>

<span data-ttu-id="5c5bb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c5bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> <span data-ttu-id="5c5bb-111">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="5c5bb-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="5c5bb-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c5bb-112">Permission Type</span></span>                        | <span data-ttu-id="5c5bb-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c5bb-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="5c5bb-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c5bb-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="5c5bb-115">CamlQuery. Read. ALL, CamlQuery. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5c5bb-115">AppCatalog.Read.All, AppCatalog.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="5c5bb-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c5bb-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c5bb-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5c5bb-117">Not supported</span></span>                       |
| <span data-ttu-id="5c5bb-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c5bb-118">Application</span></span>                            | <span data-ttu-id="5c5bb-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c5bb-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c5bb-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c5bb-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5c5bb-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5c5bb-121">Optional query parameters</span></span>

<span data-ttu-id="5c5bb-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$filter`, `$select` и `$expand` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="5c5bb-122">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="5c5bb-123">При использовании `$expand=AppDefinitions` будут возвращены дополнительные сведения о состоянии приложения.</span><span class="sxs-lookup"><span data-stu-id="5c5bb-123">Using `$expand=AppDefinitions` will return more information about the state of the app.</span></span> 

> <span data-ttu-id="5c5bb-124">**Примечание:** Можно выполнить фильтрацию по любому полю объекта [teamsApp](../resources/teamsapp.md) для сокращения списка результатов.</span><span class="sxs-lookup"><span data-stu-id="5c5bb-124">**Note:** You can filter on any of the fields of the [teamsApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="5c5bb-125">Вы можете использовать любую из следующих операций фильтрации: EQUAL, Not Equals, and, OR и not.</span><span class="sxs-lookup"><span data-stu-id="5c5bb-125">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c5bb-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c5bb-126">Request headers</span></span>

| <span data-ttu-id="5c5bb-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c5bb-127">Header</span></span>        | <span data-ttu-id="5c5bb-128">Значение</span><span class="sxs-lookup"><span data-stu-id="5c5bb-128">Value</span></span>                     |
|:--------------|:--------------------------|
| <span data-ttu-id="5c5bb-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c5bb-129">Authorization</span></span> | <span data-ttu-id="5c5bb-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c5bb-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c5bb-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5c5bb-132">Request body</span></span>

<span data-ttu-id="5c5bb-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5c5bb-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c5bb-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c5bb-134">Response</span></span>

<span data-ttu-id="5c5bb-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список объектов [teamsApp](../resources/teamsapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5c5bb-135">If successful, this method returns a `200 OK` response code and a list of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5c5bb-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="5c5bb-136">Examples</span></span>

### <a name="example-1-list-all-applications-in-your-tenant"></a><span data-ttu-id="5c5bb-137">Пример 1: список всех приложений в клиенте</span><span class="sxs-lookup"><span data-stu-id="5c5bb-137">Example 1: List all applications in your tenant</span></span>

<span data-ttu-id="5c5bb-138">В следующем примере перечисляются все приложения, характерные для вашего клиента.</span><span class="sxs-lookup"><span data-stu-id="5c5bb-138">The following example lists all apps that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="5c5bb-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c5bb-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApp?$filter=distributionMethod eq 'organization'
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="5c5bb-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c5bb-140">Response</span></span>

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

### <a name="example-2-list-applications-with-a-given-id"></a><span data-ttu-id="5c5bb-141">Пример 2: список приложений с заданным ИДЕНТИФИКАТОРом</span><span class="sxs-lookup"><span data-stu-id="5c5bb-141">Example 2: List applications with a given ID</span></span>

<span data-ttu-id="5c5bb-142">В следующем примере перечисляются приложения с указанным ИДЕНТИФИКАТОРом.</span><span class="sxs-lookup"><span data-stu-id="5c5bb-142">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="5c5bb-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c5bb-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5c5bb-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c5bb-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```
# <a name="c"></a>[<span data-ttu-id="5c5bb-145">C#</span><span class="sxs-lookup"><span data-stu-id="5c5bb-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c5bb-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c5bb-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c5bb-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c5bb-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c5bb-148">Java</span><span class="sxs-lookup"><span data-stu-id="5c5bb-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5c5bb-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c5bb-149">Response</span></span>

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
