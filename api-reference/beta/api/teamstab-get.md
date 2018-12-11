---
title: Получить вкладки
description: 'Извлечение свойств и отношения между заданной вкладки. '
ms.openlocfilehash: 7bef495fbb37a878a291f2aac6004d386e932cbd
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222410"
---
# <a name="get-tab"></a><span data-ttu-id="2de1f-103">Получить вкладки</span><span class="sxs-lookup"><span data-stu-id="2de1f-103">Get tab</span></span>

> <span data-ttu-id="2de1f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2de1f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2de1f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2de1f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2de1f-106">Извлечение свойств и связи указанного [вкладки](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="2de1f-106">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="2de1f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2de1f-107">Permissions</span></span>
<span data-ttu-id="2de1f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2de1f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2de1f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2de1f-110">Permission type</span></span>      | <span data-ttu-id="2de1f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2de1f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2de1f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2de1f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2de1f-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2de1f-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2de1f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2de1f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2de1f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2de1f-115">Not supported.</span></span>    |
|<span data-ttu-id="2de1f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2de1f-116">Application</span></span> | <span data-ttu-id="2de1f-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2de1f-117">Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="2de1f-118">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="2de1f-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="2de1f-119">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="2de1f-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="2de1f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2de1f-120">HTTP request</span></span>
```http
GET /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2de1f-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2de1f-121">Optional query parameters</span></span>

<span data-ttu-id="2de1f-122">Этот метод поддерживает $select и $разверните [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2de1f-122">This method supports the $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2de1f-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2de1f-123">Request headers</span></span>
| <span data-ttu-id="2de1f-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2de1f-124">Header</span></span>       | <span data-ttu-id="2de1f-125">Значение</span><span class="sxs-lookup"><span data-stu-id="2de1f-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2de1f-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2de1f-126">Authorization</span></span>  | <span data-ttu-id="2de1f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2de1f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2de1f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2de1f-129">Request body</span></span>
<span data-ttu-id="2de1f-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2de1f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2de1f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="2de1f-131">Response</span></span>

<span data-ttu-id="2de1f-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [tab](../resources/teamstab.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2de1f-132">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2de1f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2de1f-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2de1f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2de1f-134">Request</span></span>
<span data-ttu-id="2de1f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2de1f-135">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="2de1f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2de1f-136">Response</span></span>
<span data-ttu-id="2de1f-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2de1f-137">The following is an example of the response.</span></span> 

><span data-ttu-id="2de1f-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2de1f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "tabId",
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
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get a channel tab",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
