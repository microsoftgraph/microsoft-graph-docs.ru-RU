---
title: Создание ЛангуажепрофиЦиенци
description: Используйте этот API для создания нового ЛангуажепрофиЦиенци.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 27a45672f838e99f3de1d1c3d965e2226f19d18c
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937695"
---
# <a name="create-languageproficiency"></a><span data-ttu-id="1a338-103">Создание ЛангуажепрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="1a338-103">Create languageProficiency</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a338-104">Используйте этот API, чтобы создать новый объект [лангуажепрофиЦиенци](../resources/languageproficiency.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="1a338-104">Use this API to create a new [languageProficiency](../resources/languageproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1a338-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1a338-105">Permissions</span></span>

<span data-ttu-id="1a338-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a338-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1a338-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a338-108">Permission type</span></span>                        | <span data-ttu-id="1a338-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a338-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1a338-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a338-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a338-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1a338-111">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="1a338-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a338-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a338-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1a338-113">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="1a338-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a338-114">Application</span></span>                            | <span data-ttu-id="1a338-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a338-115">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a338-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a338-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/languages
```

## <a name="request-headers"></a><span data-ttu-id="1a338-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a338-117">Request headers</span></span>

| <span data-ttu-id="1a338-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1a338-118">Name</span></span>      |<span data-ttu-id="1a338-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1a338-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1a338-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a338-120">Authorization</span></span>  | <span data-ttu-id="1a338-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a338-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="1a338-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1a338-123">Content-Type</span></span>   | <span data-ttu-id="1a338-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a338-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a338-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1a338-126">Request body</span></span>

<span data-ttu-id="1a338-127">В тексте запроса добавьте представление объекта [лангуажепрофиЦиенци](../resources/languageproficiency.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a338-127">In the request body, supply a JSON representation of [languageProficiency](../resources/languageproficiency.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1a338-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a338-128">Response</span></span>

<span data-ttu-id="1a338-129">В случае успешного выполнения этот метод `201, Created` возвращает код отклика и новый объект [лангуажепрофиЦиенци](../resources/languageproficiency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1a338-129">If successful, this method returns `201, Created` response code and a new [languageProficiency](../resources/languageproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1a338-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="1a338-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1a338-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a338-131">Request</span></span>

<span data-ttu-id="1a338-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a338-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_languageproficiency_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/languages
Content-type: application/json

{
  "displayName": "displayName-value",
  "tag": "tag-value",
  "proficiency": "proficiency-value"
}
```

### <a name="response"></a><span data-ttu-id="1a338-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a338-133">Response</span></span>

<span data-ttu-id="1a338-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1a338-134">The following is an example of the response.</span></span>

> <span data-ttu-id="1a338-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1a338-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.languageProficiency"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "displayName": "displayName-value",
  "tag": "tag-value",
  "proficiency": "proficiency-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create languageProficiency",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->