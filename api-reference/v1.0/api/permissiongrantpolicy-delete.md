---
title: Удаление Пермиссионгрантполици
description: Удаление объекта Пермиссионгрантполици.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 5c977da45c2e640e041dc37c8be2fb17c49a8424
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377407"
---
# <a name="delete-permissiongrantpolicy"></a><span data-ttu-id="efa01-103">Удаление Пермиссионгрантполици</span><span class="sxs-lookup"><span data-stu-id="efa01-103">Delete permissionGrantPolicy</span></span>

<span data-ttu-id="efa01-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efa01-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="efa01-105">Удаление объекта [пермиссионгрантполици](../resources/permissiongrantpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="efa01-105">Delete a [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="efa01-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="efa01-106">Permissions</span></span>

<span data-ttu-id="efa01-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efa01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="efa01-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="efa01-109">Permission type</span></span>                        | <span data-ttu-id="efa01-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="efa01-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="efa01-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="efa01-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="efa01-112">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="efa01-112">Policy.ReadWrite.PermissionGrant</span></span> |
| <span data-ttu-id="efa01-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="efa01-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efa01-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efa01-114">Not supported.</span></span> |
| <span data-ttu-id="efa01-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="efa01-115">Application</span></span>                            | <span data-ttu-id="efa01-116">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="efa01-116">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="efa01-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="efa01-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="efa01-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="efa01-118">Request headers</span></span>

| <span data-ttu-id="efa01-119">Имя</span><span class="sxs-lookup"><span data-stu-id="efa01-119">Name</span></span>           | <span data-ttu-id="efa01-120">Описание</span><span class="sxs-lookup"><span data-stu-id="efa01-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="efa01-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="efa01-121">Authorization</span></span>  | <span data-ttu-id="efa01-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="efa01-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="efa01-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="efa01-124">Request body</span></span>

<span data-ttu-id="efa01-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="efa01-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efa01-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="efa01-126">Response</span></span>

<span data-ttu-id="efa01-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="efa01-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="efa01-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="efa01-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="efa01-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="efa01-130">Request</span></span>

<span data-ttu-id="efa01-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="efa01-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_permissiongrantpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/my-custom-consent-policy
```

### <a name="response"></a><span data-ttu-id="efa01-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="efa01-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy"
} -->

```http
HTTP/1.1 204 No Content
```
