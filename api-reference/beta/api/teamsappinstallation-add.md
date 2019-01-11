---
title: Добавление приложения в группу
description: Пакет приложения для указанной группы.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: d3f67b8ea49f9940b60bcf0aec7eea15a59388b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855862"
---
# <a name="add-app-to-team"></a><span data-ttu-id="d77e4-103">Добавление приложения в группу</span><span class="sxs-lookup"><span data-stu-id="d77e4-103">Add app to team</span></span>

> <span data-ttu-id="d77e4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d77e4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d77e4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d77e4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d77e4-106">Пакет [приложения](../resources/teamsapp.md) для указанной [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="d77e4-106">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d77e4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d77e4-107">Permissions</span></span>
<span data-ttu-id="d77e4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d77e4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d77e4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d77e4-110">Permission type</span></span>      | <span data-ttu-id="d77e4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d77e4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d77e4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d77e4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d77e4-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d77e4-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d77e4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d77e4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d77e4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d77e4-115">Not supported.</span></span>    |
|<span data-ttu-id="d77e4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d77e4-116">Application</span></span> | <span data-ttu-id="d77e4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d77e4-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d77e4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d77e4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="d77e4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d77e4-119">Request headers</span></span>
| <span data-ttu-id="d77e4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d77e4-120">Header</span></span>       | <span data-ttu-id="d77e4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d77e4-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d77e4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d77e4-122">Authorization</span></span>  | <span data-ttu-id="d77e4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d77e4-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d77e4-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d77e4-125">Request body</span></span>

| <span data-ttu-id="d77e4-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="d77e4-126">Property</span></span>     | <span data-ttu-id="d77e4-127">Тип</span><span class="sxs-lookup"><span data-stu-id="d77e4-127">Type</span></span>   |<span data-ttu-id="d77e4-128">Описание</span><span class="sxs-lookup"><span data-stu-id="d77e4-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d77e4-129">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d77e4-129">teamsApp</span></span>|<span data-ttu-id="d77e4-130">Строка</span><span class="sxs-lookup"><span data-stu-id="d77e4-130">String</span></span>|<span data-ttu-id="d77e4-131">Идентификатор приложения для добавления.</span><span class="sxs-lookup"><span data-stu-id="d77e4-131">The id of the app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="d77e4-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="d77e4-132">Response</span></span>

<span data-ttu-id="d77e4-133">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="d77e4-133">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="d77e4-134">Пример</span><span class="sxs-lookup"><span data-stu-id="d77e4-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d77e4-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="d77e4-135">Request</span></span>
<span data-ttu-id="d77e4-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d77e4-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/installedApps
{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
#### <a name="response"></a><span data-ttu-id="d77e4-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="d77e4-137">Response</span></span>
<span data-ttu-id="d77e4-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d77e4-138">The following is an example of the response.</span></span> <span data-ttu-id="d77e4-139">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="d77e4-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d77e4-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d77e4-140">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

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

## <a name="see-also"></a><span data-ttu-id="d77e4-141">См. также</span><span class="sxs-lookup"><span data-stu-id="d77e4-141">See also</span></span>

