---
title: Удаление Воркфорцеинтегратион
description: Удаление экземпляра объекта Воркфорцеинтегратион.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f44523533b40212a7735dc8ecbe70a7ec12666b4
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154061"
---
# <a name="delete-workforceintegration"></a><span data-ttu-id="eaac8-103">Удаление Воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="eaac8-103">Delete workforceIntegration</span></span>

<span data-ttu-id="eaac8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eaac8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eaac8-105">Удаление экземпляра объекта [воркфорцеинтегратион](../resources/workforceintegration.md).</span><span class="sxs-lookup"><span data-stu-id="eaac8-105">Delete an instance of a [workforceIntegration](../resources/workforceintegration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="eaac8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eaac8-106">Permissions</span></span>

<span data-ttu-id="eaac8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaac8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eaac8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eaac8-109">Permission type</span></span>                        | <span data-ttu-id="eaac8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eaac8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="eaac8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eaac8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="eaac8-112">Воркфорцеинтегратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="eaac8-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="eaac8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eaac8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eaac8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaac8-114">Not supported.</span></span> |
| <span data-ttu-id="eaac8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eaac8-115">Application</span></span>                            | <span data-ttu-id="eaac8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaac8-116">Not supported.</span></span> |

> <span data-ttu-id="eaac8-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="eaac8-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="eaac8-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="eaac8-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="eaac8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eaac8-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="request-headers"></a><span data-ttu-id="eaac8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eaac8-120">Request headers</span></span>

| <span data-ttu-id="eaac8-121">Имя</span><span class="sxs-lookup"><span data-stu-id="eaac8-121">Name</span></span>          | <span data-ttu-id="eaac8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="eaac8-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="eaac8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eaac8-123">Authorization</span></span> | <span data-ttu-id="eaac8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eaac8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eaac8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eaac8-126">Request body</span></span>

<span data-ttu-id="eaac8-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eaac8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eaac8-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="eaac8-128">Response</span></span>

<span data-ttu-id="eaac8-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="eaac8-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eaac8-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="eaac8-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eaac8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="eaac8-132">Request</span></span>

<span data-ttu-id="eaac8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eaac8-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_workforceintegration"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations/{workforceIntegrationId}
```

---


### <a name="response"></a><span data-ttu-id="eaac8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="eaac8-134">Response</span></span>

<span data-ttu-id="eaac8-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="eaac8-135">The following is an example of the response.</span></span>

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
  "description": "Delete workforceIntegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
