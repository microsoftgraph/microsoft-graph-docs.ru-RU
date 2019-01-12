---
title: Список опубликованных приложений из каталога приложений группами Майкрософт
description: 'Список приложений из каталога приложений группами Майкрософт. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fc8648ac99a3b502956ce07d5c5b53bab930095e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945589"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a><span data-ttu-id="d92ff-103">Список опубликованных приложений из каталога приложений группами Майкрософт</span><span class="sxs-lookup"><span data-stu-id="d92ff-103">List the published apps from the Microsoft Teams app catalog</span></span>



<span data-ttu-id="d92ff-104">Список [приложений](../resources/teamsapp.md) из каталога приложений группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="d92ff-104">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span> <span data-ttu-id="d92ff-105">Этот компонент включает приложений из магазина группами Майкрософт, а также приложений из каталога приложений организации (каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="d92ff-105">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="d92ff-106">Приобретать приложения в вашей организации только каталог приложений, укажите `Organization` как **distributionMethod** в [teamsCatalogApp](../resources/teamsapp.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="d92ff-106">To get apps from your organization's app catalog only, specify `Organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="d92ff-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d92ff-107">Permissions</span></span>

<span data-ttu-id="d92ff-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="d92ff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="d92ff-110">**Примечание:** Только глобальный администратор может вызывать этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="d92ff-110">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="d92ff-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d92ff-111">Permission Type</span></span>                        | <span data-ttu-id="d92ff-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d92ff-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="d92ff-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d92ff-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d92ff-114">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d92ff-114">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="d92ff-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d92ff-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d92ff-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d92ff-116">Not supported</span></span>|
| <span data-ttu-id="d92ff-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d92ff-117">Application</span></span>                            | <span data-ttu-id="d92ff-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d92ff-118">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="d92ff-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d92ff-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d92ff-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d92ff-120">Optional query parameters</span></span>
<span data-ttu-id="d92ff-121">Этот метод поддерживает $filter $select, и $разверните [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d92ff-121">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d92ff-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d92ff-122">Request headers</span></span>

| <span data-ttu-id="d92ff-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d92ff-123">Header</span></span>        | <span data-ttu-id="d92ff-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d92ff-124">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="d92ff-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d92ff-125">Authorization</span></span> | <span data-ttu-id="d92ff-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d92ff-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d92ff-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d92ff-128">Request body</span></span>
<span data-ttu-id="d92ff-129">Нет.</span><span class="sxs-lookup"><span data-stu-id="d92ff-129">None.</span></span>

><span data-ttu-id="d92ff-130">**Примечание:** Можно отфильтровать поля объекта [teamsCatalogApp](../resources/teamsapp.md) для сокращения списка результатов.</span><span class="sxs-lookup"><span data-stu-id="d92ff-130">**Note:** You can filter on any of the fields of the [teamsCatalogApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="d92ff-131">Можно использовать любой из следующих операций фильтра: равно, не равно и, или, а не.</span><span class="sxs-lookup"><span data-stu-id="d92ff-131">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="response"></a><span data-ttu-id="d92ff-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d92ff-132">Response</span></span>
<span data-ttu-id="d92ff-133">Успешно завершена, этот метод возвращает `200 OK` код ответа и список объектов [teamsCatalogApp](../resources/teamsapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d92ff-133">If successful, this method returns a `200 OK` response code and a list of [teamsCatalogApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d92ff-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="d92ff-134">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="d92ff-135">Пример 1</span><span class="sxs-lookup"><span data-stu-id="d92ff-135">Example 1</span></span>
<span data-ttu-id="d92ff-136">В следующем примере перечисляются все приложения, которые специфичны для вашего клиента.</span><span class="sxs-lookup"><span data-stu-id="d92ff-136">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="d92ff-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="d92ff-137">Request</span></span>
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

#### <a name="response"></a><span data-ttu-id="d92ff-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d92ff-138">Response</span></span>
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

### <a name="example-2"></a><span data-ttu-id="d92ff-139">Пример 2</span><span class="sxs-lookup"><span data-stu-id="d92ff-139">Example 2</span></span>

<span data-ttu-id="d92ff-140">В следующем примере перечисляются приложений с указанным идентификатором.</span><span class="sxs-lookup"><span data-stu-id="d92ff-140">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="d92ff-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="d92ff-141">Request</span></span>
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="d92ff-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d92ff-142">Response</span></span>
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

