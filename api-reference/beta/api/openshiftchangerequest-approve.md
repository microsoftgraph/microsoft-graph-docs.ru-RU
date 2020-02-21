---
title: 'Опеншифтчанжерекуест: утверждение'
description: Утверждение запроса опеншифт.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1301a975dcf858ff1d6f65beb1665d3ca5933de6
ms.sourcegitcommit: 31a9b4cb3d0f905f123475a4c1a86f5b1e59b935
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2020
ms.locfileid: "42219687"
---
# <a name="openshiftchangerequest-approve"></a><span data-ttu-id="63523-103">Опеншифтчанжерекуест: утверждение</span><span class="sxs-lookup"><span data-stu-id="63523-103">openShiftChangeRequest: approve</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63523-104">Утверждение объекта [опеншифтчанжерекуест](../resources/openshiftchangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="63523-104">Approve an [openshiftchangerequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="63523-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="63523-105">Permissions</span></span>

<span data-ttu-id="63523-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63523-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="63523-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63523-108">Permission type</span></span>                        | <span data-ttu-id="63523-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="63523-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="63523-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63523-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="63523-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63523-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="63523-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63523-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63523-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63523-113">Not supported.</span></span> |
| <span data-ttu-id="63523-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63523-114">Application</span></span>                            | <span data-ttu-id="63523-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63523-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="63523-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63523-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftsChangeRequests/{openShiftChangeRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="63523-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63523-117">Request headers</span></span>

| <span data-ttu-id="63523-118">Имя</span><span class="sxs-lookup"><span data-stu-id="63523-118">Name</span></span>          | <span data-ttu-id="63523-119">Описание</span><span class="sxs-lookup"><span data-stu-id="63523-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="63523-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63523-120">Authorization</span></span> | <span data-ttu-id="63523-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63523-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="63523-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="63523-123">Content-type</span></span> | <span data-ttu-id="63523-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63523-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63523-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63523-126">Request body</span></span>

<span data-ttu-id="63523-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="63523-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="63523-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="63523-128">Parameter</span></span>    | <span data-ttu-id="63523-129">Тип</span><span class="sxs-lookup"><span data-stu-id="63523-129">Type</span></span>        | <span data-ttu-id="63523-130">Описание</span><span class="sxs-lookup"><span data-stu-id="63523-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="63523-131">message</span><span class="sxs-lookup"><span data-stu-id="63523-131">message</span></span>|<span data-ttu-id="63523-132">String</span><span class="sxs-lookup"><span data-stu-id="63523-132">String</span></span>|<span data-ttu-id="63523-133">Настраиваемое сообщение утверждения.</span><span class="sxs-lookup"><span data-stu-id="63523-133">A custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="63523-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="63523-134">Response</span></span>

<span data-ttu-id="63523-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="63523-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="63523-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="63523-137">Examples</span></span>

<span data-ttu-id="63523-138">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="63523-138">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="63523-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="63523-139">Request</span></span>

<span data-ttu-id="63523-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63523-140">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "openshiftchangerequest_approve"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftsChangeRequests/{openShiftChangeRequestId}/approve
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a><span data-ttu-id="63523-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="63523-141">Response</span></span>

<span data-ttu-id="63523-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="63523-142">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openShiftChangeRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
