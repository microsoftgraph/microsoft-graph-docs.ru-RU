---
title: Создание Воркфорцеинтегратион
description: Создание нового объекта Воркфорцеинтегратион.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e6da06c27296009bcf337171af6e77d5cc55eeb0
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895798"
---
# <a name="create-workforceintegration"></a><span data-ttu-id="f20d4-103">Создание Воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="f20d4-103">Create workforceIntegration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f20d4-104">Создание нового объекта [воркфорцеинтегратион](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="f20d4-104">Create a new [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f20d4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f20d4-105">Permissions</span></span>

<span data-ttu-id="f20d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f20d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f20d4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f20d4-108">Permission type</span></span>                        | <span data-ttu-id="f20d4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f20d4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f20d4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f20d4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f20d4-111">Воркфорцеинтегратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f20d4-111">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="f20d4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f20d4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f20d4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f20d4-113">Not supported.</span></span> |
| <span data-ttu-id="f20d4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f20d4-114">Application</span></span>                            | <span data-ttu-id="f20d4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f20d4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f20d4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f20d4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="f20d4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f20d4-117">Request headers</span></span>

| <span data-ttu-id="f20d4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f20d4-118">Name</span></span>          | <span data-ttu-id="f20d4-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f20d4-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f20d4-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f20d4-120">Authorization</span></span> | <span data-ttu-id="f20d4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f20d4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f20d4-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f20d4-123">Content-type</span></span> | <span data-ttu-id="f20d4-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f20d4-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f20d4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f20d4-126">Request body</span></span>

<span data-ttu-id="f20d4-127">В тексте запроса добавьте представление объекта [воркфорцеинтегратион](../resources/workforceintegration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f20d4-127">In the request body, supply a JSON representation of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f20d4-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f20d4-128">Response</span></span>

<span data-ttu-id="f20d4-129">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [воркфорцеинтегратион](../resources/workforceintegration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f20d4-129">If successful, this method returns a `201 Created` response code and a new [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f20d4-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="f20d4-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f20d4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f20d4-131">Request</span></span>

<span data-ttu-id="f20d4-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f20d4-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_workforceintegration_from_teamwork"
}-->

```http
POST https://graph.microsoft.com/beta/teamwork/workforceIntegrations
Content-type: application/json

{
  "displayName": "displayName-value",
  "apiVersion": 99,
  "encryption": {
    "protocol": "protocol-value",
    "secret": "secret-value"
  },
  "isActive": true,
  "url": "url-value",
  "supports": "supports-value"
}
```

### <a name="response"></a><span data-ttu-id="f20d4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f20d4-133">Response</span></span>

<span data-ttu-id="f20d4-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f20d4-134">The following is an example of the response.</span></span>

> <span data-ttu-id="f20d4-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f20d4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "displayName": "displayName-value",
  "apiVersion": 99,
  "encryption": {
    "protocol": "protocol-value",
    "secret": "secret-value"
  },
  "isActive": true,
  "url": "url-value",
  "supports": "supports-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create workforceIntegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
