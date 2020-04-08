---
title: Добавление участника роли каталога
description: С помощью этого API можно создать участника роли каталога.
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 53474c5a1791be3213091150b04fea5e1d9aff2f
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43180867"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="c077a-103">Добавление участника роли каталога</span><span class="sxs-lookup"><span data-stu-id="c077a-103">Add directory role member</span></span>

<span data-ttu-id="c077a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c077a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c077a-105">С помощью этого API можно создать участника роли каталога.</span><span class="sxs-lookup"><span data-stu-id="c077a-105">Use this API to create a new directory role member.</span></span>
## <a name="permissions"></a><span data-ttu-id="c077a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c077a-106">Permissions</span></span>
<span data-ttu-id="c077a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c077a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c077a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c077a-109">Permission type</span></span>      | <span data-ttu-id="c077a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c077a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c077a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c077a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c077a-112">Ролеманажемент. ReadWrite. Directory, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="c077a-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c077a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c077a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c077a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c077a-114">Not supported.</span></span>    |
|<span data-ttu-id="c077a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c077a-115">Application</span></span> | <span data-ttu-id="c077a-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="c077a-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="c077a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c077a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="c077a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c077a-118">Request headers</span></span>
| <span data-ttu-id="c077a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c077a-119">Name</span></span>       | <span data-ttu-id="c077a-120">Тип</span><span class="sxs-lookup"><span data-stu-id="c077a-120">Type</span></span> | <span data-ttu-id="c077a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c077a-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c077a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c077a-122">Authorization</span></span>  | <span data-ttu-id="c077a-123">string</span><span class="sxs-lookup"><span data-stu-id="c077a-123">string</span></span>  | <span data-ttu-id="c077a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c077a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c077a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c077a-126">Request body</span></span>
<span data-ttu-id="c077a-127">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c077a-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c077a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c077a-128">Response</span></span>

<span data-ttu-id="c077a-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c077a-129">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c077a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c077a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c077a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c077a-131">Request</span></span>
<span data-ttu-id="c077a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c077a-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c077a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c077a-133">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="c077a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c077a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="c077a-135">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c077a-135">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c077a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c077a-136">Response</span></span>
<span data-ttu-id="c077a-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c077a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
