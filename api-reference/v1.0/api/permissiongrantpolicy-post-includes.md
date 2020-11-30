---
title: Создание Пермиссионгранткондитионсет в коллекции включенных элементов Пермиссионгрантполици
description: Добавьте условия, при которых событие предоставления разрешений включается в политику предоставления разрешений.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 42778a7eaae409a9d8602a1c9faf1189de446f79
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377327"
---
# <a name="create-permissiongrantconditionset-in-includes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="8a60d-103">Создание Пермиссионгранткондитионсет в коллекции включенных элементов Пермиссионгрантполици</span><span class="sxs-lookup"><span data-stu-id="8a60d-103">Create permissionGrantConditionSet in includes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="8a60d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a60d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8a60d-105">Добавьте условия, при которых событие предоставления разрешений *включается* в политику предоставления разрешений.</span><span class="sxs-lookup"><span data-stu-id="8a60d-105">Add conditions under which a permission grant event is *included* in a permission grant policy.</span></span> <span data-ttu-id="8a60d-106">Это можно сделать, добавив [пермиссионгранткондитионсет](../resources/permissiongrantconditionset.md) в коллекцию **includes** объекта  [пермиссионгрантполици](../resources/permissionGrantPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8a60d-106">You do this by adding a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) to the **includes** collection of a  [permissionGrantPolicy](../resources/permissionGrantPolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8a60d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8a60d-107">Permissions</span></span>

<span data-ttu-id="8a60d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a60d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a60d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a60d-110">Permission type</span></span>      | <span data-ttu-id="8a60d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a60d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a60d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a60d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8a60d-113">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="8a60d-113">Policy.ReadWrite.PermissionGrant</span></span> |
|<span data-ttu-id="8a60d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a60d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a60d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a60d-115">Not supported.</span></span>    |
|<span data-ttu-id="8a60d-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="8a60d-116">Application</span></span> | <span data-ttu-id="8a60d-117">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="8a60d-117">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a60d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a60d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /policies/permissionGrantPolicies/{id}/includes
```

## <a name="request-headers"></a><span data-ttu-id="8a60d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a60d-119">Request headers</span></span>

| <span data-ttu-id="8a60d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8a60d-120">Name</span></span>       | <span data-ttu-id="8a60d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8a60d-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="8a60d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8a60d-122">Authorization</span></span> | <span data-ttu-id="8a60d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a60d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8a60d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8a60d-125">Content-type</span></span> | <span data-ttu-id="8a60d-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a60d-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a60d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8a60d-128">Request body</span></span>

<span data-ttu-id="8a60d-129">В тексте запроса добавьте представление объекта [пермиссионгранткондитионсет](../resources/permissiongrantconditionset.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a60d-129">In the request body, supply a JSON representation of an [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8a60d-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a60d-130">Response</span></span>

<span data-ttu-id="8a60d-131">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [пермиссионгранткондитионсет](../resources/permissiongrantconditionset.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8a60d-131">If successful, this method returns a `201 Created` response code and an [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8a60d-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="8a60d-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8a60d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a60d-133">Request</span></span>

<span data-ttu-id="8a60d-134">В этом примере *все* делегированные разрешения для клиентских приложений из проверенных издателей включены в политику предоставления разрешений.</span><span class="sxs-lookup"><span data-stu-id="8a60d-134">In this example, *all* delegated permissions for client apps from verified publishers are included in the permission grant policy.</span></span> <span data-ttu-id="8a60d-135">Так как все остальные условия из [пермиссионгранткондитионсет](../resources/permissiongrantconditionset.md) опущены, они будут принимать значения по умолчанию, которые в каждом случае являются самыми-инклюзивными.</span><span class="sxs-lookup"><span data-stu-id="8a60d-135">Because all the other conditions from the [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) were omitted, they will take their default values, which in each case is the most-inclusive.</span></span>

<!-- {
  "blockType": "request",
  "truncated": true,
  "name": "permissiongrantpolicy_create_includes"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/{id}/includes
Content-Type: application/json

{
  "permissionType": "delegated",
  "clientApplicationsFromVerifiedPublisherOnly": true
}
```

### <a name="response"></a><span data-ttu-id="8a60d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a60d-136">Response</span></span>

<span data-ttu-id="8a60d-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8a60d-137">The following is an example of the response.</span></span>

> <span data-ttu-id="8a60d-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8a60d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantConditionSet"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "75ffda85-9314-43bc-bf19-554a7d079e96",
  "permissionClassification": "all",
  "permissionType": "delegated",
  "resourceApplication": "any",
  "permissions": ["all"],
  "clientApplicationIds": ["all"],
  "clientApplicationTenantIds": ["all"],
  "clientApplicationPublisherIds": ["all"],
  "clientApplicationsFromVerifiedPublisherOnly": false
}
```
