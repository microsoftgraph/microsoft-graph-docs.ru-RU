---
title: Удаление Намедлокатион
description: Удаление объекта Намедлокатион.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a98506992157868b1d80059697a3e4c2ae76d606
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384830"
---
# <a name="delete-namedlocation"></a><span data-ttu-id="adab6-103">Удаление Намедлокатион</span><span class="sxs-lookup"><span data-stu-id="adab6-103">Delete namedLocation</span></span>

<span data-ttu-id="adab6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adab6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="adab6-105">Удаление объекта [намедлокатион](../resources/namedlocation.md) .</span><span class="sxs-lookup"><span data-stu-id="adab6-105">Delete a [namedLocation](../resources/namedlocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="adab6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="adab6-106">Permissions</span></span>

<span data-ttu-id="adab6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adab6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="adab6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="adab6-109">Permission type</span></span>                        | <span data-ttu-id="adab6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="adab6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="adab6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="adab6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="adab6-112">Policy. Read. ALL и Policy. ReadWrite. Кондитионалакцесс</span><span class="sxs-lookup"><span data-stu-id="adab6-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="adab6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="adab6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="adab6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adab6-114">Not supported.</span></span> |
| <span data-ttu-id="adab6-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="adab6-115">Application</span></span>                            | <span data-ttu-id="adab6-116">Policy. Read. ALL и Policy. ReadWrite. Кондитионалакцесс</span><span class="sxs-lookup"><span data-stu-id="adab6-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="adab6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="adab6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="adab6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="adab6-118">Request headers</span></span>

| <span data-ttu-id="adab6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="adab6-119">Name</span></span>          | <span data-ttu-id="adab6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="adab6-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="adab6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="adab6-121">Authorization</span></span> | <span data-ttu-id="adab6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="adab6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="adab6-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="adab6-124">Request body</span></span>

<span data-ttu-id="adab6-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="adab6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="adab6-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="adab6-126">Response</span></span>

<span data-ttu-id="adab6-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="adab6-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="adab6-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="adab6-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="adab6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="adab6-130">Request</span></span>

<span data-ttu-id="adab6-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="adab6-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_namedlocation"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
```

### <a name="response"></a><span data-ttu-id="adab6-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="adab6-132">Response</span></span>

<span data-ttu-id="adab6-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="adab6-133">The following is an example of the response.</span></span>

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
  "description": "Delete namedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
