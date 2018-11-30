---
title: Получить вкладки
description: 'Извлечение свойств и отношения между заданной вкладки. '
ms.openlocfilehash: 57bd7d8b11b0bf20d54bf8da16cdd41220320fcd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075085"
---
# <a name="get-tab"></a><span data-ttu-id="45f47-103">Получить вкладки</span><span class="sxs-lookup"><span data-stu-id="45f47-103">Get tab</span></span>

> <span data-ttu-id="45f47-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="45f47-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45f47-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45f47-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="45f47-106">Извлечение свойств и связи указанного [вкладки](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="45f47-106">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="45f47-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="45f47-107">Permissions</span></span>
<span data-ttu-id="45f47-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45f47-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45f47-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45f47-110">Permission type</span></span>      | <span data-ttu-id="45f47-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="45f47-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45f47-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45f47-112">Delegated (work or school account)</span></span> | <span data-ttu-id="45f47-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45f47-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="45f47-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45f47-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45f47-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45f47-115">Not supported.</span></span>    |
|<span data-ttu-id="45f47-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45f47-116">Application</span></span> | <span data-ttu-id="45f47-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45f47-117">Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="45f47-118">На данный момент только [делегированных разрешений](/graph/permissions-reference) поддерживаются для этой операции.</span><span class="sxs-lookup"><span data-stu-id="45f47-118">Currently, only [delegated permissions](/graph/permissions-reference) are supported for this operation.</span></span>

## <a name="http-request"></a><span data-ttu-id="45f47-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45f47-119">HTTP request</span></span>
```http
GET /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="45f47-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="45f47-120">Optional query parameters</span></span>

<span data-ttu-id="45f47-121">Этот метод поддерживает $select и $разверните [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="45f47-121">This method supports the $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="45f47-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45f47-122">Request headers</span></span>
| <span data-ttu-id="45f47-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45f47-123">Header</span></span>       | <span data-ttu-id="45f47-124">Значение</span><span class="sxs-lookup"><span data-stu-id="45f47-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="45f47-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="45f47-125">Authorization</span></span>  | <span data-ttu-id="45f47-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45f47-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="45f47-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45f47-128">Request body</span></span>
<span data-ttu-id="45f47-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="45f47-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45f47-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="45f47-130">Response</span></span>

<span data-ttu-id="45f47-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [tab](../resources/teamstab.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="45f47-131">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="45f47-132">Пример</span><span class="sxs-lookup"><span data-stu-id="45f47-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="45f47-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="45f47-133">Request</span></span>
<span data-ttu-id="45f47-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45f47-134">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="45f47-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="45f47-135">Response</span></span>
<span data-ttu-id="45f47-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="45f47-136">The following is an example of the response.</span></span> 

><span data-ttu-id="45f47-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="45f47-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
