---
title: Удаление Цертификатебаседаусконфигуратион
description: Удаление Цертификатебаседаусконфигуратион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8bab6d42550e009897db42a2556e687059330000
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539241"
---
# <a name="delete-certificatebasedauthconfiguration"></a><span data-ttu-id="ff6de-103">Удаление Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="ff6de-103">Delete certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="ff6de-104">Удаление объекта [цертификатебаседаусконфигуратион](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ff6de-104">Delete a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff6de-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ff6de-105">Permissions</span></span>

<span data-ttu-id="ff6de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff6de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ff6de-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff6de-108">Permission type</span></span>                        | <span data-ttu-id="ff6de-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff6de-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ff6de-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff6de-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ff6de-111">Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ff6de-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="ff6de-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff6de-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff6de-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff6de-113">Not supported.</span></span> |
| <span data-ttu-id="ff6de-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="ff6de-114">Application</span></span>    | <span data-ttu-id="ff6de-115">Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ff6de-115">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff6de-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff6de-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ff6de-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff6de-117">Request headers</span></span>

| <span data-ttu-id="ff6de-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ff6de-118">Name</span></span>          | <span data-ttu-id="ff6de-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ff6de-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ff6de-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ff6de-120">Authorization</span></span> | <span data-ttu-id="ff6de-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff6de-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff6de-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ff6de-123">Request body</span></span>

<span data-ttu-id="ff6de-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ff6de-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff6de-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="ff6de-125">Response</span></span>

<span data-ttu-id="ff6de-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ff6de-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ff6de-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="ff6de-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ff6de-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff6de-129">Request</span></span>

<span data-ttu-id="ff6de-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff6de-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ff6de-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff6de-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_certificatebasedauthconfiguration"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration/{id}
```
---


### <a name="response"></a><span data-ttu-id="ff6de-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff6de-132">Response</span></span>

<span data-ttu-id="ff6de-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ff6de-133">The following is an example of the response.</span></span>

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
  "description": "Delete certificateBasedAuthConfiguration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
