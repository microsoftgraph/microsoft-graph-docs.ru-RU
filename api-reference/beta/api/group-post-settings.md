---
title: Создание параметра каталога для групп
description: Используйте этот API, чтобы создать новый параметр каталога для группы.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 7663917e2433862dd4eddfb385214e71f42d1375
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592524"
---
# <a name="create-a-directory-setting-on-groups"></a><span data-ttu-id="391b8-103">Создание параметра каталога для групп</span><span class="sxs-lookup"><span data-stu-id="391b8-103">Create a directory setting on groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="391b8-104">Используйте этот API, чтобы создать новый параметр каталога для группы.</span><span class="sxs-lookup"><span data-stu-id="391b8-104">Use this API to create a new directory setting for the group.</span></span>
## <a name="permissions"></a><span data-ttu-id="391b8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="391b8-105">Permissions</span></span>
<span data-ttu-id="391b8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="391b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="391b8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="391b8-108">Permission type</span></span>      | <span data-ttu-id="391b8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="391b8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="391b8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="391b8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="391b8-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="391b8-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="391b8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="391b8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="391b8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="391b8-113">Not supported.</span></span>    |
|<span data-ttu-id="391b8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="391b8-114">Application</span></span> | <span data-ttu-id="391b8-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="391b8-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="391b8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="391b8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="391b8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="391b8-117">Request headers</span></span>
| <span data-ttu-id="391b8-118">Имя</span><span class="sxs-lookup"><span data-stu-id="391b8-118">Name</span></span>       | <span data-ttu-id="391b8-119">Описание</span><span class="sxs-lookup"><span data-stu-id="391b8-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="391b8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="391b8-120">Authorization</span></span>  | <span data-ttu-id="391b8-121">Bearer <token>.</span><span class="sxs-lookup"><span data-stu-id="391b8-121">Bearer <token>.</span></span> <span data-ttu-id="391b8-122">Обязательный</span><span class="sxs-lookup"><span data-stu-id="391b8-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="391b8-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="391b8-123">Request body</span></span>
<span data-ttu-id="391b8-124">В тексте запроса добавьте представление объекта [Директорисеттинг](../resources/directorysetting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="391b8-124">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="391b8-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="391b8-125">Response</span></span>

<span data-ttu-id="391b8-126">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [директорисеттинг](../resources/directorysetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="391b8-126">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="391b8-127">Пример</span><span class="sxs-lookup"><span data-stu-id="391b8-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="391b8-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="391b8-128">Request</span></span>
<span data-ttu-id="391b8-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="391b8-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="391b8-130">В тексте запроса добавьте представление объекта [Директорисеттинг](../resources/directorysetting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="391b8-130">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="391b8-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="391b8-131">Response</span></span>
<span data-ttu-id="391b8-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="391b8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="391b8-135">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="391b8-135">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="391b8-136">Язык</span><span class="sxs-lookup"><span data-stu-id="391b8-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directorysetting_from_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/group-post-settings.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
