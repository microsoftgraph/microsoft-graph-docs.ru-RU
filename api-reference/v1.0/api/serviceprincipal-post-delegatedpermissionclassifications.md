---
title: Создание Делегатедпермиссионклассификатион
description: Классифицировать разрешение, добавив Делегатедпермиссионклассификатион к субъекту-службе API.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 22512ad7a61d528d22535156c1ac882b73950f72
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377320"
---
# <a name="create-delegatedpermissionclassification"></a><span data-ttu-id="c6ccc-103">Создание Делегатедпермиссионклассификатион</span><span class="sxs-lookup"><span data-stu-id="c6ccc-103">Create delegatedPermissionClassification</span></span>

<span data-ttu-id="c6ccc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6ccc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c6ccc-105">Классифицировать делегированное разрешение, добавив [делегатедпермиссионклассификатион](../resources/delegatedpermissionclassification.md) к [servicePrincipal](../resources/servicePrincipal.md) , представляющему API.</span><span class="sxs-lookup"><span data-stu-id="c6ccc-105">Classify a delegated permission by adding a [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) to the [servicePrincipal](../resources/servicePrincipal.md) representing the API.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6ccc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6ccc-106">Permissions</span></span>

<span data-ttu-id="c6ccc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6ccc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6ccc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6ccc-109">Permission type</span></span>      | <span data-ttu-id="c6ccc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6ccc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6ccc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6ccc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c6ccc-112">Пермиссионгрантполици. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c6ccc-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
|<span data-ttu-id="c6ccc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6ccc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6ccc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6ccc-114">Not supported.</span></span>    |
|<span data-ttu-id="c6ccc-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="c6ccc-115">Application</span></span> | <span data-ttu-id="c6ccc-116">Пермиссионгрантполици. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c6ccc-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6ccc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6ccc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/delegatedPermissionClassifications
```

## <a name="request-headers"></a><span data-ttu-id="c6ccc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6ccc-118">Request headers</span></span>

| <span data-ttu-id="c6ccc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c6ccc-119">Name</span></span>       | <span data-ttu-id="c6ccc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c6ccc-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="c6ccc-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c6ccc-121">Authorization</span></span> | <span data-ttu-id="c6ccc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6ccc-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c6ccc-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c6ccc-124">Content-type</span></span> | <span data-ttu-id="c6ccc-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6ccc-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6ccc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c6ccc-127">Request body</span></span>

<span data-ttu-id="c6ccc-128">В тексте запроса добавьте представление объекта [делегатедпермиссионклассификатион](../resources/delegatedpermissionclassification.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c6ccc-128">In the request body, supply a JSON representation of an [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c6ccc-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6ccc-129">Response</span></span>

<span data-ttu-id="c6ccc-130">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [делегатедпермиссионклассификатион](../resources/delegatedpermissionclassification.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c6ccc-130">If successful, this method returns a `201 Created` response code and an [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c6ccc-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="c6ccc-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c6ccc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6ccc-132">Request</span></span>

<span data-ttu-id="c6ccc-133">В следующем примере делегированное разрешение User. Read "классифицируется как" низкие ".</span><span class="sxs-lookup"><span data-stu-id="c6ccc-133">In the following example, the delegated permission "User.Read" is being classified "low".</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_create_delegatedpermissionclassification"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/delegatedPermissionClassifications
Content-Type: application/json

{
  "permissionId": "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
  "permissionName": "User.Read",
  "classification": "low"
}
```

### <a name="response"></a><span data-ttu-id="c6ccc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6ccc-134">Response</span></span>

<span data-ttu-id="c6ccc-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c6ccc-135">The following is an example of the response.</span></span>

> <span data-ttu-id="c6ccc-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c6ccc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.delegatedPermissionClassification"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "2G3-4TG6YU2J54hjnaRoPQE",
  "permissionId": "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
  "permissionName": "User.Read",
  "classification": "low"
}
```
