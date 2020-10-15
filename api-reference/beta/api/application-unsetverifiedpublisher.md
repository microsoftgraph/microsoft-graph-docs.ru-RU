---
title: 'Приложение: Унсетверифиедпублишер'
description: Отмените проверку издателя приложения.
localization_priority: Normal
author: jesakowi
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1f904a4b13e162dc503765b03d676319d3d0a510
ms.sourcegitcommit: c28da0e5feea4791c19663a30b223a0a5da0ed02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/15/2020
ms.locfileid: "48471573"
---
# <a name="application-unsetverifiedpublisher"></a><span data-ttu-id="b4f23-103">Приложение: Унсетверифиедпублишер</span><span class="sxs-lookup"><span data-stu-id="b4f23-103">application: unsetVerifiedPublisher</span></span>

<span data-ttu-id="b4f23-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4f23-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4f23-105">Отмените настройку [верифиедпублишер](../resources/verifiedPublisher.md) , предварительно заданной для [приложения](../resources/application.md), удалив все проверенные свойства издателя.</span><span class="sxs-lookup"><span data-stu-id="b4f23-105">Unset the the [verifiedPublisher](../resources/verifiedPublisher.md) previously set on an [application](../resources/application.md), removing all verified publisher properties.</span></span> <span data-ttu-id="b4f23-106">Для получения дополнительных сведений см [Проверка издателя](/azure/active-directory/develop/publisher-verification-overview).</span><span class="sxs-lookup"><span data-stu-id="b4f23-106">For more information, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="b4f23-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4f23-107">Permissions</span></span>

|<span data-ttu-id="b4f23-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4f23-108">Permission type</span></span>      | <span data-ttu-id="b4f23-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4f23-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4f23-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4f23-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b4f23-111">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4f23-111">Application.ReadWrite.All</span></span> |
|<span data-ttu-id="b4f23-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4f23-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4f23-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b4f23-113">Not supported</span></span> |
|<span data-ttu-id="b4f23-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="b4f23-114">Application</span></span> | <span data-ttu-id="b4f23-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b4f23-115">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4f23-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4f23-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/unsetVerifiedPublisher
```

## <a name="request-headers"></a><span data-ttu-id="b4f23-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4f23-117">Request headers</span></span>

| <span data-ttu-id="b4f23-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b4f23-118">Name</span></span>           | <span data-ttu-id="b4f23-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b4f23-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="b4f23-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4f23-120">Authorization</span></span>  | <span data-ttu-id="b4f23-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4f23-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b4f23-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4f23-123">Request body</span></span>

<span data-ttu-id="b4f23-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b4f23-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4f23-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4f23-125">Response</span></span>

<span data-ttu-id="b4f23-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b4f23-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b4f23-127">Пример</span><span class="sxs-lookup"><span data-stu-id="b4f23-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4f23-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4f23-128">Request</span></span>

<span data-ttu-id="b4f23-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4f23-129">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "application_unsetverifiedpublisher"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/unsetVerifiedPublisher
```

### <a name="response"></a><span data-ttu-id="b4f23-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4f23-130">Response</span></span>

<span data-ttu-id="b4f23-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b4f23-131">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: b0ed721f-7e6a-446c-89bc-2d03e1744dfe
2020-09-09 21:26:11 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: unsetVerifiedPublisher",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->
