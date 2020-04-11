---
title: Создание Хомереалмдисковериполици
description: Создание нового Хомереалмдисковериполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 34347b52eead2688b39db55a775e843af807dd6c
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227892"
---
# <a name="create-homerealmdiscoverypolicy"></a><span data-ttu-id="b71d6-103">Создание Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="b71d6-103">Create homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="b71d6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b71d6-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="b71d6-105">Создание нового объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="b71d6-105">Create a new [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b71d6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b71d6-106">Permissions</span></span>

<span data-ttu-id="b71d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b71d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b71d6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b71d6-109">Permission type</span></span>                        | <span data-ttu-id="b71d6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b71d6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b71d6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b71d6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b71d6-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="b71d6-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="b71d6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b71d6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b71d6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b71d6-114">Not supported.</span></span> |
| <span data-ttu-id="b71d6-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="b71d6-115">Application</span></span>                            | <span data-ttu-id="b71d6-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="b71d6-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="b71d6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b71d6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/homeRealmDiscoveryPolicies
```

## <a name="request-headers"></a><span data-ttu-id="b71d6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b71d6-118">Request headers</span></span>

| <span data-ttu-id="b71d6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b71d6-119">Name</span></span>          | <span data-ttu-id="b71d6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b71d6-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b71d6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b71d6-121">Authorization</span></span> | <span data-ttu-id="b71d6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b71d6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b71d6-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b71d6-124">Content-type</span></span> | <span data-ttu-id="b71d6-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b71d6-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b71d6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b71d6-127">Request body</span></span>

<span data-ttu-id="b71d6-128">В тексте запроса добавьте представление объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b71d6-128">In the request body, supply a JSON representation of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b71d6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b71d6-129">Response</span></span>

<span data-ttu-id="b71d6-130">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b71d6-130">If successful, this method returns a `201 Created` response code and a new [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b71d6-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="b71d6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b71d6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b71d6-132">Request</span></span>

<span data-ttu-id="b71d6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b71d6-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_homerealmdiscoverypolicy_from_homerealmdiscoverypolicies"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```

### <a name="response"></a><span data-ttu-id="b71d6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b71d6-134">Response</span></span>

<span data-ttu-id="b71d6-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b71d6-135">The following is an example of the response.</span></span>

> <span data-ttu-id="b71d6-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b71d6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
