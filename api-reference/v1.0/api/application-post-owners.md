---
title: Добавление владельца
description: Добавление владельца в приложение.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ba4c43e1638646987ba3afcf30610863b150329d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939686"
---
# <a name="add-owner"></a><span data-ttu-id="806d2-103">Добавление владельца</span><span class="sxs-lookup"><span data-stu-id="806d2-103">Add owner</span></span>

<span data-ttu-id="806d2-104">Добавление владельца в [приложение](../resources/application.md) путем публикации в коллекции Owners.</span><span class="sxs-lookup"><span data-stu-id="806d2-104">Add an owner to an [application](../resources/application.md) by posting to the owners collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="806d2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="806d2-105">Permissions</span></span>
<span data-ttu-id="806d2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="806d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="806d2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="806d2-108">Permission type</span></span>      | <span data-ttu-id="806d2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="806d2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="806d2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="806d2-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="806d2-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="806d2-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="806d2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="806d2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="806d2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="806d2-113">Not supported.</span></span>    |
|<span data-ttu-id="806d2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="806d2-114">Application</span></span> | <span data-ttu-id="806d2-115">Application. ReadWrite. Овнедби и Directory. Read. ALL, Application. ReadWrite. ALL и Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="806d2-115">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="806d2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="806d2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="806d2-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="806d2-117">Request headers</span></span>
| <span data-ttu-id="806d2-118">Имя</span><span class="sxs-lookup"><span data-stu-id="806d2-118">Name</span></span> | <span data-ttu-id="806d2-119">Описание</span><span class="sxs-lookup"><span data-stu-id="806d2-119">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="806d2-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="806d2-120">Authorization</span></span> | <span data-ttu-id="806d2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="806d2-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="806d2-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="806d2-123">Request body</span></span>
<span data-ttu-id="806d2-124">В тексте запроса укажите идентификатор объекта каталога, который необходимо назначить владельцем.</span><span class="sxs-lookup"><span data-stu-id="806d2-124">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="806d2-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="806d2-125">Response</span></span>

<span data-ttu-id="806d2-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="806d2-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="806d2-127">Пример</span><span class="sxs-lookup"><span data-stu-id="806d2-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="806d2-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="806d2-128">Request</span></span>
<span data-ttu-id="806d2-129">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="806d2-129">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_application"
}-->
```http
POST https://graph.microsoft.com/v1.0/applications/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}

```

### <a name="response"></a><span data-ttu-id="806d2-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="806d2-130">Response</span></span>

<span data-ttu-id="806d2-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="806d2-131">The following is an example of the response.</span></span>

><span data-ttu-id="806d2-132">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="806d2-132">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="806d2-133">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="806d2-133">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
