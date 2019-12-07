---
title: Удаление Опеншифтчанжерекуест
description: Удаление объекта Опеншифтчанжерекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1b3370a17b6f16351b3a9db944f9ae636560fe3a
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895823"
---
# <a name="delete-openshiftchangerequest"></a><span data-ttu-id="41236-103">Удаление Опеншифтчанжерекуест</span><span class="sxs-lookup"><span data-stu-id="41236-103">Delete openShiftChangeRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41236-104">Удаление [опеншифтчанжерекуест](../resources/openshiftchangerequest.md).</span><span class="sxs-lookup"><span data-stu-id="41236-104">Delete an [openShiftChangeRequest](../resources/openshiftchangerequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="41236-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41236-105">Permissions</span></span>

<span data-ttu-id="41236-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41236-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="41236-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41236-108">Permission type</span></span>                        | <span data-ttu-id="41236-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="41236-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="41236-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41236-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="41236-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41236-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="41236-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41236-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41236-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41236-113">Not supported.</span></span> |
| <span data-ttu-id="41236-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41236-114">Application</span></span>                            | <span data-ttu-id="41236-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41236-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="41236-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41236-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{id}/schedule/openShiftsChangeRequests
```

## <a name="request-headers"></a><span data-ttu-id="41236-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41236-117">Request headers</span></span>

| <span data-ttu-id="41236-118">Имя</span><span class="sxs-lookup"><span data-stu-id="41236-118">Name</span></span>          | <span data-ttu-id="41236-119">Описание</span><span class="sxs-lookup"><span data-stu-id="41236-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="41236-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41236-120">Authorization</span></span> | <span data-ttu-id="41236-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41236-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41236-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="41236-123">Request body</span></span>

<span data-ttu-id="41236-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="41236-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41236-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="41236-125">Response</span></span>

<span data-ttu-id="41236-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="41236-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="41236-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="41236-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="41236-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="41236-129">Request</span></span>

<span data-ttu-id="41236-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41236-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_openshiftchangerequest"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftsChangeRequests
```

### <a name="response"></a><span data-ttu-id="41236-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="41236-131">Response</span></span>

<span data-ttu-id="41236-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="41236-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete openShiftChangeRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
