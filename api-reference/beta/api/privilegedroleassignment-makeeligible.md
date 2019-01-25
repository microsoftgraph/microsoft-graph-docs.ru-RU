---
title: 'privilegedRoleAssignment: makeEligible'
description: Сделайте назначения ролей как подходящими. Если назначения ролей подходящими перед выполнением звонка, не выполняет никаких действий. Если постоянное назначение ролей и инициатора запроса отличается от конечного пользователя, становится доступным назначения роли и роли будут отключены для конечного пользователя. Если инициатора запроса конечного пользователя и роль имеет права администратора безопасности или привилегированной роль администратора, роль будет активировать истечение срока действия по умолчанию.
localization_priority: Normal
ms.openlocfilehash: 54260da3f69819a1f7a351e072f8af851f0e3d3a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527238"
---
# <a name="privilegedroleassignment-makeeligible"></a><span data-ttu-id="4dd58-106">privilegedRoleAssignment: makeEligible</span><span class="sxs-lookup"><span data-stu-id="4dd58-106">privilegedRoleAssignment: makeEligible</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4dd58-107">Сделайте назначения ролей как подходящими.</span><span class="sxs-lookup"><span data-stu-id="4dd58-107">Make the role assignment as eligible.</span></span> <span data-ttu-id="4dd58-108">Если назначения ролей подходящими перед выполнением звонка, не выполняет никаких действий.</span><span class="sxs-lookup"><span data-stu-id="4dd58-108">If the role assignment is already eligible before the call, it does nothing.</span></span> <span data-ttu-id="4dd58-109">Если постоянное назначение ролей и инициатора запроса отличается от конечного пользователя, становится доступным назначения роли и роли будут отключены для конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="4dd58-109">If the role assignment is permanent and the requestor is different from the target user, the role assignment will become eligible and the role will be deactivated for the target user.</span></span> <span data-ttu-id="4dd58-110">Если инициатора запроса конечного пользователя и роль имеет права администратора безопасности или привилегированной роль администратора, роль будет активировать истечение срока действия по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4dd58-110">If the requestor is the target user and the role is Security Administrator or Privileged Role Administrator, the role will be activated with the default expiration.</span></span>

## <a name="permissions"></a><span data-ttu-id="4dd58-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4dd58-111">Permissions</span></span>
<span data-ttu-id="4dd58-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4dd58-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4dd58-114">Запрашивающая сторона должна иметь роль _Привилегированной роль администратора_ .</span><span class="sxs-lookup"><span data-stu-id="4dd58-114">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="4dd58-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4dd58-115">Permission type</span></span>      | <span data-ttu-id="4dd58-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4dd58-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4dd58-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4dd58-117">Delegated (work or school account)</span></span> | <span data-ttu-id="4dd58-118">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4dd58-118">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4dd58-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4dd58-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4dd58-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dd58-120">Not supported.</span></span>    |
|<span data-ttu-id="4dd58-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4dd58-121">Application</span></span> | <span data-ttu-id="4dd58-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dd58-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4dd58-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4dd58-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makeEligible
```
## <a name="request-headers"></a><span data-ttu-id="4dd58-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4dd58-124">Request headers</span></span>
| <span data-ttu-id="4dd58-125">Имя</span><span class="sxs-lookup"><span data-stu-id="4dd58-125">Name</span></span>       | <span data-ttu-id="4dd58-126">Описание</span><span class="sxs-lookup"><span data-stu-id="4dd58-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4dd58-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4dd58-127">Authorization</span></span>  | <span data-ttu-id="4dd58-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4dd58-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4dd58-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4dd58-130">Request body</span></span>
<span data-ttu-id="4dd58-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4dd58-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4dd58-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="4dd58-132">Response</span></span>

<span data-ttu-id="4dd58-133">Успешно завершена, этот метод возвращает `200 OK` объект [privilegedRoleAssignment](../resources/privilegedroleassignment.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4dd58-133">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="4dd58-134">Обратите внимание, что необходимо зарегистрировать для PIM клиента.</span><span class="sxs-lookup"><span data-stu-id="4dd58-134">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="4dd58-135">В противном случае будут возвращены код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="4dd58-135">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="4dd58-136">Пример</span><span class="sxs-lookup"><span data-stu-id="4dd58-136">Example</span></span>
<span data-ttu-id="4dd58-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4dd58-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4dd58-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="4dd58-138">Request</span></span>
<span data-ttu-id="4dd58-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4dd58-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_makeeligible"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}/makeEligible
```

##### <a name="response"></a><span data-ttu-id="4dd58-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="4dd58-140">Response</span></span>
<span data-ttu-id="4dd58-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4dd58-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
