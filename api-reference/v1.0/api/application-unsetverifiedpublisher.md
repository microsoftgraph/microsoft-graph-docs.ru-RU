---
title: 'Приложение: Унсетверифиедпублишер'
description: Удаление проверенного издателя приложения.
localization_priority: Normal
author: jesakowi
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ee598fc37ad3aa2abc8dac1a7980b29a53e41029
ms.sourcegitcommit: c28da0e5feea4791c19663a30b223a0a5da0ed02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/15/2020
ms.locfileid: "48471535"
---
# <a name="application-unsetverifiedpublisher"></a><span data-ttu-id="75c81-103">Приложение: Унсетверифиедпублишер</span><span class="sxs-lookup"><span data-stu-id="75c81-103">application: unsetVerifiedPublisher</span></span>

<span data-ttu-id="75c81-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75c81-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="75c81-105">Отмените настройку [верифиедпублишер](../resources/verifiedPublisher.md) , предварительно заданной для [приложения](../resources/application.md), удалив все проверенные свойства издателя.</span><span class="sxs-lookup"><span data-stu-id="75c81-105">Unset the [verifiedPublisher](../resources/verifiedPublisher.md) previously set on an [application](../resources/application.md), removing all verified publisher properties.</span></span> <span data-ttu-id="75c81-106">Для получения дополнительных сведений см [Проверка издателя](/azure/active-directory/develop/publisher-verification-overview).</span><span class="sxs-lookup"><span data-stu-id="75c81-106">For more information, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="75c81-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75c81-107">Permissions</span></span>

|<span data-ttu-id="75c81-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75c81-108">Permission type</span></span>      | <span data-ttu-id="75c81-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75c81-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75c81-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75c81-110">Delegated (work or school account)</span></span> | <span data-ttu-id="75c81-111">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75c81-111">Application.ReadWrite.All</span></span> |
|<span data-ttu-id="75c81-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75c81-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75c81-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="75c81-113">Not supported</span></span> |
|<span data-ttu-id="75c81-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="75c81-114">Application</span></span> | <span data-ttu-id="75c81-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="75c81-115">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="75c81-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75c81-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/unsetVerifiedPublisher
```

## <a name="request-headers"></a><span data-ttu-id="75c81-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75c81-117">Request headers</span></span>

| <span data-ttu-id="75c81-118">Имя</span><span class="sxs-lookup"><span data-stu-id="75c81-118">Name</span></span>           | <span data-ttu-id="75c81-119">Описание</span><span class="sxs-lookup"><span data-stu-id="75c81-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="75c81-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75c81-120">Authorization</span></span>  | <span data-ttu-id="75c81-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75c81-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="75c81-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75c81-123">Request body</span></span>

<span data-ttu-id="75c81-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75c81-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75c81-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="75c81-125">Response</span></span>

<span data-ttu-id="75c81-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="75c81-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="75c81-127">Пример</span><span class="sxs-lookup"><span data-stu-id="75c81-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="75c81-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="75c81-128">Request</span></span>

<span data-ttu-id="75c81-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75c81-129">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "application_unsetverifiedpublisher"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/unsetVerifiedPublisher
```

### <a name="response"></a><span data-ttu-id="75c81-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="75c81-130">Response</span></span>

<span data-ttu-id="75c81-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="75c81-131">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: db9f2d4d-e668-4eda-9d88-776b6ca6ca20
2020-09-09 21:29:08 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: unsetVerifiedPublisher",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->
