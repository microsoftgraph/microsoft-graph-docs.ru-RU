---
title: Получение вкладки
description: 'Получение свойств и связей указанной вкладки. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3d630bcaddd46aaf1428a49035c5502f43be0bfc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027204"
---
# <a name="get-tab"></a><span data-ttu-id="8f8c7-103">Получение вкладки</span><span class="sxs-lookup"><span data-stu-id="8f8c7-103">Get tab</span></span>



<span data-ttu-id="8f8c7-104">Получение свойств и связей указанной [вкладки](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="8f8c7-104">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="8f8c7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f8c7-105">Permissions</span></span>
<span data-ttu-id="8f8c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f8c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f8c7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f8c7-108">Permission type</span></span>      | <span data-ttu-id="8f8c7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f8c7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f8c7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f8c7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8f8c7-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f8c7-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8f8c7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f8c7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f8c7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f8c7-113">Not supported.</span></span>    |
|<span data-ttu-id="8f8c7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f8c7-114">Application</span></span> | <span data-ttu-id="8f8c7-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f8c7-115">Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="8f8c7-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="8f8c7-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8f8c7-117">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="8f8c7-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8f8c7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f8c7-118">HTTP request</span></span>
```http
GET /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8f8c7-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8f8c7-119">Optional query parameters</span></span>

<span data-ttu-id="8f8c7-120">Этот метод поддерживает $select и $expand [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8f8c7-120">This method supports the $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f8c7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f8c7-121">Request headers</span></span>
| <span data-ttu-id="8f8c7-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8f8c7-122">Header</span></span>       | <span data-ttu-id="8f8c7-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8f8c7-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8f8c7-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f8c7-124">Authorization</span></span>  | <span data-ttu-id="8f8c7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f8c7-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8f8c7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8f8c7-127">Request body</span></span>
<span data-ttu-id="8f8c7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8f8c7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f8c7-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="8f8c7-129">Response</span></span>

<span data-ttu-id="8f8c7-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Tab](../resources/teamstab.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8f8c7-130">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8f8c7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8f8c7-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8f8c7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f8c7-132">Request</span></span>
<span data-ttu-id="8f8c7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f8c7-133">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs/{id}?$expand=teamsApp
```
#### <a name="response"></a><span data-ttu-id="8f8c7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f8c7-134">Response</span></span>
<span data-ttu-id="8f8c7-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8f8c7-135">The following is an example of the response.</span></span> 

><span data-ttu-id="8f8c7-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f8c7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "tabId",
  "displayName": "My Contoso Tab - updated",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "teamsApp": {
      "id": "0d820ecd-def2-4297-adad-78056cde7c78",
      "externalId": null,
      "displayName": "Contoso",
      "distributionMethod": "store"
  },
  "sortOrderIndex": "20",
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a channel tab",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
