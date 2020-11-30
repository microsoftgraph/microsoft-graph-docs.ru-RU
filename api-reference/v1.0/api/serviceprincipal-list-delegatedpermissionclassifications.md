---
title: Список Делегатедпермиссионклассификатионс коллекции servicePrincipal
description: Получение списка классификаций, предоставленных делегированным разрешениям, предоставленным субъектом-службой API.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 0177f497599def33de1f56551657b972c7eeb430
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377321"
---
# <a name="list-delegatedpermissionclassifications-collection-of-serviceprincipal"></a><span data-ttu-id="f768e-103">Список Делегатедпермиссионклассификатионс коллекции servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="f768e-103">List delegatedPermissionClassifications collection of servicePrincipal</span></span>

<span data-ttu-id="f768e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f768e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f768e-105">Получение списка [делегатедпермиссионклассификатион](../resources/delegatedpermissionclassification.md) , настроенных в настоящее время для делегированных разрешений, предоставляемых API.</span><span class="sxs-lookup"><span data-stu-id="f768e-105">Retrieve the list of [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) currently configured for the delegated permissions exposed by an API.</span></span>

## <a name="permissions"></a><span data-ttu-id="f768e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f768e-106">Permissions</span></span>

<span data-ttu-id="f768e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f768e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f768e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f768e-109">Permission type</span></span>      | <span data-ttu-id="f768e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f768e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f768e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f768e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f768e-112">Application. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="f768e-112">Application.Read.All, Directory.Read.All</span></span> |
|<span data-ttu-id="f768e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f768e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f768e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f768e-114">Not supported.</span></span>    |
|<span data-ttu-id="f768e-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="f768e-115">Application</span></span> | <span data-ttu-id="f768e-116">Application. Read. Овнедби, Application. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="f768e-116">Application.Read.OwnedBy, Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f768e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f768e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/delegatedPermissionClassifications
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f768e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f768e-118">Optional query parameters</span></span>

<span data-ttu-id="f768e-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f768e-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f768e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f768e-120">Request headers</span></span>

| <span data-ttu-id="f768e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f768e-121">Name</span></span>           | <span data-ttu-id="f768e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f768e-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="f768e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f768e-123">Authorization</span></span>  | <span data-ttu-id="f768e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f768e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f768e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f768e-126">Request body</span></span>

<span data-ttu-id="f768e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f768e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f768e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f768e-128">Response</span></span>

<span data-ttu-id="f768e-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [делегатедпермиссионклассификатион](../resources/delegatedpermissionclassification.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f768e-129">If successful, this method returns a `200 OK` response code and a collection of [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f768e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f768e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f768e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f768e-131">Request</span></span>

<span data-ttu-id="f768e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f768e-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_delegatedpermissionclassification"
}-->

```http
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/delegatedPermissionClassifications
```

### <a name="response"></a><span data-ttu-id="f768e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f768e-133">Response</span></span>

<span data-ttu-id="f768e-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f768e-134">The following is an example of the response.</span></span>

> <span data-ttu-id="f768e-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f768e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
