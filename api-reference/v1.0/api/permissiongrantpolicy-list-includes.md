---
title: Список включает коллекцию Пермиссионгрантполици
description: Получение списка наборов условий, описывающих условия, при которых событие предоставления разрешений включается в политику предоставления разрешений.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: e85fdb159f275eb1dc4a7a31604b7d51e698288f
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377254"
---
# <a name="list-includes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="1b5be-103">Список включает коллекцию Пермиссионгрантполици</span><span class="sxs-lookup"><span data-stu-id="1b5be-103">List includes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="1b5be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b5be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1b5be-105">Получение наборов условий, *включенных* в [пермиссионгрантполици](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1b5be-105">Retrieve the condition sets which are *included* in a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1b5be-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b5be-106">Permissions</span></span>

<span data-ttu-id="1b5be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b5be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b5be-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b5be-109">Permission type</span></span>      | <span data-ttu-id="1b5be-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b5be-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b5be-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b5be-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1b5be-112">Policy. Read. Пермиссионгрант, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="1b5be-112">Policy.Read.PermissionGrant, Directory.Read.All</span></span> |
|<span data-ttu-id="1b5be-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b5be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b5be-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b5be-114">Not supported.</span></span>    |
|<span data-ttu-id="1b5be-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="1b5be-115">Application</span></span> | <span data-ttu-id="1b5be-116">Policy. Read. Пермиссионгрант, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="1b5be-116">Policy.Read.PermissionGrant, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b5be-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b5be-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /policies/permissionGrantPolicies/{id}/includes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1b5be-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1b5be-118">Optional query parameters</span></span>

<span data-ttu-id="1b5be-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1b5be-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b5be-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b5be-120">Request headers</span></span>

| <span data-ttu-id="1b5be-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1b5be-121">Name</span></span>           | <span data-ttu-id="1b5be-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1b5be-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="1b5be-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b5be-123">Authorization</span></span>  | <span data-ttu-id="1b5be-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b5be-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1b5be-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b5be-126">Request body</span></span>

<span data-ttu-id="1b5be-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1b5be-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b5be-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b5be-128">Response</span></span>

<span data-ttu-id="1b5be-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [пермиссионгранткондитионсет](../resources/permissiongrantconditionset.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1b5be-129">If successful, this method returns a `200 OK` response code and a collection of [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b5be-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1b5be-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b5be-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b5be-131">Request</span></span>

<span data-ttu-id="1b5be-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b5be-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_get_includes"
}-->

```http
GET https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/microsoft-application-admin/includes
```

### <a name="response"></a><span data-ttu-id="1b5be-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b5be-133">Response</span></span>

<span data-ttu-id="1b5be-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1b5be-134">The following is an example of the response.</span></span>

> <span data-ttu-id="1b5be-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1b5be-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantConditionSet",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "811d2da7-443c-43da-96e7-28d285b234e9",
      "permissionClassification": "all",
      "permissionType": "application",
      "resourceApplication": "any",
      "permissions": [ "all" ],
      "clientApplicationIds": [ "all" ],
      "clientApplicationTenantIds": [ "all" ],
      "clientApplicationPublisherIds": [ "all" ],
      "clientApplicationsFromVerifiedPublisherOnly": false
    },
    {
      "id": "60461179-740e-4d8b-9e00-1456a338c44b",
      "permissionClassification": "all",
      "permissionType": "delegated",
      "resourceApplication": "any",
      "permissions": [ "all" ],
      "clientApplicationIds": [ "all" ],
      "clientApplicationTenantIds": [ "all" ],
      "clientApplicationPublisherIds": [ "all" ],
      "clientApplicationsFromVerifiedPublisherOnly": false
    }
  ]
}
```
