---
title: 'privilegedRoleAssignment: makeEligible'
description: Сделайте назначения ролей как подходящими. Если назначения ролей подходящими перед выполнением звонка, не выполняет никаких действий. Если постоянное назначение ролей и инициатора запроса отличается от конечного пользователя, становится доступным назначения роли и роли будут отключены для конечного пользователя. Если инициатора запроса конечного пользователя и роль имеет права администратора безопасности или привилегированной роль администратора, роль будет активировать истечение срока действия по умолчанию.
ms.openlocfilehash: f39f508c7aeae4d85db92b43f406cd3497533e38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075445"
---
# <a name="privilegedroleassignment-makeeligible"></a><span data-ttu-id="a0b62-106">privilegedRoleAssignment: makeEligible</span><span class="sxs-lookup"><span data-stu-id="a0b62-106">privilegedRoleAssignment: makeEligible</span></span>

> <span data-ttu-id="a0b62-107">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a0b62-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0b62-108">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0b62-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a0b62-109">Сделайте назначения ролей как подходящими.</span><span class="sxs-lookup"><span data-stu-id="a0b62-109">Make the role assignment as eligible.</span></span> <span data-ttu-id="a0b62-110">Если назначения ролей подходящими перед выполнением звонка, не выполняет никаких действий.</span><span class="sxs-lookup"><span data-stu-id="a0b62-110">If the role assignment is already eligible before the call, it does nothing.</span></span> <span data-ttu-id="a0b62-111">Если постоянное назначение ролей и инициатора запроса отличается от конечного пользователя, становится доступным назначения роли и роли будут отключены для конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="a0b62-111">If the role assignment is permanent and the requestor is different from the target user, the role assignment will become eligible and the role will be deactivated for the target user.</span></span> <span data-ttu-id="a0b62-112">Если инициатора запроса конечного пользователя и роль имеет права администратора безопасности или привилегированной роль администратора, роль будет активировать истечение срока действия по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a0b62-112">If the requestor is the target user and the role is Security Administrator or Privileged Role Administrator, the role will be activated with the default expiration.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0b62-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a0b62-113">Permissions</span></span>
<span data-ttu-id="a0b62-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0b62-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a0b62-116">Запрашивающая сторона должна иметь роль _Привилегированной роль администратора_ .</span><span class="sxs-lookup"><span data-stu-id="a0b62-116">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="a0b62-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0b62-117">Permission type</span></span>      | <span data-ttu-id="a0b62-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0b62-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0b62-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0b62-119">Delegated (work or school account)</span></span> | <span data-ttu-id="a0b62-120">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a0b62-120">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a0b62-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0b62-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0b62-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0b62-122">Not supported.</span></span>    |
|<span data-ttu-id="a0b62-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0b62-123">Application</span></span> | <span data-ttu-id="a0b62-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0b62-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0b62-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0b62-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makeEligible
```
## <a name="request-headers"></a><span data-ttu-id="a0b62-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0b62-126">Request headers</span></span>
| <span data-ttu-id="a0b62-127">Имя</span><span class="sxs-lookup"><span data-stu-id="a0b62-127">Name</span></span>       | <span data-ttu-id="a0b62-128">Описание</span><span class="sxs-lookup"><span data-stu-id="a0b62-128">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a0b62-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a0b62-129">Authorization</span></span>  | <span data-ttu-id="a0b62-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0b62-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0b62-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a0b62-132">Request body</span></span>
<span data-ttu-id="a0b62-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a0b62-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0b62-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="a0b62-134">Response</span></span>

<span data-ttu-id="a0b62-135">Успешно завершена, этот метод возвращает `200 OK` объект [privilegedRoleAssignment](../resources/privilegedroleassignment.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a0b62-135">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="a0b62-136">Обратите внимание, что необходимо зарегистрировать для PIM клиента.</span><span class="sxs-lookup"><span data-stu-id="a0b62-136">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="a0b62-137">В противном случае будут возвращены код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="a0b62-137">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="a0b62-138">Пример</span><span class="sxs-lookup"><span data-stu-id="a0b62-138">Example</span></span>
<span data-ttu-id="a0b62-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a0b62-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a0b62-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0b62-140">Request</span></span>
<span data-ttu-id="a0b62-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0b62-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_makeeligible"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}/makeEligible
```

##### <a name="response"></a><span data-ttu-id="a0b62-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="a0b62-142">Response</span></span>
<span data-ttu-id="a0b62-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="a0b62-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment: makeEligible",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->