---
title: Удаление Усераккаунтинформатион
description: Удаление объекта Усераккаунтинформатион.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 1cd1130b89104f1154425e94443a45e375012a61
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451587"
---
# <a name="delete-useraccountinformation"></a><span data-ttu-id="06660-103">Удаление Усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="06660-103">Delete userAccountInformation</span></span>

<span data-ttu-id="06660-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="06660-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06660-105">Удаление объекта [усераккаунтинформатион](../resources/useraccountinformation.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="06660-105">Delete a [userAccountInformation](../resources/useraccountinformation.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="06660-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="06660-106">Permissions</span></span>

<span data-ttu-id="06660-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06660-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="06660-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06660-109">Permission type</span></span>                        | <span data-ttu-id="06660-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06660-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="06660-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06660-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="06660-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06660-112">Not supported.</span></span>                              |
| <span data-ttu-id="06660-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06660-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06660-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06660-114">Not supported.</span></span>                              |
| <span data-ttu-id="06660-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06660-115">Application</span></span>                            | <span data-ttu-id="06660-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06660-116">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="06660-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06660-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /user/profile/account{id}
```

## <a name="request-headers"></a><span data-ttu-id="06660-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06660-118">Request headers</span></span>

| <span data-ttu-id="06660-119">Имя</span><span class="sxs-lookup"><span data-stu-id="06660-119">Name</span></span>           |<span data-ttu-id="06660-120">Описание</span><span class="sxs-lookup"><span data-stu-id="06660-120">Description</span></span>                 |
|:---------------|:---------------------------|
| <span data-ttu-id="06660-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06660-121">Authorization</span></span>  | <span data-ttu-id="06660-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06660-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="06660-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06660-124">Request body</span></span>

<span data-ttu-id="06660-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="06660-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06660-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="06660-126">Response</span></span>

<span data-ttu-id="06660-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="06660-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="06660-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="06660-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="06660-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="06660-130">Request</span></span>

<span data-ttu-id="06660-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06660-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_useraccountinformation"
}-->

```http
DELETE https://graph.microsoft.com/beta/user/profile/account/{id}
```

### <a name="response"></a><span data-ttu-id="06660-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="06660-132">Response</span></span>

<span data-ttu-id="06660-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="06660-133">The following is an example of the response.</span></span>

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
  "description": "Delete userAccountInformation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
