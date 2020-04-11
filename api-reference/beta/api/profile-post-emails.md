---
title: Создание Итемемаил
description: Создание нового Итемемаил.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: f65cdb5e63ba6bacf048e337b1689390caa0f347
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229341"
---
# <a name="create-itememail"></a><span data-ttu-id="b0275-103">Создание Итемемаил</span><span class="sxs-lookup"><span data-stu-id="b0275-103">Create itemEmail</span></span>

<span data-ttu-id="b0275-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0275-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0275-105">Создание нового [итемемаил](../resources/itememail.md).</span><span class="sxs-lookup"><span data-stu-id="b0275-105">Create a new [itemEmail](../resources/itememail.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b0275-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b0275-106">Permissions</span></span>

<span data-ttu-id="b0275-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0275-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b0275-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0275-109">Permission type</span></span>                        | <span data-ttu-id="b0275-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0275-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b0275-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0275-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b0275-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b0275-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="b0275-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0275-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0275-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b0275-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="b0275-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0275-115">Application</span></span>                            | <span data-ttu-id="b0275-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0275-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="b0275-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0275-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /user/profile/emails
```

## <a name="request-headers"></a><span data-ttu-id="b0275-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0275-118">Request headers</span></span>

| <span data-ttu-id="b0275-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b0275-119">Name</span></span>           |<span data-ttu-id="b0275-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b0275-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="b0275-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0275-121">Authorization</span></span>  | <span data-ttu-id="b0275-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0275-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="b0275-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b0275-124">Content-Type</span></span>   | <span data-ttu-id="b0275-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0275-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0275-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b0275-127">Request body</span></span>

<span data-ttu-id="b0275-128">В тексте запроса добавьте представление объекта [итемемаил](../resources/itememail.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0275-128">In the request body, supply a JSON representation of an [itemEmail](../resources/itememail.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b0275-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0275-129">Response</span></span>

<span data-ttu-id="b0275-130">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [итемемаил](../resources/itememail.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b0275-130">If successful, this method returns a `201 Created` response code and a new [itemEmail](../resources/itememail.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b0275-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="b0275-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b0275-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0275-132">Request</span></span>

<span data-ttu-id="b0275-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0275-133">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b0275-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0275-134">Response</span></span>

<span data-ttu-id="b0275-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b0275-135">The following is an example of the response.</span></span>

> <span data-ttu-id="b0275-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0275-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
