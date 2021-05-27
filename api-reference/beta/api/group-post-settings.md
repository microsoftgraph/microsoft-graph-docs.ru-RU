---
title: Создание параметра каталога для групп
description: Используйте этот API для создания нового параметра каталога для группы.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b9a6b32b762306d716019d0c790104338bb5f3c0
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681363"
---
# <a name="create-a-directory-setting-on-groups"></a><span data-ttu-id="c28e8-103">Создание параметра каталога для групп</span><span class="sxs-lookup"><span data-stu-id="c28e8-103">Create a directory setting on groups</span></span>

<span data-ttu-id="c28e8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c28e8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c28e8-105">Используйте этот API для создания нового параметра каталога для группы.</span><span class="sxs-lookup"><span data-stu-id="c28e8-105">Use this API to create a new directory setting for the group.</span></span>
## <a name="permissions"></a><span data-ttu-id="c28e8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c28e8-106">Permissions</span></span>
<span data-ttu-id="c28e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c28e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c28e8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c28e8-109">Permission type</span></span>      | <span data-ttu-id="c28e8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c28e8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c28e8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c28e8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c28e8-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c28e8-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c28e8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c28e8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c28e8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c28e8-114">Not supported.</span></span>    |
|<span data-ttu-id="c28e8-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="c28e8-115">Application</span></span> | <span data-ttu-id="c28e8-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c28e8-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c28e8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c28e8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="c28e8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c28e8-118">Request headers</span></span>
| <span data-ttu-id="c28e8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c28e8-119">Name</span></span>       | <span data-ttu-id="c28e8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c28e8-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c28e8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c28e8-121">Authorization</span></span>  | <span data-ttu-id="c28e8-122">Bearer <token>.</span><span class="sxs-lookup"><span data-stu-id="c28e8-122">Bearer <token>.</span></span> <span data-ttu-id="c28e8-123">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c28e8-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="c28e8-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c28e8-124">Request body</span></span>
<span data-ttu-id="c28e8-125">В теле запроса поставляем представление JSON объекта [directorySetting.](../resources/directorysetting.md)</span><span class="sxs-lookup"><span data-stu-id="c28e8-125">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c28e8-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="c28e8-126">Response</span></span>

<span data-ttu-id="c28e8-127">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект directorySetting](../resources/directorysetting.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c28e8-127">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c28e8-128">Пример</span><span class="sxs-lookup"><span data-stu-id="c28e8-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c28e8-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="c28e8-129">Request</span></span>
<span data-ttu-id="c28e8-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c28e8-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c28e8-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="c28e8-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directorysetting_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/settings
Content-type: application/json
Content-length: 222

{
  "directorySetting": {
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="c28e8-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c28e8-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directorysetting-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="c28e8-133">C#</span><span class="sxs-lookup"><span data-stu-id="c28e8-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directorysetting-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="c28e8-134">В теле запроса поставляем представление JSON объекта [directorySetting.](../resources/directorysetting.md)</span><span class="sxs-lookup"><span data-stu-id="c28e8-134">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c28e8-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c28e8-135">Response</span></span>
<span data-ttu-id="c28e8-p103">Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c28e8-p103">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
  "directorySetting": {
    "id": "id-value",
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


