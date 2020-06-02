---
title: Получение вкладки
description: 'Получение свойств и связей указанной вкладки. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5e8a2cfc5c17cbd90dd713d3cb19e43ee24b32ea
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491723"
---
# <a name="get-tab"></a><span data-ttu-id="de92f-103">Получение вкладки</span><span class="sxs-lookup"><span data-stu-id="de92f-103">Get tab</span></span>

<span data-ttu-id="de92f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de92f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de92f-105">Получение свойств и связей указанной [вкладки](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="de92f-105">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="de92f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de92f-106">Permissions</span></span>
<span data-ttu-id="de92f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de92f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de92f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de92f-109">Permission type</span></span>      | <span data-ttu-id="de92f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de92f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de92f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de92f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="de92f-112">TeamsTab. Read. ALL, TeamsTab. ReadWrite. ALL, Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="de92f-112">TeamsTab.Read.All, TeamsTab.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="de92f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de92f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de92f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de92f-114">Not supported.</span></span>    |
|<span data-ttu-id="de92f-115">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="de92f-115">Application</span></span> | <span data-ttu-id="de92f-116">TeamsTab. Read. Group *, TeamsTab. Edit. Group*, TeamsTab. Read. ALL, TeamsTab. ReadWrite. ALL, Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="de92f-116">TeamsTab.Read.Group *, TeamsTab.Edit.Group*, TeamsTab.Read.All, TeamsTab.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
> <span data-ttu-id="de92f-117">**Note**: разрешения, помеченные как \* использовать [согласие с определенным ресурсом]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="de92f-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="de92f-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="de92f-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="de92f-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="de92f-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="de92f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de92f-120">HTTP request</span></span>
```http
GET /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="de92f-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="de92f-121">Optional query parameters</span></span>

<span data-ttu-id="de92f-122">Этот метод поддерживает $select и $expand [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="de92f-122">This method supports the $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="de92f-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de92f-123">Request headers</span></span>
| <span data-ttu-id="de92f-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de92f-124">Header</span></span>       | <span data-ttu-id="de92f-125">Значение</span><span class="sxs-lookup"><span data-stu-id="de92f-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="de92f-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de92f-126">Authorization</span></span>  | <span data-ttu-id="de92f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de92f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="de92f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de92f-129">Request body</span></span>
<span data-ttu-id="de92f-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="de92f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de92f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="de92f-131">Response</span></span>

<span data-ttu-id="de92f-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Tab](../resources/teamstab.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="de92f-132">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="de92f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="de92f-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="de92f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="de92f-134">Request</span></span>
<span data-ttu-id="de92f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de92f-135">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}?$expand=teamsApp
```
#### <a name="response"></a><span data-ttu-id="de92f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="de92f-136">Response</span></span>
<span data-ttu-id="de92f-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="de92f-137">The following is an example of the response.</span></span> 

><span data-ttu-id="de92f-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de92f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": []
}
-->
