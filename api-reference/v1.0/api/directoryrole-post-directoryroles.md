---
title: Активация directoryRole
description: Активация роли каталога. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируются только неявные роли каталога пользователей, а также роли каталога администраторов организации. Чтобы получить доступ к членам и назначить для них другую роль каталога, сначала следует активировать ее с помощью соответствующего шаблона роли каталога (directoryRoleTemplate).
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5d127580c0a4851c5a991ccc0646007ddf1298a5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924918"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="03d01-106">Активация directoryRole</span><span class="sxs-lookup"><span data-stu-id="03d01-106">Activate directoryRole</span></span>

<span data-ttu-id="03d01-p102">Активация роли каталога. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируются только неявные роли каталога пользователей, а также роли каталога администраторов организации. Чтобы получить доступ к членам и назначить для них другую роль каталога, сначала следует активировать ее с помощью соответствующего шаблона роли каталога ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="03d01-p102">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="03d01-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03d01-111">Permissions</span></span>
<span data-ttu-id="03d01-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03d01-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03d01-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03d01-114">Permission type</span></span>      | <span data-ttu-id="03d01-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03d01-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03d01-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03d01-116">Delegated (work or school account)</span></span> | <span data-ttu-id="03d01-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="03d01-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="03d01-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03d01-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03d01-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03d01-119">Not supported.</span></span>    |
|<span data-ttu-id="03d01-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03d01-120">Application</span></span> | <span data-ttu-id="03d01-121">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03d01-121">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="03d01-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03d01-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="03d01-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03d01-123">Request headers</span></span>
| <span data-ttu-id="03d01-124">Имя</span><span class="sxs-lookup"><span data-stu-id="03d01-124">Name</span></span>       | <span data-ttu-id="03d01-125">Тип</span><span class="sxs-lookup"><span data-stu-id="03d01-125">Type</span></span> | <span data-ttu-id="03d01-126">Описание</span><span class="sxs-lookup"><span data-stu-id="03d01-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="03d01-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="03d01-127">Authorization</span></span>  | <span data-ttu-id="03d01-128">строка</span><span class="sxs-lookup"><span data-stu-id="03d01-128">string</span></span>  | <span data-ttu-id="03d01-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03d01-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="03d01-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="03d01-131">Content-Type</span></span>  | <span data-ttu-id="03d01-132">строка</span><span class="sxs-lookup"><span data-stu-id="03d01-132">string</span></span>  | <span data-ttu-id="03d01-133">application/json</span><span class="sxs-lookup"><span data-stu-id="03d01-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="03d01-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="03d01-134">Request body</span></span>
<span data-ttu-id="03d01-135">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03d01-135">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="03d01-136">В приведенной ниже таблице показаны обязательные свойства при активации роли каталога.</span><span class="sxs-lookup"><span data-stu-id="03d01-136">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="03d01-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="03d01-137">Parameter</span></span> | <span data-ttu-id="03d01-138">Тип</span><span class="sxs-lookup"><span data-stu-id="03d01-138">Type</span></span> | <span data-ttu-id="03d01-139">Описание</span><span class="sxs-lookup"><span data-stu-id="03d01-139">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="03d01-140">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="03d01-140">roleTemplateId</span></span> | <span data-ttu-id="03d01-141">строка</span><span class="sxs-lookup"><span data-stu-id="03d01-141">string</span></span> | <span data-ttu-id="03d01-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03d01-142">Required.</span></span> <span data-ttu-id="03d01-143">Идентификатор [directoryRoleTemplate](../resources/directoryroletemplate.md) на основе ролей.</span><span class="sxs-lookup"><span data-stu-id="03d01-143">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on.</span></span> <span data-ttu-id="03d01-144">Это единственный параметр, который может быть указано в запросе.</span><span class="sxs-lookup"><span data-stu-id="03d01-144">This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="03d01-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="03d01-145">Response</span></span>

<span data-ttu-id="03d01-146">В случае успеха этот метод возвратит код отклика `201 Created` и объект [directoryRole](../resources/directoryrole.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="03d01-146">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03d01-147">Пример</span><span class="sxs-lookup"><span data-stu-id="03d01-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03d01-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="03d01-148">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryrole_from_directoryroles"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles
Content-type: application/json

{
  "roleTemplateId": "roleTemplateId-value"
}
```
<span data-ttu-id="03d01-149">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03d01-149">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="03d01-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="03d01-150">Response</span></span>
<span data-ttu-id="03d01-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03d01-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
