---
title: Обновление oAuth2PermissionGrant
description: Обновление свойства объекта oAuth2PermissionGrant.
localization_priority: Normal
ms.openlocfilehash: fb990c56b4d7ae62ac35935a91d69688b96bff28
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522142"
---
# <a name="update-oauth2permissiongrant"></a><span data-ttu-id="3a630-103">Обновление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="3a630-103">Update oAuth2PermissionGrant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a630-104">Обновление свойства объекта oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="3a630-104">Update the properties of oAuth2PermissionGrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a630-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a630-105">Permissions</span></span>

<span data-ttu-id="3a630-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a630-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3a630-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a630-108">Permission type</span></span>      | <span data-ttu-id="3a630-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a630-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a630-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a630-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3a630-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3a630-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3a630-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a630-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a630-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a630-113">Not supported.</span></span>    |
|<span data-ttu-id="3a630-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a630-114">Application</span></span> | <span data-ttu-id="3a630-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a630-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a630-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a630-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /oAuth2Permissiongrants/{id}
PATCH /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
PATCH /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3a630-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a630-117">Request headers</span></span>
| <span data-ttu-id="3a630-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3a630-118">Name</span></span>       | <span data-ttu-id="3a630-119">Тип</span><span class="sxs-lookup"><span data-stu-id="3a630-119">Type</span></span> | <span data-ttu-id="3a630-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3a630-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3a630-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a630-121">Authorization</span></span>  | <span data-ttu-id="3a630-122">string</span><span class="sxs-lookup"><span data-stu-id="3a630-122">string</span></span>  | <span data-ttu-id="3a630-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a630-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a630-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a630-125">Request body</span></span>
<span data-ttu-id="3a630-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="3a630-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3a630-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a630-129">Property</span></span>     | <span data-ttu-id="3a630-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3a630-130">Type</span></span>   |<span data-ttu-id="3a630-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3a630-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a630-132">scope</span><span class="sxs-lookup"><span data-stu-id="3a630-132">scope</span></span>|<span data-ttu-id="3a630-133">String</span><span class="sxs-lookup"><span data-stu-id="3a630-133">String</span></span>| <span data-ttu-id="3a630-134">Задает значение утверждения область, должно привести к приложению ресурсов в маркер доступа OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="3a630-134">Specifies the value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="response"></a><span data-ttu-id="3a630-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a630-135">Response</span></span>

<span data-ttu-id="3a630-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="3a630-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a630-138">Пример</span><span class="sxs-lookup"><span data-stu-id="3a630-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a630-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a630-139">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="3a630-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a630-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/oauth2permissiongrant-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
