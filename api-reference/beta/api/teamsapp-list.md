---
title: Список опубликованных приложений из каталога приложений группами Майкрософт
description: 'Список приложений из каталога приложений группами Майкрософт. '
author: nkramer
ms.openlocfilehash: 77867d5b75721fcb169da6ad6a8ff39c46de196e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326469"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a><span data-ttu-id="cc387-103">Список опубликованных приложений из каталога приложений группами Майкрософт</span><span class="sxs-lookup"><span data-stu-id="cc387-103">List the published apps from the Microsoft Teams app catalog</span></span>

> <span data-ttu-id="cc387-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cc387-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc387-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc387-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cc387-106">Список [приложений](../resources/teamsapp.md) из каталога приложений группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="cc387-106">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span> <span data-ttu-id="cc387-107">Этот компонент включает приложений из магазина группами Майкрософт, а также приложений из каталога приложений организации (каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="cc387-107">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="cc387-108">Приобретать приложения в вашей организации только каталог приложений, укажите `Organization` как **distributionMethod** в [teamsCatalogApp](../resources/teamsapp.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="cc387-108">To get apps from your organization's app catalog only, specify `Organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc387-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cc387-109">Permissions</span></span>

<span data-ttu-id="cc387-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="cc387-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="cc387-112">**Примечание:** Только глобальный администратор может вызывать этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="cc387-112">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="cc387-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc387-113">Permission Type</span></span>                        | <span data-ttu-id="cc387-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc387-114">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="cc387-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc387-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="cc387-116">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc387-116">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="cc387-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc387-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc387-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cc387-118">Not supported</span></span>|
| <span data-ttu-id="cc387-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cc387-119">Application</span></span>                            | <span data-ttu-id="cc387-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cc387-120">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc387-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc387-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cc387-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cc387-122">Optional query parameters</span></span>
<span data-ttu-id="cc387-123">Этот метод поддерживает $filter $select, и $разверните [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cc387-123">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc387-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc387-124">Request headers</span></span>

| <span data-ttu-id="cc387-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cc387-125">Header</span></span>        | <span data-ttu-id="cc387-126">Значение</span><span class="sxs-lookup"><span data-stu-id="cc387-126">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="cc387-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cc387-127">Authorization</span></span> | <span data-ttu-id="cc387-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc387-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cc387-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc387-130">Request body</span></span>
<span data-ttu-id="cc387-131">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cc387-131">None.</span></span>

><span data-ttu-id="cc387-132">**Примечание:** Можно отфильтровать поля объекта [teamsCatalogApp](../resources/teamsapp.md) для сокращения списка результатов.</span><span class="sxs-lookup"><span data-stu-id="cc387-132">**Note:** You can filter on any of the fields of the [teamsCatalogApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="cc387-133">Можно использовать любой из следующих операций фильтра: равно, не равно и, или, а не.</span><span class="sxs-lookup"><span data-stu-id="cc387-133">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="response"></a><span data-ttu-id="cc387-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="cc387-134">Response</span></span>
<span data-ttu-id="cc387-135">Успешно завершена, этот метод возвращает `200 OK` код ответа и список объектов [teamsCatalogApp](../resources/teamsapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cc387-135">If successful, this method returns a `200 OK` response code and a list of [teamsCatalogApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cc387-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="cc387-136">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="cc387-137">Пример 1</span><span class="sxs-lookup"><span data-stu-id="cc387-137">Example 1</span></span>
<span data-ttu-id="cc387-138">В следующем примере перечисляются все приложения, которые специфичны для вашего клиента.</span><span class="sxs-lookup"><span data-stu-id="cc387-138">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="cc387-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc387-139">Request</span></span>
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

#### <a name="response"></a><span data-ttu-id="cc387-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="cc387-140">Response</span></span>
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

### <a name="example-2"></a><span data-ttu-id="cc387-141">Пример 2</span><span class="sxs-lookup"><span data-stu-id="cc387-141">Example 2</span></span>

<span data-ttu-id="cc387-142">В следующем примере перечисляются приложений с указанным идентификатором.</span><span class="sxs-lookup"><span data-stu-id="cc387-142">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="cc387-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc387-143">Request</span></span>
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="cc387-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="cc387-144">Response</span></span>
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

