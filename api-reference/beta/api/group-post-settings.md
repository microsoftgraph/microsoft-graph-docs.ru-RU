---
title: Создание параметра каталога для групп
description: Используйте этот API, чтобы создать новый параметр каталога для группы.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 8f4d7e70311d40b762bf5fc683ff9fd4c509ba82
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42418717"
---
# <a name="create-a-directory-setting-on-groups"></a><span data-ttu-id="9edfd-103">Создание параметра каталога для групп</span><span class="sxs-lookup"><span data-stu-id="9edfd-103">Create a directory setting on groups</span></span>

<span data-ttu-id="9edfd-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9edfd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9edfd-105">Используйте этот API, чтобы создать новый параметр каталога для группы.</span><span class="sxs-lookup"><span data-stu-id="9edfd-105">Use this API to create a new directory setting for the group.</span></span>
## <a name="permissions"></a><span data-ttu-id="9edfd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9edfd-106">Permissions</span></span>
<span data-ttu-id="9edfd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9edfd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9edfd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9edfd-109">Permission type</span></span>      | <span data-ttu-id="9edfd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9edfd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9edfd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9edfd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9edfd-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9edfd-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9edfd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9edfd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9edfd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9edfd-114">Not supported.</span></span>    |
|<span data-ttu-id="9edfd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9edfd-115">Application</span></span> | <span data-ttu-id="9edfd-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9edfd-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9edfd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9edfd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="9edfd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9edfd-118">Request headers</span></span>
| <span data-ttu-id="9edfd-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9edfd-119">Name</span></span>       | <span data-ttu-id="9edfd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9edfd-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9edfd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9edfd-121">Authorization</span></span>  | <span data-ttu-id="9edfd-122">Bearer <token>.</span><span class="sxs-lookup"><span data-stu-id="9edfd-122">Bearer <token>.</span></span> <span data-ttu-id="9edfd-123">Обязательна</span><span class="sxs-lookup"><span data-stu-id="9edfd-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="9edfd-124">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="9edfd-124">Request body</span></span>
<span data-ttu-id="9edfd-125">В тексте запроса добавьте представление объекта [директорисеттинг](../resources/directorysetting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9edfd-125">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9edfd-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="9edfd-126">Response</span></span>

<span data-ttu-id="9edfd-127">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [директорисеттинг](../resources/directorysetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9edfd-127">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9edfd-128">Пример</span><span class="sxs-lookup"><span data-stu-id="9edfd-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9edfd-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="9edfd-129">Request</span></span>
<span data-ttu-id="9edfd-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9edfd-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9edfd-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="9edfd-131">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="9edfd-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9edfd-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directorysetting-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="9edfd-133">В тексте запроса добавьте представление объекта [директорисеттинг](../resources/directorysetting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9edfd-133">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9edfd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9edfd-134">Response</span></span>
<span data-ttu-id="9edfd-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9edfd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
