---
title: Удаление Цертификатебаседаусконфигуратион
description: Удаление Цертификатебаседаусконфигуратион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2c9fc5a1bcc524551fd83efe54ab5dabf9bfc943
ms.sourcegitcommit: 23aa2941cfb8bd744d8d59e8bba9d2c5f57f8e29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/29/2019
ms.locfileid: "36667668"
---
# <a name="delete-certificatebasedauthconfiguration"></a><span data-ttu-id="1a637-103">Удаление Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="1a637-103">Delete certificateBasedAuthConfiguration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a637-104">Удаление объекта [цертификатебаседаусконфигуратион](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1a637-104">Delete a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a637-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1a637-105">Permissions</span></span>

<span data-ttu-id="1a637-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a637-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1a637-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a637-108">Permission type</span></span>                        | <span data-ttu-id="1a637-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a637-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1a637-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a637-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a637-111">Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1a637-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="1a637-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a637-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a637-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a637-113">Not supported.</span></span> |
| <span data-ttu-id="1a637-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a637-114">Application</span></span>    | <span data-ttu-id="1a637-115">Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1a637-115">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a637-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a637-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1a637-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a637-117">Request headers</span></span>

| <span data-ttu-id="1a637-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1a637-118">Name</span></span>          | <span data-ttu-id="1a637-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1a637-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1a637-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a637-120">Authorization</span></span> | <span data-ttu-id="1a637-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="1a637-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a637-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1a637-122">Request body</span></span>

<span data-ttu-id="1a637-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1a637-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a637-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="1a637-124">Response</span></span>

<span data-ttu-id="1a637-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1a637-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1a637-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="1a637-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1a637-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a637-128">Request</span></span>

<span data-ttu-id="1a637-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a637-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_certificatebasedauthconfiguration"
}-->

```http
DELETE https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration/{id}
```

### <a name="response"></a><span data-ttu-id="1a637-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a637-130">Response</span></span>

<span data-ttu-id="1a637-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1a637-131">The following is an example of the response.</span></span>

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
