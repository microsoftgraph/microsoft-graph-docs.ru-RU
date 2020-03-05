---
title: Список опубликованных приложений из каталога приложений Microsoft Teams
description: 'Перечисление приложений из каталога приложений Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a76edf899f6a2bc3482b79776a52bf4080c8441a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452516"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a><span data-ttu-id="8b9ec-103">Список опубликованных приложений из каталога приложений Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="8b9ec-103">List the published apps from the Microsoft Teams app catalog</span></span>

<span data-ttu-id="8b9ec-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8b9ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b9ec-105">Перечисление [приложений](../resources/teamsapp.md) из каталога приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="8b9ec-105">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="8b9ec-106">Сюда входят приложения из магазина Microsoft Teams, а также приложения из каталога приложений организации (Каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="8b9ec-106">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="8b9ec-107">Чтобы получить доступ к приложениям только из каталога приложений вашей организации, `Organization` укажите в качестве **distributionMethod** в ресурсе [теамскаталогапп](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="8b9ec-107">To get apps from your organization's app catalog only, specify `Organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b9ec-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b9ec-108">Permissions</span></span>

<span data-ttu-id="8b9ec-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="8b9ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

| <span data-ttu-id="8b9ec-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b9ec-111">Permission Type</span></span>                        | <span data-ttu-id="8b9ec-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b9ec-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="8b9ec-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b9ec-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b9ec-114">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b9ec-114">AppCatalog.ReadWrite.All</span></span>            |
| <span data-ttu-id="8b9ec-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b9ec-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b9ec-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8b9ec-116">Not supported</span></span>                       |
| <span data-ttu-id="8b9ec-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b9ec-117">Application</span></span>                            | <span data-ttu-id="8b9ec-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8b9ec-118">Not supported</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="8b9ec-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b9ec-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8b9ec-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8b9ec-120">Optional query parameters</span></span>

<span data-ttu-id="8b9ec-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $filter, $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8b9ec-121">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b9ec-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b9ec-122">Request headers</span></span>

| <span data-ttu-id="8b9ec-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b9ec-123">Header</span></span>        | <span data-ttu-id="8b9ec-124">Значение</span><span class="sxs-lookup"><span data-stu-id="8b9ec-124">Value</span></span>                     |
|:--------------|:--------------------------|
| <span data-ttu-id="8b9ec-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b9ec-125">Authorization</span></span> | <span data-ttu-id="8b9ec-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b9ec-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b9ec-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b9ec-128">Request body</span></span>

<span data-ttu-id="8b9ec-129">Нет.</span><span class="sxs-lookup"><span data-stu-id="8b9ec-129">None.</span></span>

> <span data-ttu-id="8b9ec-130">**Примечание:** Можно выполнить фильтрацию по любому полю объекта [теамскаталогапп](../resources/teamsapp.md) для сокращения списка результатов.</span><span class="sxs-lookup"><span data-stu-id="8b9ec-130">**Note:** You can filter on any of the fields of the [teamsCatalogApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="8b9ec-131">Вы можете использовать любую из следующих операций фильтрации: EQUAL, Not Equals, and, OR и not.</span><span class="sxs-lookup"><span data-stu-id="8b9ec-131">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="response"></a><span data-ttu-id="8b9ec-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b9ec-132">Response</span></span>

<span data-ttu-id="8b9ec-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список объектов [теамскаталогапп](../resources/teamsapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8b9ec-133">If successful, this method returns a `200 OK` response code and a list of [teamsCatalogApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8b9ec-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="8b9ec-134">Examples</span></span>

### <a name="example-1-list-all-applications"></a><span data-ttu-id="8b9ec-135">Пример 1: List All Applications</span><span class="sxs-lookup"><span data-stu-id="8b9ec-135">Example 1: List all applications</span></span>

<span data-ttu-id="8b9ec-136">В приведенном ниже примере выводится список всех приложений, относящихся к вашему клиенту.</span><span class="sxs-lookup"><span data-stu-id="8b9ec-136">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="8b9ec-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b9ec-137">Request</span></span>

```http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="8b9ec-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b9ec-138">Response</span></span>

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

### <a name="example-2-list-applications-with-a-given-id"></a><span data-ttu-id="8b9ec-139">Пример 2: список приложений с заданным ИДЕНТИФИКАТОРом</span><span class="sxs-lookup"><span data-stu-id="8b9ec-139">Example 2: List applications with a given ID</span></span>

<span data-ttu-id="8b9ec-140">В следующем примере перечисляются приложения с указанным ИДЕНТИФИКАТОРом.</span><span class="sxs-lookup"><span data-stu-id="8b9ec-140">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="8b9ec-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b9ec-141">Request</span></span>

```http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="8b9ec-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b9ec-142">Response</span></span>

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

