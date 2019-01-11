---
title: Обновление oAuth2PermissionGrant
description: Обновление свойства объекта oAuth2PermissionGrant.
localization_priority: Normal
ms.openlocfilehash: 3c01d62dfb7c0c6906ff860656ee87b5f6d40aed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822353"
---
# <a name="update-oauth2permissiongrant"></a><span data-ttu-id="6f88a-103">Обновление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="6f88a-103">Update oAuth2PermissionGrant</span></span>

> <span data-ttu-id="6f88a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6f88a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f88a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f88a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6f88a-106">Обновление свойства объекта oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="6f88a-106">Update the properties of oAuth2PermissionGrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f88a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6f88a-107">Permissions</span></span>

<span data-ttu-id="6f88a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f88a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6f88a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f88a-110">Permission type</span></span>      | <span data-ttu-id="6f88a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f88a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f88a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f88a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6f88a-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6f88a-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6f88a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f88a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f88a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f88a-115">Not supported.</span></span>    |
|<span data-ttu-id="6f88a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f88a-116">Application</span></span> | <span data-ttu-id="6f88a-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f88a-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f88a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f88a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /oAuth2Permissiongrants/{id}
PATCH /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
PATCH /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6f88a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f88a-119">Request headers</span></span>
| <span data-ttu-id="6f88a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6f88a-120">Name</span></span>       | <span data-ttu-id="6f88a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6f88a-121">Type</span></span> | <span data-ttu-id="6f88a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6f88a-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6f88a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f88a-123">Authorization</span></span>  | <span data-ttu-id="6f88a-124">string</span><span class="sxs-lookup"><span data-stu-id="6f88a-124">string</span></span>  | <span data-ttu-id="6f88a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f88a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f88a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6f88a-127">Request body</span></span>
<span data-ttu-id="6f88a-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="6f88a-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6f88a-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f88a-131">Property</span></span>     | <span data-ttu-id="6f88a-132">Тип</span><span class="sxs-lookup"><span data-stu-id="6f88a-132">Type</span></span>   |<span data-ttu-id="6f88a-133">Описание</span><span class="sxs-lookup"><span data-stu-id="6f88a-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f88a-134">scope</span><span class="sxs-lookup"><span data-stu-id="6f88a-134">scope</span></span>|<span data-ttu-id="6f88a-135">Строка</span><span class="sxs-lookup"><span data-stu-id="6f88a-135">String</span></span>| <span data-ttu-id="6f88a-136">Задает значение утверждения область, должно привести к приложению ресурсов в маркер доступа OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="6f88a-136">Specifies the value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="response"></a><span data-ttu-id="6f88a-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f88a-137">Response</span></span>

<span data-ttu-id="6f88a-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="6f88a-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f88a-140">Пример</span><span class="sxs-lookup"><span data-stu-id="6f88a-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6f88a-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f88a-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_oAuth2Permissiongrant"
}-->
```http
PATCH https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
Content-type: application/json
Content-length: 30

{
  "scope": "scope-value"
}
```
##### <a name="response"></a><span data-ttu-id="6f88a-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f88a-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
