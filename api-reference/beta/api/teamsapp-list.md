---
title: Список опубликованных приложений из каталога приложений группами Майкрософт
description: 'Список приложений из каталога приложений группами Майкрософт. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1e4d9348cbb28ed0daf1ec48459378935d78e0a2
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967258"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a><span data-ttu-id="0543c-103">Список опубликованных приложений из каталога приложений группами Майкрософт</span><span class="sxs-lookup"><span data-stu-id="0543c-103">List the published apps from the Microsoft Teams app catalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0543c-104">Список [приложений](../resources/teamsapp.md) из каталога приложений группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="0543c-104">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="0543c-105">Этот компонент включает приложений из магазина группами Майкрософт, а также приложений из каталога приложений организации (каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="0543c-105">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="0543c-106">Приобретать приложения в вашей организации только каталог приложений, укажите `Organization` как **distributionMethod** в [teamsCatalogApp](../resources/teamsapp.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="0543c-106">To get apps from your organization's app catalog only, specify `Organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="0543c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0543c-107">Permissions</span></span>

<span data-ttu-id="0543c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="0543c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

> <span data-ttu-id="0543c-110">**Примечание:** Только глобальный администратор может вызывать этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="0543c-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="0543c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0543c-111">Permission Type</span></span>                        | <span data-ttu-id="0543c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0543c-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="0543c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0543c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="0543c-114">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0543c-114">AppCatalog.ReadWrite.All</span></span>            |
| <span data-ttu-id="0543c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0543c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0543c-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0543c-116">Not supported</span></span>                       |
| <span data-ttu-id="0543c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0543c-117">Application</span></span>                            | <span data-ttu-id="0543c-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0543c-118">Not supported</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="0543c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0543c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0543c-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0543c-120">Optional query parameters</span></span>

<span data-ttu-id="0543c-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $filter, $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0543c-121">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0543c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0543c-122">Request headers</span></span>

| <span data-ttu-id="0543c-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0543c-123">Header</span></span>        | <span data-ttu-id="0543c-124">Значение</span><span class="sxs-lookup"><span data-stu-id="0543c-124">Value</span></span>                     |
|:--------------|:--------------------------|
| <span data-ttu-id="0543c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0543c-125">Authorization</span></span> | <span data-ttu-id="0543c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0543c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0543c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0543c-128">Request body</span></span>

<span data-ttu-id="0543c-129">Нет.</span><span class="sxs-lookup"><span data-stu-id="0543c-129">None.</span></span>

> <span data-ttu-id="0543c-130">**Примечание:** Можно отфильтровать поля объекта [teamsCatalogApp](../resources/teamsapp.md) для сокращения списка результатов.</span><span class="sxs-lookup"><span data-stu-id="0543c-130">**Note:** You can filter on any of the fields of the [teamsCatalogApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="0543c-131">Можно использовать любой из следующих операций фильтра: равно, не равно и, или, а не.</span><span class="sxs-lookup"><span data-stu-id="0543c-131">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="response"></a><span data-ttu-id="0543c-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="0543c-132">Response</span></span>

<span data-ttu-id="0543c-133">Успешно завершена, этот метод возвращает `200 OK` код ответа и список объектов [teamsCatalogApp](../resources/teamsapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0543c-133">If successful, this method returns a `200 OK` response code and a list of [teamsCatalogApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0543c-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="0543c-134">Examples</span></span>

### <a name="example-1-list-all-applications"></a><span data-ttu-id="0543c-135">В примере 1: Список всех приложений</span><span class="sxs-lookup"><span data-stu-id="0543c-135">Example 1: List all applications</span></span>

<span data-ttu-id="0543c-136">В следующем примере перечисляются все приложения, которые специфичны для вашего клиента.</span><span class="sxs-lookup"><span data-stu-id="0543c-136">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="0543c-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="0543c-137">Request</span></span>

```http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="0543c-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="0543c-138">Response</span></span>

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

### <a name="example-2-list-applications-with-a-given-id"></a><span data-ttu-id="0543c-139">Пример 2: Список приложений с заданным Идентификатором</span><span class="sxs-lookup"><span data-stu-id="0543c-139">Example 2: List applications with a given ID</span></span>

<span data-ttu-id="0543c-140">В следующем примере перечисляются приложений с указанным идентификатором.</span><span class="sxs-lookup"><span data-stu-id="0543c-140">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="0543c-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="0543c-141">Request</span></span>

```http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="0543c-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="0543c-142">Response</span></span>

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

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/teamsapp-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
