---
title: Список Делегатедпермиссионклассификатионс коллекции servicePrincipal
description: Получение списка классификаций, предоставленных делегированным разрешениям, предоставленным субъектом-службой API.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: cb2b347917642eeed7a4ca07ecd4b1984514ae16
ms.sourcegitcommit: 775b38baac6a4e7704d6144ef4589f2fc476bd61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/13/2020
ms.locfileid: "48433619"
---
# <a name="list-delegatedpermissionclassifications-collection-of-serviceprincipal"></a><span data-ttu-id="76157-103">Список Делегатедпермиссионклассификатионс коллекции servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="76157-103">List delegatedPermissionClassifications collection of servicePrincipal</span></span>

<span data-ttu-id="76157-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76157-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76157-105">Получение списка [делегатедпермиссионклассификатион](../resources/delegatedpermissionclassification.md) , настроенных в настоящее время для делегированных разрешений, предоставляемых API.</span><span class="sxs-lookup"><span data-stu-id="76157-105">Retrieve the list of [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) currently configured for the delegated permissions exposed by an API.</span></span>

## <a name="permissions"></a><span data-ttu-id="76157-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="76157-106">Permissions</span></span>

<span data-ttu-id="76157-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76157-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76157-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76157-109">Permission type</span></span>      | <span data-ttu-id="76157-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="76157-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76157-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76157-111">Delegated (work or school account)</span></span> | <span data-ttu-id="76157-112">Application. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="76157-112">Application.Read.All, Directory.Read.All</span></span> |
|<span data-ttu-id="76157-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76157-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76157-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76157-114">Not supported.</span></span>    |
|<span data-ttu-id="76157-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="76157-115">Application</span></span> | <span data-ttu-id="76157-116">Application. Read. Овнедби, Application. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="76157-116">Application.Read.OwnedBy, Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="76157-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76157-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/delegatedPermissionClassifications
```

## <a name="optional-query-parameters"></a><span data-ttu-id="76157-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="76157-118">Optional query parameters</span></span>

<span data-ttu-id="76157-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="76157-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="76157-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="76157-120">Request headers</span></span>

| <span data-ttu-id="76157-121">Имя</span><span class="sxs-lookup"><span data-stu-id="76157-121">Name</span></span>           | <span data-ttu-id="76157-122">Описание</span><span class="sxs-lookup"><span data-stu-id="76157-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="76157-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="76157-123">Authorization</span></span>  | <span data-ttu-id="76157-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76157-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="76157-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="76157-126">Request body</span></span>

<span data-ttu-id="76157-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="76157-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76157-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="76157-128">Response</span></span>

<span data-ttu-id="76157-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [делегатедпермиссионклассификатион](../resources/delegatedpermissionclassification.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="76157-129">If successful, this method returns a `200 OK` response code and a collection of [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76157-130">Пример</span><span class="sxs-lookup"><span data-stu-id="76157-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="76157-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="76157-131">Request</span></span>

<span data-ttu-id="76157-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76157-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_delegatedpermissionclassification"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/delegatedPermissionClassifications
```

### <a name="response"></a><span data-ttu-id="76157-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="76157-133">Response</span></span>

<span data-ttu-id="76157-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="76157-134">The following is an example of the response.</span></span>

> <span data-ttu-id="76157-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="76157-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.delegatedPermissionClassification",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
        "id": "2G3-4TG6YU2J54hjnaRoPQE",
        "permissionId": "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
        "permissionName": "User.Read",
        "classification": "low"
    }
  ]
}
```
