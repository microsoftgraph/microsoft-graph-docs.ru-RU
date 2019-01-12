---
title: Добавление приложения в группу
description: Пакет приложения для указанной группы.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8332204de2c75235720d7b2652d029e9f145f576
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922377"
---
# <a name="add-app-to-team"></a><span data-ttu-id="7f61c-103">Добавление приложения в группу</span><span class="sxs-lookup"><span data-stu-id="7f61c-103">Add app to team</span></span>



<span data-ttu-id="7f61c-104">Пакет [приложения](../resources/teamsapp.md) для указанной [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="7f61c-104">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7f61c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f61c-105">Permissions</span></span>
<span data-ttu-id="7f61c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f61c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f61c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f61c-108">Permission type</span></span>      | <span data-ttu-id="7f61c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f61c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f61c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f61c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7f61c-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f61c-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7f61c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f61c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f61c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f61c-113">Not supported.</span></span>    |
|<span data-ttu-id="7f61c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f61c-114">Application</span></span> | <span data-ttu-id="7f61c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f61c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f61c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f61c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="7f61c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f61c-117">Request headers</span></span>
| <span data-ttu-id="7f61c-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f61c-118">Header</span></span>       | <span data-ttu-id="7f61c-119">Значение</span><span class="sxs-lookup"><span data-stu-id="7f61c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7f61c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7f61c-120">Authorization</span></span>  | <span data-ttu-id="7f61c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f61c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7f61c-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7f61c-123">Request body</span></span>

| <span data-ttu-id="7f61c-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f61c-124">Property</span></span>     | <span data-ttu-id="7f61c-125">Тип</span><span class="sxs-lookup"><span data-stu-id="7f61c-125">Type</span></span>   |<span data-ttu-id="7f61c-126">Описание</span><span class="sxs-lookup"><span data-stu-id="7f61c-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f61c-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="7f61c-127">teamsApp</span></span>| [<span data-ttu-id="7f61c-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="7f61c-128">teamsApp</span></span>](../resources/teamsapp.md) |<span data-ttu-id="7f61c-129">Чтобы добавить приложение.</span><span class="sxs-lookup"><span data-stu-id="7f61c-129">The app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="7f61c-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f61c-130">Response</span></span>

<span data-ttu-id="7f61c-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="7f61c-131">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7f61c-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7f61c-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7f61c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f61c-133">Request</span></span>
<span data-ttu-id="7f61c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f61c-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST /teams/{id}/installedApps
{
   "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
#### <a name="response"></a><span data-ttu-id="7f61c-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f61c-135">Response</span></span>
<span data-ttu-id="7f61c-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7f61c-136">The following is an example of the response.</span></span> <span data-ttu-id="7f61c-137">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="7f61c-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7f61c-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7f61c-138">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="7f61c-139">См. также</span><span class="sxs-lookup"><span data-stu-id="7f61c-139">See also</span></span>

