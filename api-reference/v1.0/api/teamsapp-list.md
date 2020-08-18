---
title: Список teamsApp
description: Список приложений Teams, опубликованных в каталоге приложений клиента.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 613011ce44b05b1743a8d297fc63450d4eed7dee
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790744"
---
# <a name="list-teamsapp"></a><span data-ttu-id="28ee2-103">Список teamsApp</span><span class="sxs-lookup"><span data-stu-id="28ee2-103">List teamsApp</span></span>

<span data-ttu-id="28ee2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28ee2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="28ee2-105">Список [приложений](../resources/teamsapp.md) , опубликованных в каталоге приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="28ee2-105">List [apps](../resources/teamsapp.md) published in the Microsoft Teams app catalog.</span></span> <span data-ttu-id="28ee2-106">Сюда входят приложения из магазина Microsoft Teams, а также приложения из каталога приложений организации (Каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="28ee2-106">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="28ee2-107">Чтобы получить доступ к приложениям только из каталога приложений вашей организации, укажите в `organization` качестве **distributionMethod** в запросе.</span><span class="sxs-lookup"><span data-stu-id="28ee2-107">To get apps from your organization's app catalog only, specify `organization` as the **distributionMethod** in the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="28ee2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="28ee2-108">Permissions</span></span>

<span data-ttu-id="28ee2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28ee2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> <span data-ttu-id="28ee2-111">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="28ee2-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="28ee2-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28ee2-112">Permission Type</span></span>                        | <span data-ttu-id="28ee2-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28ee2-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="28ee2-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28ee2-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="28ee2-115">CamlQuery. Read. ALL, CamlQuery. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="28ee2-115">AppCatalog.Read.All, AppCatalog.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="28ee2-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28ee2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28ee2-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="28ee2-117">Not supported</span></span>                       |
| <span data-ttu-id="28ee2-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28ee2-118">Application</span></span>                            | <span data-ttu-id="28ee2-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28ee2-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="28ee2-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28ee2-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="28ee2-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="28ee2-121">Optional query parameters</span></span>

<span data-ttu-id="28ee2-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$filter`, `$select` и `$expand` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="28ee2-122">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

> <span data-ttu-id="28ee2-123">**Примечание:** Можно выполнить фильтрацию по любому полю объекта [teamsApp](../resources/teamsapp.md) для сокращения списка результатов.</span><span class="sxs-lookup"><span data-stu-id="28ee2-123">**Note:** You can filter on any of the fields of the [teamsApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="28ee2-124">Вы можете использовать любую из следующих операций фильтрации: EQUAL, Not Equals, and, OR и not.</span><span class="sxs-lookup"><span data-stu-id="28ee2-124">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28ee2-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28ee2-125">Request headers</span></span>

| <span data-ttu-id="28ee2-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="28ee2-126">Header</span></span>        | <span data-ttu-id="28ee2-127">Значение</span><span class="sxs-lookup"><span data-stu-id="28ee2-127">Value</span></span>                     |
|:--------------|:--------------------------|
| <span data-ttu-id="28ee2-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28ee2-128">Authorization</span></span> | <span data-ttu-id="28ee2-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28ee2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28ee2-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28ee2-131">Request body</span></span>

<span data-ttu-id="28ee2-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="28ee2-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28ee2-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="28ee2-133">Response</span></span>

<span data-ttu-id="28ee2-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список объектов [teamsApp](../resources/teamsapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="28ee2-134">If successful, this method returns a `200 OK` response code and a list of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="28ee2-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="28ee2-135">Examples</span></span>

### <a name="example-1-list-all-applications-in-your-tenant"></a><span data-ttu-id="28ee2-136">Пример 1: список всех приложений в клиенте</span><span class="sxs-lookup"><span data-stu-id="28ee2-136">Example 1: List all applications in your tenant</span></span>

<span data-ttu-id="28ee2-137">В следующем примере перечисляются все приложения, характерные для вашего клиента.</span><span class="sxs-lookup"><span data-stu-id="28ee2-137">The following example lists all apps that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="28ee2-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="28ee2-138">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```http
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApp?$filter=distributionMethod eq 'organization'
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="28ee2-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="28ee2-139">Response</span></span>

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

### <a name="example-2-list-applications-with-a-given-id"></a><span data-ttu-id="28ee2-140">Пример 2: список приложений с заданным ИДЕНТИФИКАТОРом</span><span class="sxs-lookup"><span data-stu-id="28ee2-140">Example 2: List applications with a given ID</span></span>

<span data-ttu-id="28ee2-141">В следующем примере перечисляются приложения с указанным ИДЕНТИФИКАТОРом.</span><span class="sxs-lookup"><span data-stu-id="28ee2-141">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="28ee2-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="28ee2-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```http
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="28ee2-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="28ee2-143">Response</span></span>

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
