---
title: Создание параметра каталога для групп
description: Используйте этот API, чтобы создать новый параметр каталога для группы.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c04b08f4774a8aa24d2c7fcbd8c5645ef1d0e249
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681833"
---
# <a name="create-a-directory-setting-on-groups"></a><span data-ttu-id="2aea6-103">Создание параметра каталога для групп</span><span class="sxs-lookup"><span data-stu-id="2aea6-103">Create a directory setting on groups</span></span>

<span data-ttu-id="2aea6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2aea6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2aea6-105">Используйте этот API, чтобы создать новый параметр каталога для группы.</span><span class="sxs-lookup"><span data-stu-id="2aea6-105">Use this API to create a new directory setting for the group.</span></span>
## <a name="permissions"></a><span data-ttu-id="2aea6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2aea6-106">Permissions</span></span>
<span data-ttu-id="2aea6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2aea6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2aea6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2aea6-109">Permission type</span></span>      | <span data-ttu-id="2aea6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2aea6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2aea6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2aea6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2aea6-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2aea6-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2aea6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2aea6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2aea6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2aea6-114">Not supported.</span></span>    |
|<span data-ttu-id="2aea6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2aea6-115">Application</span></span> | <span data-ttu-id="2aea6-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2aea6-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2aea6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2aea6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="2aea6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2aea6-118">Request headers</span></span>
| <span data-ttu-id="2aea6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2aea6-119">Name</span></span>       | <span data-ttu-id="2aea6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2aea6-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2aea6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2aea6-121">Authorization</span></span>  | <span data-ttu-id="2aea6-122">Bearer <token>.</span><span class="sxs-lookup"><span data-stu-id="2aea6-122">Bearer <token>.</span></span> <span data-ttu-id="2aea6-123">Обязательное</span><span class="sxs-lookup"><span data-stu-id="2aea6-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="2aea6-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2aea6-124">Request body</span></span>
<span data-ttu-id="2aea6-125">В тексте запроса добавьте представление объекта [директорисеттинг](../resources/directorysetting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2aea6-125">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2aea6-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="2aea6-126">Response</span></span>

<span data-ttu-id="2aea6-127">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [директорисеттинг](../resources/directorysetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2aea6-127">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2aea6-128">Пример</span><span class="sxs-lookup"><span data-stu-id="2aea6-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2aea6-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="2aea6-129">Request</span></span>
<span data-ttu-id="2aea6-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2aea6-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2aea6-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="2aea6-131">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="2aea6-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2aea6-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directorysetting-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="2aea6-133">C#</span><span class="sxs-lookup"><span data-stu-id="2aea6-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directorysetting-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="2aea6-134">В тексте запроса добавьте представление объекта [директорисеттинг](../resources/directorysetting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2aea6-134">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2aea6-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2aea6-135">Response</span></span>
<span data-ttu-id="2aea6-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2aea6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
