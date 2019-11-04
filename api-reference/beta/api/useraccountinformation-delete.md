---
title: Удаление Усераккаунтинформатион
description: Удаление объекта Усераккаунтинформатион.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 090df364dd86f2ab47b02259ff81acc36ad0aa6d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938150"
---
# <a name="delete-useraccountinformation"></a><span data-ttu-id="0d70c-103">Удаление Усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="0d70c-103">Delete userAccountInformation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d70c-104">Удаление объекта [усераккаунтинформатион](../resources/useraccountinformation.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="0d70c-104">Delete a [userAccountInformation](../resources/useraccountinformation.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0d70c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0d70c-105">Permissions</span></span>

<span data-ttu-id="0d70c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d70c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0d70c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d70c-108">Permission type</span></span>                        | <span data-ttu-id="0d70c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d70c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0d70c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d70c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0d70c-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d70c-111">Not supported.</span></span>                              |
| <span data-ttu-id="0d70c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d70c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d70c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d70c-113">Not supported.</span></span>                              |
| <span data-ttu-id="0d70c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d70c-114">Application</span></span>                            | <span data-ttu-id="0d70c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d70c-115">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="0d70c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d70c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /user/profile/account{id}
```

## <a name="request-headers"></a><span data-ttu-id="0d70c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d70c-117">Request headers</span></span>

| <span data-ttu-id="0d70c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0d70c-118">Name</span></span>           |<span data-ttu-id="0d70c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0d70c-119">Description</span></span>                 |
|:---------------|:---------------------------|
| <span data-ttu-id="0d70c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0d70c-120">Authorization</span></span>  | <span data-ttu-id="0d70c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d70c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0d70c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d70c-123">Request body</span></span>

<span data-ttu-id="0d70c-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0d70c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d70c-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d70c-125">Response</span></span>

<span data-ttu-id="0d70c-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0d70c-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0d70c-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="0d70c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0d70c-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d70c-129">Request</span></span>

<span data-ttu-id="0d70c-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d70c-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_useraccountinformation"
}-->

```http
DELETE https://graph.microsoft.com/beta/user/profile/account/{id}
```

### <a name="response"></a><span data-ttu-id="0d70c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d70c-131">Response</span></span>

<span data-ttu-id="0d70c-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0d70c-132">The following is an example of the response.</span></span>

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
