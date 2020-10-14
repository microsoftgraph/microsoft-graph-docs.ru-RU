---
title: Создание Делегатедпермиссионклассификатион
description: Классифицировать разрешение, добавив Делегатедпермиссионклассификатион к субъекту-службе API.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 47f4c1eb7a1098744a2760bf48c3b931beee96c0
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48461300"
---
# <a name="create-delegatedpermissionclassification"></a><span data-ttu-id="ed8c7-103">Создание Делегатедпермиссионклассификатион</span><span class="sxs-lookup"><span data-stu-id="ed8c7-103">Create delegatedPermissionClassification</span></span>

<span data-ttu-id="ed8c7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed8c7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed8c7-105">Классифицировать делегированное разрешение, добавив [делегатедпермиссионклассификатион](../resources/delegatedpermissionclassification.md) к [servicePrincipal](../resources/servicePrincipal.md) , представляющему API.</span><span class="sxs-lookup"><span data-stu-id="ed8c7-105">Classify a delegated permission by adding a [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) to the [servicePrincipal](../resources/servicePrincipal.md) representing the API.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed8c7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ed8c7-106">Permissions</span></span>

<span data-ttu-id="ed8c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed8c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed8c7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed8c7-109">Permission type</span></span>      | <span data-ttu-id="ed8c7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed8c7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed8c7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed8c7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ed8c7-112">Пермиссионгрантполици. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ed8c7-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
|<span data-ttu-id="ed8c7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed8c7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed8c7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed8c7-114">Not supported.</span></span>    |
|<span data-ttu-id="ed8c7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed8c7-115">Application</span></span> | <span data-ttu-id="ed8c7-116">Пермиссионгрантполици. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ed8c7-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed8c7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed8c7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/delegatedPermissionClassifications
```

## <a name="request-headers"></a><span data-ttu-id="ed8c7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed8c7-118">Request headers</span></span>

| <span data-ttu-id="ed8c7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ed8c7-119">Name</span></span>       | <span data-ttu-id="ed8c7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ed8c7-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="ed8c7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ed8c7-121">Authorization</span></span> | <span data-ttu-id="ed8c7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ed8c7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ed8c7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ed8c7-124">Content-type</span></span> | <span data-ttu-id="ed8c7-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ed8c7-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed8c7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ed8c7-127">Request body</span></span>

<span data-ttu-id="ed8c7-128">В тексте запроса добавьте представление объекта [делегатедпермиссионклассификатион](../resources/delegatedpermissionclassification.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed8c7-128">In the request body, supply a JSON representation of an [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ed8c7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed8c7-129">Response</span></span>

<span data-ttu-id="ed8c7-130">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [делегатедпермиссионклассификатион](../resources/delegatedpermissionclassification.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ed8c7-130">If successful, this method returns a `201 Created` response code and an [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ed8c7-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="ed8c7-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ed8c7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed8c7-132">Request</span></span>

<span data-ttu-id="ed8c7-133">В следующем примере делегированное разрешение User. Read "классифицируется как" низкие ".</span><span class="sxs-lookup"><span data-stu-id="ed8c7-133">In the following example, the delegated permission "User.Read" is being classified "low".</span></span>


# <a name="http"></a>[<span data-ttu-id="ed8c7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed8c7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_create_delegatedpermissionclassification"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/delegatedPermissionClassifications
Content-Type: application/json

{
  "permissionId": "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
  "permissionName": "User.Read",
  "classification": "low"
}
```
# <a name="javascript"></a>[<span data-ttu-id="ed8c7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed8c7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-create-delegatedpermissionclassification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ed8c7-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed8c7-136">Response</span></span>

<span data-ttu-id="ed8c7-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ed8c7-137">The following is an example of the response.</span></span>

> <span data-ttu-id="ed8c7-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ed8c7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
