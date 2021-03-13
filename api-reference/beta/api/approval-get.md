---
title: Получить утверждение
description: Извлечение свойств объекта утверждения.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f9f2a3c1d32d578937a6d124da73136292958cfc
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760786"
---
# <a name="get-approval"></a><span data-ttu-id="4c377-103">Получить утверждение</span><span class="sxs-lookup"><span data-stu-id="4c377-103">Get approval</span></span>

<span data-ttu-id="4c377-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c377-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c377-105">Извлечение свойств объекта [утверждения.](../resources/approval.md)</span><span class="sxs-lookup"><span data-stu-id="4c377-105">Retrieve the properties of an [approval](../resources/approval.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c377-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c377-106">Permissions</span></span>

<span data-ttu-id="4c377-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c377-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4c377-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c377-109">Permission type</span></span>                        | <span data-ttu-id="4c377-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c377-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4c377-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c377-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4c377-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c377-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="4c377-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c377-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c377-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c377-114">Not supported.</span></span> |
| <span data-ttu-id="4c377-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c377-115">Application</span></span>                            | <span data-ttu-id="4c377-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c377-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c377-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c377-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4c377-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c377-118">Request headers</span></span>

| <span data-ttu-id="4c377-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4c377-119">Name</span></span>      |<span data-ttu-id="4c377-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4c377-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4c377-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c377-121">Authorization</span></span> | <span data-ttu-id="4c377-122">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="4c377-122">Bearer \{token\}.</span></span> <span data-ttu-id="4c377-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="4c377-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c377-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c377-124">Request body</span></span>

<span data-ttu-id="4c377-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4c377-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c377-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c377-126">Response</span></span>

<span data-ttu-id="4c377-127">В случае успеха этот метод возвращает код ответа и запрашиваемого объекта `200 OK` утверждения в тексте ответа. [](../resources/approval.md)</span><span class="sxs-lookup"><span data-stu-id="4c377-127">If successful, this method returns a `200 OK` response code and the requested [approval](../resources/approval.md) object in the response body.</span></span> <span data-ttu-id="4c377-128">Однако если у вызываемого не имеется нужных разрешений, метод возвращает `403 Forbidden` код ответа.</span><span class="sxs-lookup"><span data-stu-id="4c377-128">However, if the caller does not have the right permissions, the method returns a `403 Forbidden` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4c377-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="4c377-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4c377-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c377-130">Request</span></span>

<span data-ttu-id="4c377-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c377-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_approval"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489
```
---


### <a name="response"></a><span data-ttu-id="4c377-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c377-132">Response</span></span>

<span data-ttu-id="4c377-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4c377-133">The following is an example of the response.</span></span>

> <span data-ttu-id="4c377-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4c377-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approval"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "abd306ef-f7b2-4a10-9fd1-493454322489",
    "steps": [
        {
            "id": "d4fa4045-4716-436d-aec5-57b0a713f095",
            "displayName": null,
            "reviewedDateTime": null,
            "reviewResult": "NotReviewed",
            "status": "InProgress",
            "assignedToMe": true,
            "justification": "",
            "reviewedBy": null
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-02-12 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get approval",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


