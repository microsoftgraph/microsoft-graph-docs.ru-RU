---
title: Удаление Каунтринамедлокатион
description: Удаление объекта Каунтринамедлокатион.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1d97d545fcd8411e0192321b1e461b81697ef858
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384774"
---
# <a name="delete-countrynamedlocation"></a><span data-ttu-id="23c13-103">Удаление Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="23c13-103">Delete countryNamedLocation</span></span>

<span data-ttu-id="23c13-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23c13-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="23c13-105">Удаление объекта [каунтринамедлокатион](../resources/countryNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="23c13-105">Delete a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="23c13-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23c13-106">Permissions</span></span>

<span data-ttu-id="23c13-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23c13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="23c13-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23c13-109">Permission type</span></span>                        | <span data-ttu-id="23c13-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23c13-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="23c13-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23c13-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="23c13-112">Policy. Read. ALL и Policy. ReadWrite. Кондитионалакцесс</span><span class="sxs-lookup"><span data-stu-id="23c13-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="23c13-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23c13-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23c13-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23c13-114">Not supported.</span></span> |
| <span data-ttu-id="23c13-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="23c13-115">Application</span></span>                            | <span data-ttu-id="23c13-116">Policy. Read. ALL и Policy. ReadWrite. Кондитионалакцесс</span><span class="sxs-lookup"><span data-stu-id="23c13-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="23c13-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23c13-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="23c13-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23c13-118">Request headers</span></span>

| <span data-ttu-id="23c13-119">Имя</span><span class="sxs-lookup"><span data-stu-id="23c13-119">Name</span></span>          | <span data-ttu-id="23c13-120">Описание</span><span class="sxs-lookup"><span data-stu-id="23c13-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="23c13-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23c13-121">Authorization</span></span> | <span data-ttu-id="23c13-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23c13-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23c13-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23c13-124">Request body</span></span>

<span data-ttu-id="23c13-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="23c13-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23c13-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="23c13-126">Response</span></span>

<span data-ttu-id="23c13-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="23c13-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="23c13-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="23c13-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="23c13-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="23c13-130">Request</span></span>

<span data-ttu-id="23c13-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23c13-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_countrynamedlocation"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
```

### <a name="response"></a><span data-ttu-id="23c13-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="23c13-132">Response</span></span>

<span data-ttu-id="23c13-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="23c13-133">The following is an example of the response.</span></span>

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
  "description": "Delete countryNamedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
