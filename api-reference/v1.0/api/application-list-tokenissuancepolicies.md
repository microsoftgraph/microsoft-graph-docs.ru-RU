---
title: Список назначенных ТокениссуанцеполиЦиес
description: Список ТокениссуанцеполиЦиес, назначенных приложению.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3e116d5938ebc8575b4c4664156e6c7ab194b276
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227928"
---
# <a name="list-assigned-tokenissuancepolicies"></a><span data-ttu-id="df622-103">Список назначенных ТокениссуанцеполиЦиес</span><span class="sxs-lookup"><span data-stu-id="df622-103">List assigned tokenIssuancePolicies</span></span>

<span data-ttu-id="df622-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df622-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="df622-105">Перечисление объектов [токениссуанцеполици](../resources/tokenissuancepolicy.md) , назначенных [приложению](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="df622-105">List the [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) objects that are assigned to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="df622-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="df622-106">Permissions</span></span>

<span data-ttu-id="df622-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df622-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="df622-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df622-109">Permission type</span></span>                        | <span data-ttu-id="df622-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="df622-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="df622-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df622-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="df622-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="df622-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="df622-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df622-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df622-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df622-114">Not supported.</span></span> |
| <span data-ttu-id="df622-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="df622-115">Application</span></span>                            | <span data-ttu-id="df622-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="df622-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="df622-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df622-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/tokenIssuancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="df622-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="df622-118">Request headers</span></span>

| <span data-ttu-id="df622-119">Имя</span><span class="sxs-lookup"><span data-stu-id="df622-119">Name</span></span>          | <span data-ttu-id="df622-120">Описание</span><span class="sxs-lookup"><span data-stu-id="df622-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="df622-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="df622-121">Authorization</span></span> | <span data-ttu-id="df622-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df622-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df622-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="df622-124">Request body</span></span>

<span data-ttu-id="df622-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="df622-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df622-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="df622-126">Response</span></span>

<span data-ttu-id="df622-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [токениссуанцеполици](../resources/tokenissuancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="df622-127">If successful, this method returns a `200 OK` response code and a collection of [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="df622-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="df622-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="df622-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="df622-129">Request</span></span>

<span data-ttu-id="df622-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="df622-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_tokenissuancepolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/{id}/tokenIssuancePolicies
```

### <a name="response"></a><span data-ttu-id="df622-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="df622-131">Response</span></span>

<span data-ttu-id="df622-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="df622-132">The following is an example of the response.</span></span>

> <span data-ttu-id="df622-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="df622-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenIssuancePolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List assigned tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
