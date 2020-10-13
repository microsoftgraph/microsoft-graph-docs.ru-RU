---
title: Удаление Пермиссионгрантполици
description: Удаление объекта Пермиссионгрантполици.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 70e157a853d54a3f344fe36ab009b7ca69f8ec6a
ms.sourcegitcommit: 775b38baac6a4e7704d6144ef4589f2fc476bd61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/13/2020
ms.locfileid: "48433670"
---
# <a name="delete-permissiongrantpolicy"></a><span data-ttu-id="87aeb-103">Удаление Пермиссионгрантполици</span><span class="sxs-lookup"><span data-stu-id="87aeb-103">Delete permissionGrantPolicy</span></span>

<span data-ttu-id="87aeb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87aeb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87aeb-105">Удаление объекта [пермиссионгрантполици](../resources/permissiongrantpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="87aeb-105">Delete a [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="87aeb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="87aeb-106">Permissions</span></span>

<span data-ttu-id="87aeb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87aeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="87aeb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87aeb-109">Permission type</span></span>                        | <span data-ttu-id="87aeb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="87aeb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="87aeb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87aeb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="87aeb-112">Policy. ReadWrite. Пермиссионгрант</span><span class="sxs-lookup"><span data-stu-id="87aeb-112">Policy.ReadWrite.PermissionGrant</span></span> |
| <span data-ttu-id="87aeb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87aeb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87aeb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87aeb-114">Not supported.</span></span> |
| <span data-ttu-id="87aeb-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="87aeb-115">Application</span></span>                            | <span data-ttu-id="87aeb-116">Policy. ReadWrite. Пермиссионгрант</span><span class="sxs-lookup"><span data-stu-id="87aeb-116">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="87aeb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87aeb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="87aeb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="87aeb-118">Request headers</span></span>

| <span data-ttu-id="87aeb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="87aeb-119">Name</span></span>           | <span data-ttu-id="87aeb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="87aeb-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="87aeb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="87aeb-121">Authorization</span></span>  | <span data-ttu-id="87aeb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87aeb-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="87aeb-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="87aeb-124">Request body</span></span>

<span data-ttu-id="87aeb-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="87aeb-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87aeb-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="87aeb-126">Response</span></span>

<span data-ttu-id="87aeb-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="87aeb-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="87aeb-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="87aeb-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="87aeb-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="87aeb-130">Request</span></span>

<span data-ttu-id="87aeb-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87aeb-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_permissiongrantpolicy"
}-->

```msgraph-interactive
DELETE https://graph.microsoft.com/beta/policies/permissionGrantPolicies/my-custom-consent-policy
```

### <a name="response"></a><span data-ttu-id="87aeb-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="87aeb-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy"
} -->

```http
HTTP/1.1 204 No Content
```
