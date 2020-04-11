---
title: Удаление типа ресурса tokenLifetimePolicy
description: Удаление Токенлифетимеполици из приложения.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ec2b4ba053aff07167dec663eebbabe3f509eb54
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229225"
---
# <a name="remove-tokenlifetimepolicy"></a><span data-ttu-id="5a1e7-103">Удаление типа ресурса tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="5a1e7-103">Remove tokenLifetimePolicy</span></span>

<span data-ttu-id="5a1e7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a1e7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5a1e7-105">Удаление [токенлифетимеполици](../resources/tokenlifetimepolicy.md) из [приложения](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="5a1e7-105">Remove a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5a1e7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5a1e7-106">Permissions</span></span>

<span data-ttu-id="5a1e7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a1e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5a1e7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a1e7-109">Permission type</span></span>                        | <span data-ttu-id="5a1e7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a1e7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5a1e7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a1e7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5a1e7-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5a1e7-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="5a1e7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a1e7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a1e7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a1e7-114">Not supported.</span></span> |
| <span data-ttu-id="5a1e7-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="5a1e7-115">Application</span></span>                            | <span data-ttu-id="5a1e7-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5a1e7-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a1e7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a1e7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenLifetimePolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="5a1e7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a1e7-118">Request headers</span></span>

| <span data-ttu-id="5a1e7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5a1e7-119">Name</span></span>          | <span data-ttu-id="5a1e7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5a1e7-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5a1e7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a1e7-121">Authorization</span></span> | <span data-ttu-id="5a1e7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a1e7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a1e7-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5a1e7-124">Request body</span></span>

<span data-ttu-id="5a1e7-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5a1e7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a1e7-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a1e7-126">Response</span></span>

<span data-ttu-id="5a1e7-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5a1e7-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5a1e7-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="5a1e7-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5a1e7-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a1e7-129">Request</span></span>

<span data-ttu-id="5a1e7-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a1e7-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_tokenlifetimepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}/tokenLifetimePolicies/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="5a1e7-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a1e7-131">Response</span></span>

<span data-ttu-id="5a1e7-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5a1e7-132">The following is an example of the response.</span></span>

> <span data-ttu-id="5a1e7-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a1e7-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
