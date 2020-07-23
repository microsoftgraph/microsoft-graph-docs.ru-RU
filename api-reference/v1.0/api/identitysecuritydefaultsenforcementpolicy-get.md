---
title: Получение Идентитисекуритидефаултсенфорцементполици
description: Получение свойств и связей объекта идентитисекуритидефаултсенфорцементполици.
localization_priority: Normal
author: rohinigoyal1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 48a28d0aa32d8abc23f0c731a0ca4cb89d774e34
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384732"
---
# <a name="get-identitysecuritydefaultsenforcementpolicy"></a><span data-ttu-id="afa02-103">Получение Идентитисекуритидефаултсенфорцементполици</span><span class="sxs-lookup"><span data-stu-id="afa02-103">Get identitySecurityDefaultsEnforcementPolicy</span></span>

<span data-ttu-id="afa02-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afa02-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="afa02-105">Получение свойств объекта [идентитисекуритидефаултсенфорцементполици](../resources/identitysecuritydefaultsenforcementpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="afa02-105">Retrieve the properties of an [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="afa02-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="afa02-106">Permissions</span></span>

<span data-ttu-id="afa02-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afa02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="afa02-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="afa02-109">Permission type</span></span>                        | <span data-ttu-id="afa02-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="afa02-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="afa02-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="afa02-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="afa02-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="afa02-112">Policy.Read.All</span></span> |
| <span data-ttu-id="afa02-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="afa02-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afa02-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afa02-114">Not supported.</span></span> |
| <span data-ttu-id="afa02-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="afa02-115">Application</span></span>                            | <span data-ttu-id="afa02-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="afa02-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="afa02-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="afa02-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/identitySecurityDefaultsEnforcementPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="afa02-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="afa02-118">Optional query parameters</span></span>

<span data-ttu-id="afa02-119">Этот метод поддерживает `select` параметр запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="afa02-119">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="afa02-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="afa02-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="afa02-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="afa02-121">Request headers</span></span>

| <span data-ttu-id="afa02-122">Имя</span><span class="sxs-lookup"><span data-stu-id="afa02-122">Name</span></span>      |<span data-ttu-id="afa02-123">Описание</span><span class="sxs-lookup"><span data-stu-id="afa02-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="afa02-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="afa02-124">Authorization</span></span> | <span data-ttu-id="afa02-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="afa02-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="afa02-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="afa02-127">Request body</span></span>

<span data-ttu-id="afa02-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="afa02-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afa02-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="afa02-129">Response</span></span>

<span data-ttu-id="afa02-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [идентитисекуритидефаултсенфорцементполици](../resources/identitysecuritydefaultsenforcementpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="afa02-130">If successful, this method returns a `200 OK` response code and the requested [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="afa02-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="afa02-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="afa02-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="afa02-132">Request</span></span>

<span data-ttu-id="afa02-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="afa02-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identitysecuritydefaultsenforcementpolicy"
}-->

```http
GET https://graph.microsoft.com/v1.0/policies/identitySecurityDefaultsEnforcementPolicy
```

### <a name="response"></a><span data-ttu-id="afa02-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="afa02-134">Response</span></span>

<span data-ttu-id="afa02-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="afa02-135">The following is an example of the response.</span></span>

> <span data-ttu-id="afa02-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="afa02-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identitySecurityDefaultsEnforcementPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/identitySecurityDefaultsEnforcementPolicy",
  "description": "Security defaults is a set of basic identity security mechanisms recommended by Microsoft. When enabled, these recommendations will be automatically enforced in your organization. Administrators and users will be better protected from common identity related attacks.",
  "displayName": "Security Defaults",
  "id": "00000000-0000-0000-0000-000000000005",
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get identitySecurityDefaultsEnforcementPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
