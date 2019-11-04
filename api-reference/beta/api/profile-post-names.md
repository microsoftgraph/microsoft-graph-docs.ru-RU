---
title: Создание personName
description: Используйте этот API, чтобы создать новый personName в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 6a2523d72909946eed95b455e50b3e1fb1a1c51f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937688"
---
# <a name="create-personname"></a><span data-ttu-id="8cf7c-103">Создание personName</span><span class="sxs-lookup"><span data-stu-id="8cf7c-103">Create personName</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cf7c-104">Используйте этот API, чтобы создать новый объект [PersonName](../resources/personname.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="8cf7c-104">Use this API to create a new [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8cf7c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8cf7c-105">Permissions</span></span>

<span data-ttu-id="8cf7c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cf7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8cf7c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8cf7c-108">Permission type</span></span>                        | <span data-ttu-id="8cf7c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8cf7c-109">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="8cf7c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8cf7c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8cf7c-111">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8cf7c-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="8cf7c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8cf7c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cf7c-113">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8cf7c-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="8cf7c-114">Application</span><span class="sxs-lookup"><span data-stu-id="8cf7c-114">Application</span></span>                            | <span data-ttu-id="8cf7c-115">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8cf7c-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8cf7c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8cf7c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/names
```

## <a name="request-headers"></a><span data-ttu-id="8cf7c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8cf7c-117">Request headers</span></span>

| <span data-ttu-id="8cf7c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8cf7c-118">Name</span></span>           |<span data-ttu-id="8cf7c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8cf7c-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="8cf7c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8cf7c-120">Authorization</span></span>  | <span data-ttu-id="8cf7c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8cf7c-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="8cf7c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8cf7c-123">Content-Type</span></span>   | <span data-ttu-id="8cf7c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8cf7c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8cf7c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8cf7c-126">Request body</span></span>

<span data-ttu-id="8cf7c-127">В тексте запроса добавьте представление объекта [PersonName](../resources/personname.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8cf7c-127">In the request body, supply a JSON representation of [personName](../resources/personname.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8cf7c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cf7c-128">Response</span></span>

<span data-ttu-id="8cf7c-129">В случае успешного выполнения этот метод `201, Created` возвращает код отклика и новый объект [PersonName](../resources/personname.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8cf7c-129">If successful, this method returns `201, Created` response code and a new [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8cf7c-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="8cf7c-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8cf7c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8cf7c-131">Request</span></span>

<span data-ttu-id="8cf7c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8cf7c-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_personname_from_profilev2"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/names
Content-type: application/json

{
  "displayName": "displayName-value",
  "first": "first-value",
  "initials": "initials-value",
  "last": "last-value",
  "languageTag": "languageTag-value",
  "maiden": "maiden-value"
}
```

### <a name="response"></a><span data-ttu-id="8cf7c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cf7c-133">Response</span></span>

<span data-ttu-id="8cf7c-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8cf7c-134">The following is an example of the response.</span></span>

> <span data-ttu-id="8cf7c-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8cf7c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "displayName": "displayName-value",
  "first": "first-value",
  "initials": "initials-value",
  "last": "last-value",
  "languageTag": "languageTag-value",
  "maiden": "maiden-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create personName",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->