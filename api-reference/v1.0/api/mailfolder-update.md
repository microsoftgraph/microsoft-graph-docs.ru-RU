---
title: Обновление объекта mailfolder
description: Обновление свойств объекта mailfolder.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: e2ce809c75a911b7d68ed80692a14a537c659d37
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871633"
---
# <a name="update-mailfolder"></a><span data-ttu-id="31dd6-103">Обновление объекта mailfolder</span><span class="sxs-lookup"><span data-stu-id="31dd6-103">Update mailfolder</span></span>

<span data-ttu-id="31dd6-104">Обновление свойств объекта mailfolder.</span><span class="sxs-lookup"><span data-stu-id="31dd6-104">Update the properties of mailfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="31dd6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="31dd6-105">Permissions</span></span>
<span data-ttu-id="31dd6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31dd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31dd6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31dd6-108">Permission type</span></span>      | <span data-ttu-id="31dd6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="31dd6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31dd6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31dd6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="31dd6-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="31dd6-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="31dd6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31dd6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31dd6-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="31dd6-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="31dd6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31dd6-114">Application</span></span> | <span data-ttu-id="31dd6-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="31dd6-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="31dd6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31dd6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="31dd6-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31dd6-117">Request headers</span></span>
| <span data-ttu-id="31dd6-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="31dd6-118">Header</span></span>       | <span data-ttu-id="31dd6-119">Значение</span><span class="sxs-lookup"><span data-stu-id="31dd6-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="31dd6-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="31dd6-120">Authorization</span></span>  | <span data-ttu-id="31dd6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31dd6-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="31dd6-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="31dd6-123">Content-Type</span></span>  | <span data-ttu-id="31dd6-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31dd6-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="31dd6-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="31dd6-126">Request body</span></span>
<span data-ttu-id="31dd6-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="31dd6-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="31dd6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="31dd6-130">Property</span></span>     | <span data-ttu-id="31dd6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="31dd6-131">Type</span></span>   |<span data-ttu-id="31dd6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="31dd6-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31dd6-133">displayName</span><span class="sxs-lookup"><span data-stu-id="31dd6-133">displayName</span></span>|<span data-ttu-id="31dd6-134">Строка</span><span class="sxs-lookup"><span data-stu-id="31dd6-134">String</span></span>|<span data-ttu-id="31dd6-135">Отображаемое имя объекта mailFolder.</span><span class="sxs-lookup"><span data-stu-id="31dd6-135">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="31dd6-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="31dd6-136">Response</span></span>

<span data-ttu-id="31dd6-137">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="31dd6-137">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="31dd6-138">Пример</span><span class="sxs-lookup"><span data-stu-id="31dd6-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="31dd6-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="31dd6-139">Request</span></span>
<span data-ttu-id="31dd6-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31dd6-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_mailfolder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailFolders/{id}
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```
##### <a name="response"></a><span data-ttu-id="31dd6-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="31dd6-141">Response</span></span>
<span data-ttu-id="31dd6-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="31dd6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update mailfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
