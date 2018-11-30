---
title: Список вкладок в канале
description: 'Получить список вкладок в указанный канал в группе. '
ms.openlocfilehash: 6c72bae20542911c7ab1563e994ca9ebdb79b37a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081689"
---
# <a name="list-tabs-in-channel"></a><span data-ttu-id="51bdb-103">Список вкладок в канале</span><span class="sxs-lookup"><span data-stu-id="51bdb-103">List tabs in channel</span></span>

> <span data-ttu-id="51bdb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="51bdb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51bdb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51bdb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="51bdb-106">Получить список [вкладок](../resources/teamstab.md) в указанный [канала](../resources/channel.md) в пределах [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="51bdb-106">Retrieve the list of [tabs](../resources/teamstab.md) in the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="51bdb-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51bdb-107">Permissions</span></span>
<span data-ttu-id="51bdb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51bdb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51bdb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51bdb-110">Permission type</span></span>      | <span data-ttu-id="51bdb-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51bdb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51bdb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51bdb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="51bdb-113">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="51bdb-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="51bdb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51bdb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51bdb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51bdb-115">Not supported.</span></span>    |
| <span data-ttu-id="51bdb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51bdb-116">Application</span></span>                            | <span data-ttu-id="51bdb-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51bdb-117">Group.Read.All, Group.ReadWrite.All</span></span>         |

## <a name="http-request"></a><span data-ttu-id="51bdb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51bdb-118">HTTP request</span></span>

```http
GET /teams/{id}/channels/{id}/tabs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51bdb-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="51bdb-119">Optional query parameters</span></span>

<span data-ttu-id="51bdb-120">Этот метод поддерживает $filter $select, и $разверните [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="51bdb-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="51bdb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51bdb-121">Request headers</span></span>
| <span data-ttu-id="51bdb-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51bdb-122">Header</span></span>       | <span data-ttu-id="51bdb-123">Значение</span><span class="sxs-lookup"><span data-stu-id="51bdb-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="51bdb-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51bdb-124">Authorization</span></span>  | <span data-ttu-id="51bdb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51bdb-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="51bdb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51bdb-127">Request body</span></span>
<span data-ttu-id="51bdb-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51bdb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51bdb-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="51bdb-129">Response</span></span>
<span data-ttu-id="51bdb-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [вкладок](../resources/teamstab.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="51bdb-130">If successful, this method returns a `200 OK` response code and collection of [tabs](../resources/teamstab.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51bdb-131">Пример</span><span class="sxs-lookup"><span data-stu-id="51bdb-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="51bdb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="51bdb-132">Request</span></span>
<span data-ttu-id="51bdb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51bdb-133">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs
```

#### <a name="response"></a><span data-ttu-id="51bdb-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="51bdb-134">Response</span></span>
<span data-ttu-id="51bdb-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="51bdb-135">The following is an example of the response.</span></span>
><span data-ttu-id="51bdb-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51bdb-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
