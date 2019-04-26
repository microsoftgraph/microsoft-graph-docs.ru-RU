---
title: 'Привилежедроле: Селфдеактивате'
description: Деактивация роли, назначенной запрашивающей стороне.
localization_priority: Normal
ms.openlocfilehash: 4e627486cf58f1ea7bc71e29fe9c06c3fa3dfb25
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337431"
---
# <a name="privilegedrole-selfdeactivate"></a><span data-ttu-id="49758-103">Привилежедроле: Селфдеактивате</span><span class="sxs-lookup"><span data-stu-id="49758-103">privilegedRole: selfDeactivate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49758-104">Деактивация роли, назначенной запрашивающей стороне.</span><span class="sxs-lookup"><span data-stu-id="49758-104">Deactivate the role that is assigned to the requestor.</span></span>
## <a name="permissions"></a><span data-ttu-id="49758-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49758-105">Permissions</span></span>
<span data-ttu-id="49758-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49758-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="49758-108">Запрашивающая сторона может вызвать ```selfDeactivate``` только назначенную ему роль.</span><span class="sxs-lookup"><span data-stu-id="49758-108">The requestor can only call ```selfDeactivate``` for the role that is assigned to him.</span></span> 

|<span data-ttu-id="49758-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49758-109">Permission type</span></span>      | <span data-ttu-id="49758-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49758-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49758-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49758-111">Delegated (work or school account)</span></span> | <span data-ttu-id="49758-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="49758-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="49758-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49758-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49758-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49758-114">Not supported.</span></span>    |
|<span data-ttu-id="49758-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49758-115">Application</span></span> | <span data-ttu-id="49758-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49758-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49758-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49758-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfDeactivate
```

<span data-ttu-id="49758-118">Обратите ``<id>`` внимание, что это идентификатор целевой роли.</span><span class="sxs-lookup"><span data-stu-id="49758-118">Note that ``<id>`` is the target role id.</span></span>
## <a name="request-headers"></a><span data-ttu-id="49758-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49758-119">Request headers</span></span>
| <span data-ttu-id="49758-120">Имя</span><span class="sxs-lookup"><span data-stu-id="49758-120">Name</span></span>       | <span data-ttu-id="49758-121">Описание</span><span class="sxs-lookup"><span data-stu-id="49758-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="49758-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49758-122">Authorization</span></span>  | <span data-ttu-id="49758-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49758-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49758-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49758-125">Request body</span></span>
<span data-ttu-id="49758-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="49758-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49758-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="49758-127">Response</span></span>

<span data-ttu-id="49758-128">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49758-128">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="49758-129">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="49758-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="49758-130">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="49758-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="49758-131">Пример</span><span class="sxs-lookup"><span data-stu-id="49758-131">Example</span></span>
<span data-ttu-id="49758-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="49758-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="49758-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="49758-133">Request</span></span>
<span data-ttu-id="49758-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49758-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfdeactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfDeactivate
```

##### <a name="response"></a><span data-ttu-id="49758-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="49758-135">Response</span></span>
<span data-ttu-id="49758-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49758-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRole: selfDeactivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
