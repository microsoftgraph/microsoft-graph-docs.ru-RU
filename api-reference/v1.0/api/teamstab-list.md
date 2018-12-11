---
title: Список вкладок в канале
description: 'Получить список вкладок в указанный канал в группе. '
ms.openlocfilehash: 4efbe8508fc125d87268adfb05c23b99ab2c3d4b
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222375"
---
# <a name="list-tabs-in-channel"></a><span data-ttu-id="ecb58-103">Список вкладок в канале</span><span class="sxs-lookup"><span data-stu-id="ecb58-103">List tabs in channel</span></span>



<span data-ttu-id="ecb58-104">Получить список [вкладок](../resources/teamstab.md) в указанный [канала](../resources/channel.md) в пределах [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="ecb58-104">Retrieve the list of [tabs](../resources/teamstab.md) in the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="ecb58-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ecb58-105">Permissions</span></span>
<span data-ttu-id="ecb58-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecb58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecb58-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ecb58-108">Permission type</span></span>      | <span data-ttu-id="ecb58-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ecb58-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ecb58-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ecb58-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ecb58-111">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ecb58-111">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="ecb58-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ecb58-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ecb58-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecb58-113">Not supported.</span></span>    |
| <span data-ttu-id="ecb58-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ecb58-114">Application</span></span>                            | <span data-ttu-id="ecb58-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecb58-115">Group.Read.All, Group.ReadWrite.All</span></span>         |

> <span data-ttu-id="ecb58-116">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="ecb58-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ecb58-117">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="ecb58-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ecb58-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ecb58-118">HTTP request</span></span>

```http
GET /teams/{id}/channels/{id}/tabs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ecb58-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ecb58-119">Optional query parameters</span></span>

<span data-ttu-id="ecb58-120">Этот метод поддерживает $filter $select, и $разверните [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ecb58-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ecb58-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ecb58-121">Request headers</span></span>
| <span data-ttu-id="ecb58-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ecb58-122">Header</span></span>       | <span data-ttu-id="ecb58-123">Значение</span><span class="sxs-lookup"><span data-stu-id="ecb58-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ecb58-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ecb58-124">Authorization</span></span>  | <span data-ttu-id="ecb58-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ecb58-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ecb58-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ecb58-127">Request body</span></span>
<span data-ttu-id="ecb58-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ecb58-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecb58-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecb58-129">Response</span></span>
<span data-ttu-id="ecb58-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [вкладок](../resources/teamstab.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ecb58-130">If successful, this method returns a `200 OK` response code and collection of [tabs](../resources/teamstab.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecb58-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ecb58-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ecb58-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ecb58-132">Request</span></span>
<span data-ttu-id="ecb58-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ecb58-133">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs
```

#### <a name="response"></a><span data-ttu-id="ecb58-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecb58-134">Response</span></span>
<span data-ttu-id="ecb58-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ecb58-135">The following is an example of the response.</span></span>
><span data-ttu-id="ecb58-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ecb58-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "value": [
    {
      "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
      "name": "My Contoso Tab - updated",
      "teamsAppId": "06805b9e-77e3-4b93-ac81-525eb87513b8",
      "configuration": {
        "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
        "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
        "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
        "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
      },
      "sortOrderIndex": 20,
      "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
    },
    {
      "id": "b5d5f001-0471-49a5-aac4-04ef96683be0",
      "name": "My Trello Tab",
      "teamsAppId": "23134c6b-5e4b-439c-8f70-3ded1df20805",
      "configuration": null,
      "sortOrderIndex": 21,
      "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3a3709b35c-a0ba-467c-8001-0f66895fb9d3?label=My%20Trello%Tab"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List all tabs in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
