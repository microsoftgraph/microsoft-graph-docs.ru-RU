---
title: Добавление приложения в команду
description: Устанавливает приложение в указанную группу.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b1a241ebb9d39b26e12f59b6f8f08e71220d8021
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521896"
---
# <a name="add-app-to-team"></a><span data-ttu-id="4b645-103">Добавление приложения в команду</span><span class="sxs-lookup"><span data-stu-id="4b645-103">Add app to team</span></span>



<span data-ttu-id="4b645-104">Устанавливает [приложение](../resources/teamsapp.md) в указанную [группу](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="4b645-104">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4b645-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b645-105">Permissions</span></span>
<span data-ttu-id="4b645-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b645-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b645-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b645-108">Permission type</span></span>      | <span data-ttu-id="4b645-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b645-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b645-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b645-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4b645-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b645-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4b645-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b645-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b645-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b645-113">Not supported.</span></span>    |
|<span data-ttu-id="4b645-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b645-114">Application</span></span> | <span data-ttu-id="4b645-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b645-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b645-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b645-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="4b645-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b645-117">Request headers</span></span>
| <span data-ttu-id="4b645-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b645-118">Header</span></span>       | <span data-ttu-id="4b645-119">Значение</span><span class="sxs-lookup"><span data-stu-id="4b645-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4b645-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b645-120">Authorization</span></span>  | <span data-ttu-id="4b645-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b645-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4b645-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b645-123">Request body</span></span>

| <span data-ttu-id="4b645-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b645-124">Property</span></span>     | <span data-ttu-id="4b645-125">Тип</span><span class="sxs-lookup"><span data-stu-id="4b645-125">Type</span></span>   |<span data-ttu-id="4b645-126">Описание</span><span class="sxs-lookup"><span data-stu-id="4b645-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b645-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="4b645-127">teamsApp</span></span>| [<span data-ttu-id="4b645-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="4b645-128">teamsApp</span></span>](../resources/teamsapp.md) |<span data-ttu-id="4b645-129">Добавляемое приложение.</span><span class="sxs-lookup"><span data-stu-id="4b645-129">The app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="4b645-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b645-130">Response</span></span>

<span data-ttu-id="4b645-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="4b645-131">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4b645-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4b645-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4b645-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b645-133">Request</span></span>
<span data-ttu-id="4b645-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b645-134">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="4b645-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b645-135">Response</span></span>
<span data-ttu-id="4b645-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4b645-136">The following is an example of the response.</span></span> <span data-ttu-id="4b645-137">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="4b645-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4b645-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b645-138">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="4b645-139">См. также</span><span class="sxs-lookup"><span data-stu-id="4b645-139">See also</span></span>

