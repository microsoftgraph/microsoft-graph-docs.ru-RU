---
title: 'Привилежедролеассигнмент: Макилигибле'
description: Выполнение назначения ролей как соответствующего требованиям. Если назначение роли уже доступно перед вызовом, оно ничего не делает. Если назначение роли является необратимым, а запрашивающий отличается от конечного пользователя, назначение роли станет доступным, и роль будет отключена для целевого пользователя. Если запрашивающей стороны является целевой пользователь, а роль является администратором безопасности или привилегированным администратором ролей, роль будет активирована с истечением срока действия по умолчанию.
localization_priority: Normal
ms.openlocfilehash: 54260da3f69819a1f7a351e072f8af851f0e3d3a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546602"
---
# <a name="privilegedroleassignment-makeeligible"></a><span data-ttu-id="1e84a-106">Привилежедролеассигнмент: Макилигибле</span><span class="sxs-lookup"><span data-stu-id="1e84a-106">privilegedRoleAssignment: makeEligible</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e84a-107">Выполнение назначения ролей как соответствующего требованиям.</span><span class="sxs-lookup"><span data-stu-id="1e84a-107">Make the role assignment as eligible.</span></span> <span data-ttu-id="1e84a-108">Если назначение роли уже доступно перед вызовом, оно ничего не делает.</span><span class="sxs-lookup"><span data-stu-id="1e84a-108">If the role assignment is already eligible before the call, it does nothing.</span></span> <span data-ttu-id="1e84a-109">Если назначение роли является необратимым, а запрашивающий отличается от конечного пользователя, назначение роли станет доступным, и роль будет отключена для целевого пользователя.</span><span class="sxs-lookup"><span data-stu-id="1e84a-109">If the role assignment is permanent and the requestor is different from the target user, the role assignment will become eligible and the role will be deactivated for the target user.</span></span> <span data-ttu-id="1e84a-110">Если запрашивающей стороны является целевой пользователь, а роль является администратором безопасности или привилегированным администратором ролей, роль будет активирована с истечением срока действия по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1e84a-110">If the requestor is the target user and the role is Security Administrator or Privileged Role Administrator, the role will be activated with the default expiration.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e84a-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1e84a-111">Permissions</span></span>
<span data-ttu-id="1e84a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e84a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="1e84a-114">Запрашивающая сторона должна иметь привилегированную роль _администратора ролей_ .</span><span class="sxs-lookup"><span data-stu-id="1e84a-114">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="1e84a-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e84a-115">Permission type</span></span>      | <span data-ttu-id="1e84a-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e84a-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e84a-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e84a-117">Delegated (work or school account)</span></span> | <span data-ttu-id="1e84a-118">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1e84a-118">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1e84a-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e84a-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e84a-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e84a-120">Not supported.</span></span>    |
|<span data-ttu-id="1e84a-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1e84a-121">Application</span></span> | <span data-ttu-id="1e84a-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e84a-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e84a-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e84a-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makeEligible
```
## <a name="request-headers"></a><span data-ttu-id="1e84a-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1e84a-124">Request headers</span></span>
| <span data-ttu-id="1e84a-125">Имя</span><span class="sxs-lookup"><span data-stu-id="1e84a-125">Name</span></span>       | <span data-ttu-id="1e84a-126">Описание</span><span class="sxs-lookup"><span data-stu-id="1e84a-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1e84a-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1e84a-127">Authorization</span></span>  | <span data-ttu-id="1e84a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e84a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e84a-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1e84a-130">Request body</span></span>
<span data-ttu-id="1e84a-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1e84a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e84a-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="1e84a-132">Response</span></span>

<span data-ttu-id="1e84a-133">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1e84a-133">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="1e84a-134">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="1e84a-134">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="1e84a-135">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="1e84a-135">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="1e84a-136">Пример</span><span class="sxs-lookup"><span data-stu-id="1e84a-136">Example</span></span>
<span data-ttu-id="1e84a-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1e84a-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1e84a-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e84a-138">Request</span></span>
<span data-ttu-id="1e84a-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1e84a-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_makeeligible"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}/makeEligible
```

##### <a name="response"></a><span data-ttu-id="1e84a-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e84a-140">Response</span></span>
<span data-ttu-id="1e84a-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1e84a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "privilegedRoleAssignment: makeEligible",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignment-makeeligible.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
