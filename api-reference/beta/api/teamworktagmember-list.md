---
title: Список командной работыTagMembers
description: Получите список объектов teamworkTagMember и их свойств.
author: anniecolonna
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c0eca6f9469f53cb639068d712421e85b27e185f
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209166"
---
# <a name="list-members-in-a-teamworktag"></a><span data-ttu-id="ecc9b-103">Список участников в командной работеTag</span><span class="sxs-lookup"><span data-stu-id="ecc9b-103">List members in a teamworkTag</span></span>
<span data-ttu-id="ecc9b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecc9b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ecc9b-105">Получите список участников [стандартного](../resources/teamworktagmember.md) тега в команде и их свойства.</span><span class="sxs-lookup"><span data-stu-id="ecc9b-105">Get a list of the [members](../resources/teamworktagmember.md) of a standard tag in a team and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="ecc9b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ecc9b-106">Permissions</span></span>
<span data-ttu-id="ecc9b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecc9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecc9b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ecc9b-109">Permission type</span></span>|<span data-ttu-id="ecc9b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ecc9b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecc9b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ecc9b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ecc9b-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecc9b-112">Not supported.</span></span>|
|<span data-ttu-id="ecc9b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ecc9b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecc9b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecc9b-114">Not supported.</span></span>|
|<span data-ttu-id="ecc9b-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="ecc9b-115">Application</span></span>|<span data-ttu-id="ecc9b-116">TeamworkTag.Read.All, TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecc9b-116">TeamworkTag.Read.All, TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecc9b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ecc9b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-Id}/tags/{teamworkTag-Id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ecc9b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ecc9b-118">Optional query parameters</span></span>
<span data-ttu-id="ecc9b-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ecc9b-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ecc9b-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ecc9b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ecc9b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ecc9b-121">Request headers</span></span>
|<span data-ttu-id="ecc9b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ecc9b-122">Name</span></span>|<span data-ttu-id="ecc9b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ecc9b-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ecc9b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ecc9b-124">Authorization</span></span>|<span data-ttu-id="ecc9b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ecc9b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecc9b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ecc9b-127">Request body</span></span>
<span data-ttu-id="ecc9b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ecc9b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecc9b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecc9b-129">Response</span></span>

<span data-ttu-id="ecc9b-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [teamworkTagMember](../resources/teamworktagmember.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ecc9b-130">If successful, this method returns a `200 OK` response code and a collection of [teamworkTagMember](../resources/teamworktagmember.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ecc9b-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="ecc9b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ecc9b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ecc9b-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ecc9b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ecc9b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamworktagmember"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==/members
```
# <a name="c"></a>[<span data-ttu-id="ecc9b-134">C#</span><span class="sxs-lookup"><span data-stu-id="ecc9b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamworktagmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ecc9b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ecc9b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamworktagmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ecc9b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ecc9b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamworktagmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ecc9b-137">Java</span><span class="sxs-lookup"><span data-stu-id="ecc9b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamworktagmember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ecc9b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecc9b-138">Response</span></span>
><span data-ttu-id="ecc9b-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ecc9b-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkTagMember",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.teamworkTagMember",
      "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyNlYjY1M2Y5Mi04MzczLTRkZTYtYmZlYy01YjRkMjE2YjZhZGUjI2QzYjJiM2ViLWM0N2YtNDViOS05NWYyLWIyZjJlZjYyMTVjZQ==",
      "displayName": "Grady Archie",
      "tenantId": "18be64a9-c73a-4862-bccc-76c31ef09b9d",
      "userId": "92f6952f-61ca-4a94-8910-508a240bc167"
    },
    {
      "@odata.type": "#microsoft.graph.teamworkTagMember",
      "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyNlYjY1M2Y5Mi04MzczLTRkZTYtYmZlYy01YjRkMjE2YjZhZGUjI2QzYjJiM2ViLMW0N2YtNDViOS05NWYyLWIyZjJlZjYyGHVjZQ==",
      "displayName": "Lee Gu",
      "tenantId": "18be64a9-c73a-4862-bccc-76c31ef09b9d",    
      "userId": "945fe02a-5dc1-4d28-bf5c-30a6147fe842"
    }
  ]
}
```
