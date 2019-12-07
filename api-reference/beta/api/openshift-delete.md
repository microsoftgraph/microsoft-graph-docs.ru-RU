---
title: Удаление Опеншифт
description: Удаление объекта Опеншифт.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 006801d123a90fe3f3dc2cad3593df662325902d
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895835"
---
# <a name="delete-openshift"></a><span data-ttu-id="2b5a4-103">Удаление Опеншифт</span><span class="sxs-lookup"><span data-stu-id="2b5a4-103">Delete openShift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b5a4-104">Удаление объекта [опеншифт](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="2b5a4-104">Delete an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b5a4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b5a4-105">Permissions</span></span>

<span data-ttu-id="2b5a4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b5a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2b5a4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b5a4-108">Permission type</span></span>                        | <span data-ttu-id="2b5a4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b5a4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2b5a4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b5a4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2b5a4-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b5a4-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="2b5a4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b5a4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b5a4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b5a4-113">Not supported.</span></span> |
| <span data-ttu-id="2b5a4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b5a4-114">Application</span></span>                            | <span data-ttu-id="2b5a4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b5a4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b5a4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b5a4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{id}/schedule/openShifts
```

## <a name="request-headers"></a><span data-ttu-id="2b5a4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b5a4-117">Request headers</span></span>

| <span data-ttu-id="2b5a4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2b5a4-118">Name</span></span>          | <span data-ttu-id="2b5a4-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2b5a4-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2b5a4-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b5a4-120">Authorization</span></span> | <span data-ttu-id="2b5a4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b5a4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b5a4-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b5a4-123">Request body</span></span>

<span data-ttu-id="2b5a4-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b5a4-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b5a4-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b5a4-125">Response</span></span>

<span data-ttu-id="2b5a4-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2b5a4-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2b5a4-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="2b5a4-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2b5a4-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b5a4-129">Request</span></span>

<span data-ttu-id="2b5a4-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b5a4-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_openshift"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/schedule/openShifts
```

### <a name="response"></a><span data-ttu-id="2b5a4-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b5a4-131">Response</span></span>

<span data-ttu-id="2b5a4-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2b5a4-132">The following is an example of the response.</span></span>

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
  "description": "Delete openShift",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
