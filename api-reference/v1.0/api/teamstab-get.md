---
title: Получить вкладки
description: 'Извлечение свойств и отношения между заданной вкладки. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: dd23ffc6bcfdeb8821e2227331e2be801f348ce8
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016676"
---
# <a name="get-tab"></a><span data-ttu-id="1596b-103">Получить вкладки</span><span class="sxs-lookup"><span data-stu-id="1596b-103">Get tab</span></span>



<span data-ttu-id="1596b-104">Извлечение свойств и связи указанного [вкладки](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="1596b-104">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="1596b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1596b-105">Permissions</span></span>
<span data-ttu-id="1596b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1596b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1596b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1596b-108">Permission type</span></span>      | <span data-ttu-id="1596b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1596b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1596b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1596b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1596b-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1596b-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1596b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1596b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1596b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1596b-113">Not supported.</span></span>    |
|<span data-ttu-id="1596b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1596b-114">Application</span></span> | <span data-ttu-id="1596b-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1596b-115">Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="1596b-116">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="1596b-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="1596b-117">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="1596b-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1596b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1596b-118">HTTP request</span></span>
```http
GET /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1596b-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1596b-119">Optional query parameters</span></span>

<span data-ttu-id="1596b-120">Этот метод поддерживает $select и $разверните [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1596b-120">This method supports the $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1596b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1596b-121">Request headers</span></span>
| <span data-ttu-id="1596b-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1596b-122">Header</span></span>       | <span data-ttu-id="1596b-123">Значение</span><span class="sxs-lookup"><span data-stu-id="1596b-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1596b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1596b-124">Authorization</span></span>  | <span data-ttu-id="1596b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1596b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1596b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1596b-127">Request body</span></span>
<span data-ttu-id="1596b-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1596b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1596b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1596b-129">Response</span></span>

<span data-ttu-id="1596b-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [tab](../resources/teamstab.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1596b-130">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1596b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1596b-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1596b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1596b-132">Request</span></span>
<span data-ttu-id="1596b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1596b-133">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="1596b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1596b-134">Response</span></span>
<span data-ttu-id="1596b-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1596b-135">The following is an example of the response.</span></span> 

><span data-ttu-id="1596b-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1596b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
