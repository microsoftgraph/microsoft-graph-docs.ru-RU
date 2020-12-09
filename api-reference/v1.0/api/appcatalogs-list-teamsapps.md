---
title: Список teamsApp
description: Список приложений Teams, опубликованных в каталоге приложений клиента.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fa54d1ac1eec5dfc0a6995f85ced9f46fa8d47ae
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607436"
---
# <a name="list-teamsapp"></a><span data-ttu-id="bf634-103">Список teamsApp</span><span class="sxs-lookup"><span data-stu-id="bf634-103">List teamsApp</span></span>

<span data-ttu-id="bf634-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf634-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bf634-105">Список [приложений](../resources/teamsapp.md) , опубликованных в каталоге приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="bf634-105">List [apps](../resources/teamsapp.md) published in the Microsoft Teams app catalog.</span></span> <span data-ttu-id="bf634-106">Сюда входят приложения из магазина Microsoft Teams, а также приложения из каталога приложений организации (Каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="bf634-106">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="bf634-107">Чтобы получить доступ к приложениям только из каталога приложений вашей организации, укажите в `organization` качестве **distributionMethod** в запросе.</span><span class="sxs-lookup"><span data-stu-id="bf634-107">To get apps from your organization's app catalog only, specify `organization` as the **distributionMethod** in the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf634-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bf634-108">Permissions</span></span>

<span data-ttu-id="bf634-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf634-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> <span data-ttu-id="bf634-111">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="bf634-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="bf634-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf634-112">Permission Type</span></span>                        | <span data-ttu-id="bf634-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf634-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="bf634-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf634-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="bf634-115">CamlQuery. Read. ALL, CamlQuery. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="bf634-115">AppCatalog.Read.All, AppCatalog.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="bf634-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf634-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf634-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="bf634-117">Not supported</span></span>                       |
| <span data-ttu-id="bf634-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf634-118">Application</span></span>                            | <span data-ttu-id="bf634-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf634-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf634-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf634-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bf634-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bf634-121">Optional query parameters</span></span>

<span data-ttu-id="bf634-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$filter`, `$select` и `$expand` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="bf634-122">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="bf634-123">При использовании `$expand=AppDefinitions` будут возвращены дополнительные сведения о состоянии приложения.</span><span class="sxs-lookup"><span data-stu-id="bf634-123">Using `$expand=AppDefinitions` will return more information about the state of the app.</span></span> 

> <span data-ttu-id="bf634-124">**Примечание:** Можно выполнить фильтрацию по любому полю объекта [teamsApp](../resources/teamsapp.md) для сокращения списка результатов.</span><span class="sxs-lookup"><span data-stu-id="bf634-124">**Note:** You can filter on any of the fields of the [teamsApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="bf634-125">Вы можете использовать любую из следующих операций фильтрации: EQUAL, Not Equals, and, OR и not.</span><span class="sxs-lookup"><span data-stu-id="bf634-125">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bf634-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf634-126">Request headers</span></span>

| <span data-ttu-id="bf634-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bf634-127">Header</span></span>        | <span data-ttu-id="bf634-128">Значение</span><span class="sxs-lookup"><span data-stu-id="bf634-128">Value</span></span>                     |
|:--------------|:--------------------------|
| <span data-ttu-id="bf634-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf634-129">Authorization</span></span> | <span data-ttu-id="bf634-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf634-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bf634-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf634-132">Request body</span></span>

<span data-ttu-id="bf634-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bf634-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf634-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf634-134">Response</span></span>

<span data-ttu-id="bf634-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список объектов [teamsApp](../resources/teamsapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bf634-135">If successful, this method returns a `200 OK` response code and a list of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bf634-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="bf634-136">Examples</span></span>

### <a name="example-1-list-all-applications-specific-to-the-tenant"></a><span data-ttu-id="bf634-137">Пример 1: список всех приложений, относящихся к клиенту</span><span class="sxs-lookup"><span data-stu-id="bf634-137">Example 1: List all applications specific to the tenant</span></span>

<span data-ttu-id="bf634-138">В приведенном ниже примере выводится список всех приложений, относящихся к вашему клиенту.</span><span class="sxs-lookup"><span data-stu-id="bf634-138">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="bf634-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf634-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_teamsapps_filter_distributionMethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```



<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="bf634-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf634-140">Response</span></span>

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

### <a name="example-2-list-applications-with-a-given-id"></a><span data-ttu-id="bf634-141">Пример 2: список приложений с заданным ИДЕНТИФИКАТОРом</span><span class="sxs-lookup"><span data-stu-id="bf634-141">Example 2: List applications with a given ID</span></span>

<span data-ttu-id="bf634-142">В следующем примере перечисляются приложения с указанным ИДЕНТИФИКАТОРом.</span><span class="sxs-lookup"><span data-stu-id="bf634-142">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="bf634-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf634-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_teamsapp_filter_id"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="bf634-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf634-144">Response</span></span>

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
### <a name="example-3-find-application-based-on-the-teams-app-manifest-id"></a><span data-ttu-id="bf634-145">Пример 3: Find Application на основе идентификатора манифеста приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="bf634-145">Example 3: Find application based on the Teams app manifest ID.</span></span>

<span data-ttu-id="bf634-146">В следующем примере перечисляются приложения, которые совпадают с идентификатором "ID", указанным в манифесте приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="bf634-146">The following example lists applications that match the 'id' specified in the Teams app manifest.</span></span> <span data-ttu-id="bf634-147">В этом примере идентификатор манифеста приложения Teams — "cf1ba4c7-f94e-4d80-ba90-5594b641a8ee".</span><span class="sxs-lookup"><span data-stu-id="bf634-147">In the example, the manifest ID of the Teams app is 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'.</span></span>

#### <a name="request"></a><span data-ttu-id="bf634-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf634-148">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_teamsapp_filter_externalid"
}-->

```msgraph-interactive
GET  https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'
```

#### <a name="response"></a><span data-ttu-id="bf634-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf634-149">Response</span></span>

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

## <a name="see-also"></a><span data-ttu-id="bf634-150">См. также</span><span class="sxs-lookup"><span data-stu-id="bf634-150">See also</span></span>

- [<span data-ttu-id="bf634-151">Список приложений, установленных в команде</span><span class="sxs-lookup"><span data-stu-id="bf634-151">List apps installed in a team</span></span>](team-list-installedapps.md)
- [<span data-ttu-id="bf634-152">Список приложений, установленных в личной области пользователя</span><span class="sxs-lookup"><span data-stu-id="bf634-152">List apps installed in the personal scope of a user</span></span>](userteamwork-list-installedapps.md)

