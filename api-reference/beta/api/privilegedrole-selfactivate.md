---
title: 'privilegedRole: selfActivate'
description: Активируйте роль, назначенная для инициатора запроса.
localization_priority: Normal
ms.openlocfilehash: 9423d87714fcd4a7b7cce1dd5cd03bcef3e0ef9f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872130"
---
# <a name="privilegedrole-selfactivate"></a><span data-ttu-id="b3d85-103">privilegedRole: selfActivate</span><span class="sxs-lookup"><span data-stu-id="b3d85-103">privilegedRole: selfActivate</span></span>

><span data-ttu-id="b3d85-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b3d85-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3d85-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3d85-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b3d85-106">Активируйте роль, назначенная для инициатора запроса.</span><span class="sxs-lookup"><span data-stu-id="b3d85-106">Activate the role that is assigned to the requester.</span></span>

><span data-ttu-id="b3d85-107">**Примечание:** Эффективный 2018 декабря, этот интерфейс API больше не поддерживается и не должен использоваться.</span><span class="sxs-lookup"><span data-stu-id="b3d85-107">**Note:** Effective December 2018, this API will no longer be supported and should not be used.</span></span> <span data-ttu-id="b3d85-108">Вместо этого используйте [Создание PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) .</span><span class="sxs-lookup"><span data-stu-id="b3d85-108">Use the [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) instead.</span></span>


## <a name="permissions"></a><span data-ttu-id="b3d85-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3d85-109">Permissions</span></span>
<span data-ttu-id="b3d85-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3d85-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b3d85-112">Запрашивающая сторона может вызывать только ```selfActivate``` для роли, назначенные ему.</span><span class="sxs-lookup"><span data-stu-id="b3d85-112">The requestor can only call ```selfActivate``` for the role that is assigned to him.</span></span>
 

|<span data-ttu-id="b3d85-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3d85-113">Permission type</span></span>      | <span data-ttu-id="b3d85-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3d85-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3d85-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3d85-115">Delegated (work or school account)</span></span> | <span data-ttu-id="b3d85-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b3d85-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b3d85-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3d85-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3d85-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3d85-118">Not supported.</span></span>    |
|<span data-ttu-id="b3d85-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3d85-119">Application</span></span> | <span data-ttu-id="b3d85-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3d85-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3d85-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3d85-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfActivate
```

<span data-ttu-id="b3d85-122">Обратите внимание, что ``<id>`` — это идентификатор целевого роли.</span><span class="sxs-lookup"><span data-stu-id="b3d85-122">Note that ``<id>`` is the target role ID.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b3d85-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3d85-123">Request headers</span></span>
| <span data-ttu-id="b3d85-124">Имя</span><span class="sxs-lookup"><span data-stu-id="b3d85-124">Name</span></span>       | <span data-ttu-id="b3d85-125">Описание</span><span class="sxs-lookup"><span data-stu-id="b3d85-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b3d85-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3d85-126">Authorization</span></span>  | <span data-ttu-id="b3d85-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3d85-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3d85-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b3d85-129">Request body</span></span>
<span data-ttu-id="b3d85-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b3d85-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b3d85-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="b3d85-131">Parameter</span></span>    | <span data-ttu-id="b3d85-132">Тип</span><span class="sxs-lookup"><span data-stu-id="b3d85-132">Type</span></span>   |<span data-ttu-id="b3d85-133">Описание</span><span class="sxs-lookup"><span data-stu-id="b3d85-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b3d85-134">Причина</span><span class="sxs-lookup"><span data-stu-id="b3d85-134">reason</span></span>|<span data-ttu-id="b3d85-135">string</span><span class="sxs-lookup"><span data-stu-id="b3d85-135">string</span></span>|<span data-ttu-id="b3d85-136">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="b3d85-136">Optional.</span></span> <span data-ttu-id="b3d85-137">Описание причины для активации этой роли.</span><span class="sxs-lookup"><span data-stu-id="b3d85-137">Description about the reason for this role activation.</span></span>|
|<span data-ttu-id="b3d85-138">duration</span><span class="sxs-lookup"><span data-stu-id="b3d85-138">duration</span></span>|<span data-ttu-id="b3d85-139">string</span><span class="sxs-lookup"><span data-stu-id="b3d85-139">string</span></span>|<span data-ttu-id="b3d85-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="b3d85-140">Optional.</span></span> <span data-ttu-id="b3d85-141">Допустимые значения может быть ```min``` (Минимальная активации длительность), ```default``` (длительность по умолчанию активации для роли), или значение типа double, чтобы указать, сколько часов активации.</span><span class="sxs-lookup"><span data-stu-id="b3d85-141">Valid values could be ```min``` (minimal activation duration), ```default``` (default activation duration for the role), or a double value to specify how many hours is the activation.</span></span> <span data-ttu-id="b3d85-142">Указанный период не может превышать продолжительность активации роли из параметров ролей.</span><span class="sxs-lookup"><span data-stu-id="b3d85-142">The specified duration cannot be longer than the role's activation duration from the role setting.</span></span> |
|<span data-ttu-id="b3d85-143">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="b3d85-143">ticketNumber</span></span>|<span data-ttu-id="b3d85-144">string</span><span class="sxs-lookup"><span data-stu-id="b3d85-144">string</span></span>|<span data-ttu-id="b3d85-145">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="b3d85-145">Optional.</span></span> <span data-ttu-id="b3d85-146">Номер билетов, используемый для отслеживания активации этой роли.</span><span class="sxs-lookup"><span data-stu-id="b3d85-146">The ticket number that is used to tracking this role activation.</span></span>|
|<span data-ttu-id="b3d85-147">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="b3d85-147">ticketSystem</span></span>|<span data-ttu-id="b3d85-148">string</span><span class="sxs-lookup"><span data-stu-id="b3d85-148">string</span></span>|<span data-ttu-id="b3d85-149">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="b3d85-149">Optional.</span></span> <span data-ttu-id="b3d85-150">Система билетов.</span><span class="sxs-lookup"><span data-stu-id="b3d85-150">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="b3d85-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="b3d85-151">Response</span></span>

<span data-ttu-id="b3d85-152">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [privilegedRoleAssignment](../resources/privilegedroleassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b3d85-152">If successful, this method returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="b3d85-153">Обратите внимание, что необходимо зарегистрировать для PIM клиента.</span><span class="sxs-lookup"><span data-stu-id="b3d85-153">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="b3d85-154">В противном случае будут возвращены код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="b3d85-154">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="b3d85-155">Пример</span><span class="sxs-lookup"><span data-stu-id="b3d85-155">Example</span></span>
<span data-ttu-id="b3d85-156">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="b3d85-156">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b3d85-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3d85-157">Request</span></span>
<span data-ttu-id="b3d85-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3d85-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfActivate
Content-type: application/json
Content-length: 142

{
  "reason": "reason-value",
  "duration": "duration-value",
  "ticketNumber": "ticketNumber-value",
  "ticketSystem": "ticketSystem-value"
}
```

##### <a name="response"></a><span data-ttu-id="b3d85-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="b3d85-159">Response</span></span>
<span data-ttu-id="b3d85-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b3d85-160">Here is an example of the response.</span></span> 

><span data-ttu-id="b3d85-p110">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b3d85-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "privilegedRole: selfActivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
