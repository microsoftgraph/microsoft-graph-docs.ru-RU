---
title: Список опубликованных приложений из каталога приложений группами Майкрософт
description: 'Список приложений из каталога приложений группами Майкрософт. '
ms.openlocfilehash: 84b5576ed2a7d38783e45b1384c79f05c9ea418b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082709"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a><span data-ttu-id="74bb6-103">Список опубликованных приложений из каталога приложений группами Майкрософт</span><span class="sxs-lookup"><span data-stu-id="74bb6-103">List the published apps from the Microsoft Teams app catalog</span></span>

> <span data-ttu-id="74bb6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="74bb6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74bb6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74bb6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="74bb6-106">Список [приложений](../resources/teamsapp.md) из каталога приложений группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="74bb6-106">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span> <span data-ttu-id="74bb6-107">Этот компонент включает приложений из магазина группами Майкрософт, а также приложений из каталога приложений организации (каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="74bb6-107">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="74bb6-108">Приобретать приложения в вашей организации только каталог приложений, укажите `Organization` как **distributionMethod** в [teamsCatalogApp](../resources/teamsapp.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="74bb6-108">To get apps from your organization's app catalog only, specify `Organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="74bb6-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74bb6-109">Permissions</span></span>

<span data-ttu-id="74bb6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="74bb6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="74bb6-112">**Примечание:** Только глобальный администратор может вызывать этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="74bb6-112">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="74bb6-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74bb6-113">Permission Type</span></span>                        | <span data-ttu-id="74bb6-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74bb6-114">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="74bb6-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74bb6-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="74bb6-116">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74bb6-116">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="74bb6-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74bb6-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74bb6-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="74bb6-118">Not supported</span></span>|
| <span data-ttu-id="74bb6-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74bb6-119">Application</span></span>                            | <span data-ttu-id="74bb6-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="74bb6-120">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="74bb6-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74bb6-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="74bb6-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="74bb6-122">Optional query parameters</span></span>
<span data-ttu-id="74bb6-123">Этот метод поддерживает $filter $select, и $разверните [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="74bb6-123">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="74bb6-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74bb6-124">Request headers</span></span>

| <span data-ttu-id="74bb6-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="74bb6-125">Header</span></span>        | <span data-ttu-id="74bb6-126">Значение</span><span class="sxs-lookup"><span data-stu-id="74bb6-126">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="74bb6-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="74bb6-127">Authorization</span></span> | <span data-ttu-id="74bb6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74bb6-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="74bb6-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="74bb6-130">Request body</span></span>
<span data-ttu-id="74bb6-131">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="74bb6-131">None.</span></span>

><span data-ttu-id="74bb6-132">**Примечание:** Можно отфильтровать поля объекта [teamsCatalogApp](../resources/teamsapp.md) для сокращения списка результатов.</span><span class="sxs-lookup"><span data-stu-id="74bb6-132">**Note:** You can filter on any of the fields of the [teamsCatalogApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="74bb6-133">Можно использовать любой из следующих операций фильтра: равно, не равно и, или, а не.</span><span class="sxs-lookup"><span data-stu-id="74bb6-133">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="response"></a><span data-ttu-id="74bb6-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="74bb6-134">Response</span></span>
<span data-ttu-id="74bb6-135">Успешно завершена, этот метод возвращает `200 OK` код ответа и список объектов [teamsCatalogApp](../resources/teamsapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="74bb6-135">If successful, this method returns a `200 OK` response code and a list of [teamsCatalogApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="74bb6-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="74bb6-136">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="74bb6-137">Пример 1</span><span class="sxs-lookup"><span data-stu-id="74bb6-137">Example 1</span></span>
<span data-ttu-id="74bb6-138">В следующем примере перечисляются все приложения, которые специфичны для вашего клиента.</span><span class="sxs-lookup"><span data-stu-id="74bb6-138">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="74bb6-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="74bb6-139">Request</span></span>
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

#### <a name="response"></a><span data-ttu-id="74bb6-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="74bb6-140">Response</span></span>
```
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod":"Organization"
    }
  ]
}
```

### <a name="example-2"></a><span data-ttu-id="74bb6-141">Пример 2</span><span class="sxs-lookup"><span data-stu-id="74bb6-141">Example 2</span></span>

<span data-ttu-id="74bb6-142">В следующем примере перечисляются приложений с указанным идентификатором.</span><span class="sxs-lookup"><span data-stu-id="74bb6-142">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="74bb6-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="74bb6-143">Request</span></span>
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="74bb6-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="74bb6-144">Response</span></span>
```
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod":"Organization"
    }
  ]
}
```

