---
title: Добавление приложения в группу
description: Пакет приложения для указанной группы.
ms.openlocfilehash: de5817f243b02462817d23d0e2b3864d5644b1d4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025907"
---
# <a name="add-app-to-team"></a><span data-ttu-id="d912e-103">Добавление приложения в группу</span><span class="sxs-lookup"><span data-stu-id="d912e-103">Add app to team</span></span>



<span data-ttu-id="d912e-104">Пакет [приложения](../resources/teamsapp.md) для указанной [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="d912e-104">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d912e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d912e-105">Permissions</span></span>
<span data-ttu-id="d912e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d912e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d912e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d912e-108">Permission type</span></span>      | <span data-ttu-id="d912e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d912e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d912e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d912e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d912e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d912e-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d912e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d912e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d912e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d912e-113">Not supported.</span></span>    |
|<span data-ttu-id="d912e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d912e-114">Application</span></span> | <span data-ttu-id="d912e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d912e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d912e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d912e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="d912e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d912e-117">Request headers</span></span>
| <span data-ttu-id="d912e-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d912e-118">Header</span></span>       | <span data-ttu-id="d912e-119">Значение</span><span class="sxs-lookup"><span data-stu-id="d912e-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d912e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d912e-120">Authorization</span></span>  | <span data-ttu-id="d912e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d912e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d912e-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d912e-123">Request body</span></span>

| <span data-ttu-id="d912e-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="d912e-124">Property</span></span>     | <span data-ttu-id="d912e-125">Тип</span><span class="sxs-lookup"><span data-stu-id="d912e-125">Type</span></span>   |<span data-ttu-id="d912e-126">Описание</span><span class="sxs-lookup"><span data-stu-id="d912e-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d912e-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d912e-127">teamsApp</span></span>| [<span data-ttu-id="d912e-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d912e-128">teamsApp</span></span>](../resources/teamsapp.md) |<span data-ttu-id="d912e-129">Чтобы добавить приложение.</span><span class="sxs-lookup"><span data-stu-id="d912e-129">The app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="d912e-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="d912e-130">Response</span></span>

<span data-ttu-id="d912e-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="d912e-131">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d912e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d912e-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d912e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d912e-133">Request</span></span>
<span data-ttu-id="d912e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d912e-134">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="d912e-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="d912e-135">Response</span></span>
<span data-ttu-id="d912e-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d912e-136">The following is an example of the response.</span></span> <span data-ttu-id="d912e-137">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="d912e-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d912e-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d912e-138">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="d912e-139">См. также</span><span class="sxs-lookup"><span data-stu-id="d912e-139">See also</span></span>

