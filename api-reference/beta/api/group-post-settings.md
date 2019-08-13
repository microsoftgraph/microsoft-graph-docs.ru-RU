---
title: Создание параметра каталога для групп
description: Используйте этот API, чтобы создать новый параметр каталога для группы.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d6879bdd6793cd29ee166c43a60beee275b865db
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323208"
---
# <a name="create-a-directory-setting-on-groups"></a><span data-ttu-id="d77ff-103">Создание параметра каталога для групп</span><span class="sxs-lookup"><span data-stu-id="d77ff-103">Create a directory setting on groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d77ff-104">Используйте этот API, чтобы создать новый параметр каталога для группы.</span><span class="sxs-lookup"><span data-stu-id="d77ff-104">Use this API to create a new directory setting for the group.</span></span>
## <a name="permissions"></a><span data-ttu-id="d77ff-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d77ff-105">Permissions</span></span>
<span data-ttu-id="d77ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d77ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d77ff-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d77ff-108">Permission type</span></span>      | <span data-ttu-id="d77ff-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d77ff-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d77ff-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d77ff-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d77ff-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d77ff-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d77ff-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d77ff-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d77ff-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d77ff-113">Not supported.</span></span>    |
|<span data-ttu-id="d77ff-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d77ff-114">Application</span></span> | <span data-ttu-id="d77ff-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d77ff-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d77ff-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d77ff-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="d77ff-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d77ff-117">Request headers</span></span>
| <span data-ttu-id="d77ff-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d77ff-118">Name</span></span>       | <span data-ttu-id="d77ff-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d77ff-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d77ff-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d77ff-120">Authorization</span></span>  | <span data-ttu-id="d77ff-121">Bearer <token>.</span><span class="sxs-lookup"><span data-stu-id="d77ff-121">Bearer <token>.</span></span> <span data-ttu-id="d77ff-122">Обязательный</span><span class="sxs-lookup"><span data-stu-id="d77ff-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="d77ff-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d77ff-123">Request body</span></span>
<span data-ttu-id="d77ff-124">В тексте запроса добавьте представление объекта [директорисеттинг](../resources/directorysetting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d77ff-124">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d77ff-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="d77ff-125">Response</span></span>

<span data-ttu-id="d77ff-126">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [директорисеттинг](../resources/directorysetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d77ff-126">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d77ff-127">Пример</span><span class="sxs-lookup"><span data-stu-id="d77ff-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d77ff-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="d77ff-128">Request</span></span>
<span data-ttu-id="d77ff-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d77ff-129">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d77ff-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="d77ff-130">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d77ff-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d77ff-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directorysetting-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="d77ff-132">В тексте запроса добавьте представление объекта [директорисеттинг](../resources/directorysetting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d77ff-132">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d77ff-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d77ff-133">Response</span></span>
<span data-ttu-id="d77ff-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d77ff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
