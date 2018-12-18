---
title: 'вызов: changeScreenSharingRole'
description: Запуск и остановка совместного использования экрана в вызове. Этот интерфейс API используется для разрешения приложений для совместного использования экрана содержимое с участниками звонок или собрания.
author: VinodRavichandran
ms.openlocfilehash: 4b4c7e0afa452bef414dd466086463aa16c9d9cf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328366"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="7d9c2-104">вызов: changeScreenSharingRole</span><span class="sxs-lookup"><span data-stu-id="7d9c2-104">call: changeScreenSharingRole</span></span>

> <span data-ttu-id="7d9c2-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7d9c2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d9c2-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d9c2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7d9c2-107">Запуск и остановка совместного использования экрана в вызове.</span><span class="sxs-lookup"><span data-stu-id="7d9c2-107">Start and stop sharing screen in the call.</span></span> <span data-ttu-id="7d9c2-108">Этот интерфейс API используется для разрешения приложений для совместного использования экрана содержимое с участниками звонок или собрания.</span><span class="sxs-lookup"><span data-stu-id="7d9c2-108">This API is used to allow applications to share screen content with the participants of a call or meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d9c2-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7d9c2-109">Permissions</span></span>
<span data-ttu-id="7d9c2-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d9c2-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7d9c2-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d9c2-112">Permission type</span></span>                        | <span data-ttu-id="7d9c2-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d9c2-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7d9c2-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d9c2-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="7d9c2-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7d9c2-115">Not Supported</span></span>                               |
| <span data-ttu-id="7d9c2-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d9c2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d9c2-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7d9c2-117">Not Supported</span></span>                               |
| <span data-ttu-id="7d9c2-118">Application</span><span class="sxs-lookup"><span data-stu-id="7d9c2-118">Application</span></span>                            | <span data-ttu-id="7d9c2-119">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="7d9c2-119">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="7d9c2-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d9c2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/changeScreenSharingRole
POST /applications/{id}/calls/{id}/changeScreenSharingRole
```

## <a name="request-headers"></a><span data-ttu-id="7d9c2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d9c2-121">Request headers</span></span>
| <span data-ttu-id="7d9c2-122">Имя</span><span class="sxs-lookup"><span data-stu-id="7d9c2-122">Name</span></span>          | <span data-ttu-id="7d9c2-123">Описание</span><span class="sxs-lookup"><span data-stu-id="7d9c2-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="7d9c2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7d9c2-124">Authorization</span></span> | <span data-ttu-id="7d9c2-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d9c2-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d9c2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d9c2-127">Request body</span></span>
<span data-ttu-id="7d9c2-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="7d9c2-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7d9c2-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="7d9c2-129">Parameter</span></span>      | <span data-ttu-id="7d9c2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7d9c2-130">Type</span></span>    |<span data-ttu-id="7d9c2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7d9c2-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d9c2-132">role</span><span class="sxs-lookup"><span data-stu-id="7d9c2-132">role</span></span>|<span data-ttu-id="7d9c2-133">String.</span><span class="sxs-lookup"><span data-stu-id="7d9c2-133">String</span></span>|<span data-ttu-id="7d9c2-134">Возможные значения: «Средство просмотра», «Активного проекта»</span><span class="sxs-lookup"><span data-stu-id="7d9c2-134">Possible values are: 'Viewer', 'Sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="7d9c2-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="7d9c2-135">Response</span></span>
<span data-ttu-id="7d9c2-136">Возвращает `202 Accepted` код ответа.</span><span class="sxs-lookup"><span data-stu-id="7d9c2-136">Returns `202 Accepted` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7d9c2-137">Пример</span><span class="sxs-lookup"><span data-stu-id="7d9c2-137">Example</span></span>
<span data-ttu-id="7d9c2-138">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="7d9c2-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="7d9c2-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d9c2-139">Request</span></span>
<span data-ttu-id="7d9c2-140">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d9c2-140">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call_changeScreenSharingRole"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/changeScreenSharingRole
Content-Type: application/json
Content-Length: 24

{
  "role": "viewer"
}
```

##### <a name="response"></a><span data-ttu-id="7d9c2-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="7d9c2-141">Response</span></span>
<span data-ttu-id="7d9c2-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7d9c2-142">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: changeScreenSharingRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
