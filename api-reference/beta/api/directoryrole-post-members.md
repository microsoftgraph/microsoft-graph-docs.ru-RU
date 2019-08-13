---
title: Добавление участника роли каталога
description: С помощью этого API можно создать участника роли каталога.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7ed3c3a9a46061c477aa47a777521c96ae539686
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324613"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="ed142-103">Добавление участника роли каталога</span><span class="sxs-lookup"><span data-stu-id="ed142-103">Add directory role member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed142-104">С помощью этого API можно создать участника роли каталога.</span><span class="sxs-lookup"><span data-stu-id="ed142-104">Use this API to create a new directory role member.</span></span>
## <a name="permissions"></a><span data-ttu-id="ed142-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ed142-105">Permissions</span></span>
<span data-ttu-id="ed142-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed142-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed142-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed142-108">Permission type</span></span>      | <span data-ttu-id="ed142-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed142-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed142-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed142-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ed142-111">Ролеманажемент. ReadWrite. Directory, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="ed142-111">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ed142-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed142-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed142-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed142-113">Not supported.</span></span>    |
|<span data-ttu-id="ed142-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed142-114">Application</span></span> | <span data-ttu-id="ed142-115">Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="ed142-115">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed142-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed142-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="ed142-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed142-117">Request headers</span></span>
| <span data-ttu-id="ed142-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ed142-118">Name</span></span>       | <span data-ttu-id="ed142-119">Тип</span><span class="sxs-lookup"><span data-stu-id="ed142-119">Type</span></span> | <span data-ttu-id="ed142-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ed142-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ed142-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed142-121">Authorization</span></span>  | <span data-ttu-id="ed142-122">string</span><span class="sxs-lookup"><span data-stu-id="ed142-122">string</span></span>  | <span data-ttu-id="ed142-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ed142-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed142-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ed142-125">Request body</span></span>
<span data-ttu-id="ed142-126">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed142-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ed142-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed142-127">Response</span></span>

<span data-ttu-id="ed142-128">В случае успеха этот метод возвращает код отклика `201 Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ed142-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed142-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ed142-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ed142-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed142-130">Request</span></span>
<span data-ttu-id="ed142-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed142-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ed142-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed142-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ed142-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed142-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="ed142-134">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed142-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ed142-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed142-135">Response</span></span>
<span data-ttu-id="ed142-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ed142-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
