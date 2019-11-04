---
title: Создание Персонанниверсари
description: Используйте этот API для создания нового Персонанниверсари.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: e6e73919913f710bee6721ec1710847cc742ba4d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937723"
---
# <a name="create-personanniversary"></a><span data-ttu-id="e6d76-103">Создание Персонанниверсари</span><span class="sxs-lookup"><span data-stu-id="e6d76-103">Create personAnniversary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6d76-104">Используйте этот API, чтобы создать новый объект [персонанниверсари](../resources/personanniversary.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="e6d76-104">Use this API to create a new [personAnniversary](../resources/personanniversary.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e6d76-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e6d76-105">Permissions</span></span>

<span data-ttu-id="e6d76-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6d76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e6d76-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6d76-108">Permission type</span></span>                        | <span data-ttu-id="e6d76-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6d76-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e6d76-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6d76-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e6d76-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e6d76-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e6d76-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6d76-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6d76-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e6d76-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e6d76-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6d76-114">Application</span></span>                            | <span data-ttu-id="e6d76-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6d76-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="e6d76-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6d76-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/anniversaries 
```

## <a name="request-headers"></a><span data-ttu-id="e6d76-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6d76-117">Request headers</span></span>

| <span data-ttu-id="e6d76-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e6d76-118">Name</span></span>      |<span data-ttu-id="e6d76-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e6d76-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e6d76-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6d76-120">Authorization</span></span>  | <span data-ttu-id="e6d76-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6d76-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="e6d76-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e6d76-123">Content-Type</span></span>   | <span data-ttu-id="e6d76-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6d76-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6d76-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e6d76-126">Request body</span></span>

<span data-ttu-id="e6d76-127">В тексте запроса добавьте представление объекта [персонанниверсари](../resources/personanniversary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6d76-127">In the request body, supply a JSON representation of [personAnniversary](../resources/personanniversary.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e6d76-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6d76-128">Response</span></span>

<span data-ttu-id="e6d76-129">В случае успешного выполнения этот метод `201, Created` возвращает код отклика и новый объект [персонанниверсари](../resources/personanniversary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e6d76-129">If successful, this method returns `201, Created` response code and a new [personAnniversary](../resources/personanniversary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e6d76-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="e6d76-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e6d76-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6d76-131">Request</span></span>

<span data-ttu-id="e6d76-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6d76-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_personanniversary_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/anniversaries
Content-type: application/json

{
  "type": "type-value",
  "date": "datetime-value"
}
```

### <a name="response"></a><span data-ttu-id="e6d76-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6d76-133">Response</span></span>

<span data-ttu-id="e6d76-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e6d76-134">The following is an example of the response.</span></span>

> <span data-ttu-id="e6d76-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e6d76-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAnniversary"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "type": "type-value",
  "date": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create personAnniversary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->