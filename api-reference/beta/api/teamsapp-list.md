---
title: Список опубликованных приложений из каталога приложений Microsoft Teams
description: 'Перечисление приложений из каталога приложений Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4a27a7b63248ddb94e4ea819300f325e04a02c9f
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636520"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a><span data-ttu-id="f7e12-103">Список опубликованных приложений из каталога приложений Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="f7e12-103">List the published apps from the Microsoft Teams app catalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7e12-104">Перечисление [приложений](../resources/teamsapp.md) из каталога приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f7e12-104">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="f7e12-105">Сюда входят приложения из магазина Microsoft Teams, а также приложения из каталога приложений организации (Каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="f7e12-105">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="f7e12-106">Чтобы получить доступ к приложениям только из каталога приложений вашей организации, `Organization` укажите в качестве **distributionMethod** в ресурсе [теамскаталогапп](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="f7e12-106">To get apps from your organization's app catalog only, specify `Organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7e12-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7e12-107">Permissions</span></span>

<span data-ttu-id="f7e12-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="f7e12-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

| <span data-ttu-id="f7e12-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7e12-110">Permission Type</span></span>                        | <span data-ttu-id="f7e12-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7e12-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="f7e12-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7e12-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f7e12-113">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7e12-113">AppCatalog.ReadWrite.All</span></span>            |
| <span data-ttu-id="f7e12-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7e12-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7e12-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f7e12-115">Not supported</span></span>                       |
| <span data-ttu-id="f7e12-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7e12-116">Application</span></span>                            | <span data-ttu-id="f7e12-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f7e12-117">Not supported</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="f7e12-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7e12-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f7e12-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f7e12-119">Optional query parameters</span></span>

<span data-ttu-id="f7e12-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $filter, $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f7e12-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7e12-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7e12-121">Request headers</span></span>

| <span data-ttu-id="f7e12-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7e12-122">Header</span></span>        | <span data-ttu-id="f7e12-123">Значение</span><span class="sxs-lookup"><span data-stu-id="f7e12-123">Value</span></span>                     |
|:--------------|:--------------------------|
| <span data-ttu-id="f7e12-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7e12-124">Authorization</span></span> | <span data-ttu-id="f7e12-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7e12-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7e12-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7e12-127">Request body</span></span>

<span data-ttu-id="f7e12-128">Нет.</span><span class="sxs-lookup"><span data-stu-id="f7e12-128">None.</span></span>

> <span data-ttu-id="f7e12-129">**Примечание:** Можно выполнить фильтрацию по любому полю объекта [теамскаталогапп](../resources/teamsapp.md) для сокращения списка результатов.</span><span class="sxs-lookup"><span data-stu-id="f7e12-129">**Note:** You can filter on any of the fields of the [teamsCatalogApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="f7e12-130">Вы можете использовать любую из следующих операций фильтрации: EQUAL, Not Equals, and, OR и not.</span><span class="sxs-lookup"><span data-stu-id="f7e12-130">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="response"></a><span data-ttu-id="f7e12-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7e12-131">Response</span></span>

<span data-ttu-id="f7e12-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список объектов [теамскаталогапп](../resources/teamsapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f7e12-132">If successful, this method returns a `200 OK` response code and a list of [teamsCatalogApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f7e12-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="f7e12-133">Examples</span></span>

### <a name="example-1-list-all-applications"></a><span data-ttu-id="f7e12-134">Пример 1: List All Applications</span><span class="sxs-lookup"><span data-stu-id="f7e12-134">Example 1: List all applications</span></span>

<span data-ttu-id="f7e12-135">В приведенном ниже примере выводится список всех приложений, относящихся к вашему клиенту.</span><span class="sxs-lookup"><span data-stu-id="f7e12-135">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="f7e12-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7e12-136">Request</span></span>

```http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="f7e12-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7e12-137">Response</span></span>

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

### <a name="example-2-list-applications-with-a-given-id"></a><span data-ttu-id="f7e12-138">Пример 2: список приложений с заданным ИДЕНТИФИКАТОРом</span><span class="sxs-lookup"><span data-stu-id="f7e12-138">Example 2: List applications with a given ID</span></span>

<span data-ttu-id="f7e12-139">В следующем примере перечисляются приложения с указанным ИДЕНТИФИКАТОРом.</span><span class="sxs-lookup"><span data-stu-id="f7e12-139">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="f7e12-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7e12-140">Request</span></span>

```http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="f7e12-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7e12-141">Response</span></span>

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

