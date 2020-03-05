---
title: Создание Итемемаил
description: Создание нового Итемемаил.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: c273e7c826d8222596521948c91f48d939657575
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455111"
---
# <a name="create-itememail"></a><span data-ttu-id="aef59-103">Создание Итемемаил</span><span class="sxs-lookup"><span data-stu-id="aef59-103">Create itemEmail</span></span>

<span data-ttu-id="aef59-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="aef59-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aef59-105">Создание нового [итемемаил](../resources/itememail.md).</span><span class="sxs-lookup"><span data-stu-id="aef59-105">Create a new [itemEmail](../resources/itememail.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="aef59-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aef59-106">Permissions</span></span>

<span data-ttu-id="aef59-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aef59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aef59-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aef59-109">Permission type</span></span>                        | <span data-ttu-id="aef59-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aef59-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="aef59-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aef59-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="aef59-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="aef59-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="aef59-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aef59-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aef59-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="aef59-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="aef59-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aef59-115">Application</span></span>                            | <span data-ttu-id="aef59-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aef59-116">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aef59-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aef59-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /user/profile/emails
```

## <a name="request-headers"></a><span data-ttu-id="aef59-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aef59-118">Request headers</span></span>

| <span data-ttu-id="aef59-119">Имя</span><span class="sxs-lookup"><span data-stu-id="aef59-119">Name</span></span>      |<span data-ttu-id="aef59-120">Описание</span><span class="sxs-lookup"><span data-stu-id="aef59-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aef59-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aef59-121">Authorization</span></span>  | <span data-ttu-id="aef59-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aef59-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="aef59-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aef59-124">Content-Type</span></span>   | <span data-ttu-id="aef59-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aef59-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aef59-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="aef59-127">Request body</span></span>

<span data-ttu-id="aef59-128">В тексте запроса добавьте представление объекта [итемемаил](../resources/itememail.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aef59-128">In the request body, supply a JSON representation of an [itemEmail](../resources/itememail.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="aef59-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="aef59-129">Response</span></span>

<span data-ttu-id="aef59-130">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [итемемаил](../resources/itememail.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aef59-130">If successful, this method returns a `201 Created` response code and a new [itemEmail](../resources/itememail.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aef59-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="aef59-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aef59-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="aef59-132">Request</span></span>

<span data-ttu-id="aef59-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aef59-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_itememail_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/user/profile/emails
Content-type: application/json

{
  "address": "address-value",
  "displayName": "displayName-value",
  "type": "type-value"
}
```

### <a name="response"></a><span data-ttu-id="aef59-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="aef59-134">Response</span></span>

<span data-ttu-id="aef59-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="aef59-135">The following is an example of the response.</span></span>

> <span data-ttu-id="aef59-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aef59-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemEmail"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "address": "address-value",
  "displayName": "displayName-value",
  "type": "type-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create itemEmail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
