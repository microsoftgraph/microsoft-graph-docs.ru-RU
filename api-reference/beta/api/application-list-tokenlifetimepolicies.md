---
title: Список назначенных ТокенлифетимеполиЦиес
description: Список ТокенлифетимеполиЦиес, назначенных приложению или servicePrincipal.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4ffd3395b362a1ecee61005a7663b09793e50f63
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234452"
---
# <a name="list-assigned-tokenlifetimepolicy"></a><span data-ttu-id="60050-103">Список назначенных Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="60050-103">List assigned tokenLifetimePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60050-104">Перечисление объектов [токенлифетимеполици](../resources/tokenlifetimepolicy.md) , назначенных [приложению](../resources/application.md) или [servicePrincipal](../resources/servicePrincipal.md)..</span><span class="sxs-lookup"><span data-stu-id="60050-104">List the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects that are assigned to an [application](../resources/application.md) or [servicePrincipal](../resources/servicePrincipal.md)..</span></span>

## <a name="permissions"></a><span data-ttu-id="60050-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60050-105">Permissions</span></span>

<span data-ttu-id="60050-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60050-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="60050-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60050-108">Permission type</span></span>                        | <span data-ttu-id="60050-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60050-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="60050-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60050-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="60050-111">Policy. Read. ALL и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="60050-111">Policy.Read.All and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="60050-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60050-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60050-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60050-113">Not supported.</span></span> |
| <span data-ttu-id="60050-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="60050-114">Application</span></span>                            | <span data-ttu-id="60050-115">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="60050-115">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60050-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60050-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/tokenLifetimePolicies
GET /servicePrincipals/{id}/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="60050-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60050-117">Request headers</span></span>

| <span data-ttu-id="60050-118">Имя</span><span class="sxs-lookup"><span data-stu-id="60050-118">Name</span></span>          | <span data-ttu-id="60050-119">Описание</span><span class="sxs-lookup"><span data-stu-id="60050-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="60050-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="60050-120">Authorization</span></span> | <span data-ttu-id="60050-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="60050-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="60050-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="60050-122">Request body</span></span>

<span data-ttu-id="60050-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="60050-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60050-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="60050-124">Response</span></span>

<span data-ttu-id="60050-125">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [токенлифетимеполици](../resources/tokenLifetimePolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="60050-125">If successful, this method returns a `200 OK` response code and a collection of [tokenLifetimePolicy](../resources/tokenLifetimePolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="60050-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="60050-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="60050-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="60050-127">Request</span></span>

<span data-ttu-id="60050-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="60050-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_tokenlifetimepolicies_on_application"
}-->

```http
GET https://graph.microsoft.com/beta/applications/{id}/tokenLifetimePolicies
```

### <a name="response"></a><span data-ttu-id="60050-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="60050-129">Response</span></span>

<span data-ttu-id="60050-130">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="60050-130">The following is an example of the response.</span></span>

> <span data-ttu-id="60050-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="60050-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List assigned tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->