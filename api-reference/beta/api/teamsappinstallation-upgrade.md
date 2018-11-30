---
title: Обновление приложения в группе
description: Обновляет установку приложения в группе
ms.openlocfilehash: 90cec9dcb41b27a239661f3ed1850e073775be71
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079506"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="137e1-103">Обновление приложения в группе</span><span class="sxs-lookup"><span data-stu-id="137e1-103">Upgrade an app in a team</span></span>

> <span data-ttu-id="137e1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="137e1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="137e1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="137e1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="137e1-106">Обновляет [установки приложения](../resources/teamsappinstallation.md) в [группы](../resources/team.md) до последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="137e1-106">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="137e1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="137e1-107">Permissions</span></span>

<span data-ttu-id="137e1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="137e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="137e1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="137e1-110">Permission type</span></span>      | <span data-ttu-id="137e1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="137e1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="137e1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="137e1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="137e1-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="137e1-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="137e1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="137e1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="137e1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="137e1-115">Not supported.</span></span>    |
|<span data-ttu-id="137e1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="137e1-116">Application</span></span> | <span data-ttu-id="137e1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="137e1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="137e1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="137e1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="137e1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="137e1-119">Request headers</span></span>
| <span data-ttu-id="137e1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="137e1-120">Header</span></span>       | <span data-ttu-id="137e1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="137e1-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="137e1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="137e1-122">Authorization</span></span>  | <span data-ttu-id="137e1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="137e1-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="137e1-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="137e1-125">Request body</span></span>
<span data-ttu-id="137e1-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="137e1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="137e1-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="137e1-127">Response</span></span>

<span data-ttu-id="137e1-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="137e1-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="137e1-130">Пример</span><span class="sxs-lookup"><span data-stu-id="137e1-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="137e1-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="137e1-131">Request</span></span>
<span data-ttu-id="137e1-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="137e1-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
#### <a name="response"></a><span data-ttu-id="137e1-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="137e1-133">Response</span></span>
<span data-ttu-id="137e1-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="137e1-134">The following is an example of the response.</span></span> 

><span data-ttu-id="137e1-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="137e1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
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
