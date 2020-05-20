---
title: Список опубликованных приложений из каталога приложений Microsoft Teams
description: 'Перечисление приложений из каталога приложений Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d2dbbc77cdd6ca5fad9afcf975388a678ac1c7a1
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290323"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a><span data-ttu-id="7aae4-103">Список опубликованных приложений из каталога приложений Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="7aae4-103">List the published apps from the Microsoft Teams app catalog</span></span>

<span data-ttu-id="7aae4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7aae4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7aae4-105">Перечисление [приложений](../resources/teamsapp.md) из каталога приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="7aae4-105">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="7aae4-106">Сюда входят приложения из магазина Microsoft Teams, а также приложения из каталога приложений организации (Каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="7aae4-106">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="7aae4-107">Чтобы получить доступ к приложениям только из каталога приложений вашей организации, укажите в `Organization` качестве **distributionMethod** в ресурсе [теамскаталогапп](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="7aae4-107">To get apps from your organization's app catalog only, specify `Organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="7aae4-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7aae4-108">Permissions</span></span>

<span data-ttu-id="7aae4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="7aae4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

> <span data-ttu-id="7aae4-111">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="7aae4-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="7aae4-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7aae4-112">Permission Type</span></span>                        | <span data-ttu-id="7aae4-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7aae4-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="7aae4-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7aae4-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="7aae4-115">CamlQuery. Read. ALL, CamlQuery. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7aae4-115">AppCatalog.Read.All, AppCatalog.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="7aae4-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7aae4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7aae4-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7aae4-117">Not supported</span></span>                       |
| <span data-ttu-id="7aae4-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7aae4-118">Application</span></span>                            | <span data-ttu-id="7aae4-119">CamlQuery. Read. ALL, CamlQuery. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7aae4-119">AppCatalog.Read.All, AppCatalog.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7aae4-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7aae4-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7aae4-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7aae4-121">Optional query parameters</span></span>

<span data-ttu-id="7aae4-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $filter, $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="7aae4-122">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7aae4-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7aae4-123">Request headers</span></span>

| <span data-ttu-id="7aae4-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7aae4-124">Header</span></span>        | <span data-ttu-id="7aae4-125">Значение</span><span class="sxs-lookup"><span data-stu-id="7aae4-125">Value</span></span>                     |
|:--------------|:--------------------------|
| <span data-ttu-id="7aae4-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7aae4-126">Authorization</span></span> | <span data-ttu-id="7aae4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7aae4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7aae4-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7aae4-129">Request body</span></span>

<span data-ttu-id="7aae4-130">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7aae4-130">None.</span></span>

> <span data-ttu-id="7aae4-131">**Примечание:** Можно выполнить фильтрацию по любому полю объекта [теамскаталогапп](../resources/teamsapp.md) для сокращения списка результатов.</span><span class="sxs-lookup"><span data-stu-id="7aae4-131">**Note:** You can filter on any of the fields of the [teamsCatalogApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="7aae4-132">Вы можете использовать любую из следующих операций фильтрации: EQUAL, Not Equals, and, OR и not.</span><span class="sxs-lookup"><span data-stu-id="7aae4-132">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="response"></a><span data-ttu-id="7aae4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="7aae4-133">Response</span></span>

<span data-ttu-id="7aae4-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список объектов [теамскаталогапп](../resources/teamsapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7aae4-134">If successful, this method returns a `200 OK` response code and a list of [teamsCatalogApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7aae4-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="7aae4-135">Examples</span></span>

### <a name="example-1-list-all-applications"></a><span data-ttu-id="7aae4-136">Пример 1: List All Applications</span><span class="sxs-lookup"><span data-stu-id="7aae4-136">Example 1: List all applications</span></span>

<span data-ttu-id="7aae4-137">В приведенном ниже примере выводится список всех приложений, относящихся к вашему клиенту.</span><span class="sxs-lookup"><span data-stu-id="7aae4-137">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="7aae4-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="7aae4-138">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="7aae4-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="7aae4-139">Response</span></span>

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

### <a name="example-2-list-applications-with-a-given-id"></a><span data-ttu-id="7aae4-140">Пример 2: список приложений с заданным ИДЕНТИФИКАТОРом</span><span class="sxs-lookup"><span data-stu-id="7aae4-140">Example 2: List applications with a given ID</span></span>

<span data-ttu-id="7aae4-141">В следующем примере перечисляются приложения с указанным ИДЕНТИФИКАТОРом.</span><span class="sxs-lookup"><span data-stu-id="7aae4-141">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="7aae4-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="7aae4-142">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="7aae4-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="7aae4-143">Response</span></span>

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
