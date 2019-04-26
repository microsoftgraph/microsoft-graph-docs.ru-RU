---
title: Активация directoryRole
description: Активация роли каталога. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируются только неявные роли каталога пользователей, а также роли каталога администраторов организации. Чтобы получить доступ к членам и назначить для них другую роль каталога, сначала следует активировать ее с помощью соответствующего шаблона роли каталога (directoryRoleTemplate).
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5d127580c0a4851c5a991ccc0646007ddf1298a5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562435"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="a68ea-106">Активация directoryRole</span><span class="sxs-lookup"><span data-stu-id="a68ea-106">Activate directoryRole</span></span>

<span data-ttu-id="a68ea-p102">Активация роли каталога. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируются только неявные роли каталога пользователей, а также роли каталога администраторов организации. Чтобы получить доступ к членам и назначить для них другую роль каталога, сначала следует активировать ее с помощью соответствующего шаблона роли каталога ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="a68ea-p102">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="a68ea-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a68ea-111">Permissions</span></span>
<span data-ttu-id="a68ea-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a68ea-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a68ea-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a68ea-114">Permission type</span></span>      | <span data-ttu-id="a68ea-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a68ea-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a68ea-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a68ea-116">Delegated (work or school account)</span></span> | <span data-ttu-id="a68ea-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a68ea-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a68ea-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a68ea-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a68ea-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a68ea-119">Not supported.</span></span>    |
|<span data-ttu-id="a68ea-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a68ea-120">Application</span></span> | <span data-ttu-id="a68ea-121">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a68ea-121">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a68ea-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a68ea-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="a68ea-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a68ea-123">Request headers</span></span>
| <span data-ttu-id="a68ea-124">Имя</span><span class="sxs-lookup"><span data-stu-id="a68ea-124">Name</span></span>       | <span data-ttu-id="a68ea-125">Тип</span><span class="sxs-lookup"><span data-stu-id="a68ea-125">Type</span></span> | <span data-ttu-id="a68ea-126">Описание</span><span class="sxs-lookup"><span data-stu-id="a68ea-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a68ea-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="a68ea-127">Authorization</span></span>  | <span data-ttu-id="a68ea-128">string</span><span class="sxs-lookup"><span data-stu-id="a68ea-128">string</span></span>  | <span data-ttu-id="a68ea-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a68ea-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a68ea-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a68ea-131">Content-Type</span></span>  | <span data-ttu-id="a68ea-132">string</span><span class="sxs-lookup"><span data-stu-id="a68ea-132">string</span></span>  | <span data-ttu-id="a68ea-133">application/json</span><span class="sxs-lookup"><span data-stu-id="a68ea-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a68ea-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a68ea-134">Request body</span></span>
<span data-ttu-id="a68ea-135">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a68ea-135">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="a68ea-136">В приведенной ниже таблице показаны обязательные свойства при активации роли каталога.</span><span class="sxs-lookup"><span data-stu-id="a68ea-136">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="a68ea-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="a68ea-137">Parameter</span></span> | <span data-ttu-id="a68ea-138">Тип</span><span class="sxs-lookup"><span data-stu-id="a68ea-138">Type</span></span> | <span data-ttu-id="a68ea-139">Описание</span><span class="sxs-lookup"><span data-stu-id="a68ea-139">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="a68ea-140">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="a68ea-140">roleTemplateId</span></span> | <span data-ttu-id="a68ea-141">string</span><span class="sxs-lookup"><span data-stu-id="a68ea-141">string</span></span> | <span data-ttu-id="a68ea-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a68ea-142">Required.</span></span> <span data-ttu-id="a68ea-143">Идентификатор для объекта [directoryRoleTemplate](../resources/directoryroletemplate.md), который лежит в основе роли.</span><span class="sxs-lookup"><span data-stu-id="a68ea-143">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on.</span></span> <span data-ttu-id="a68ea-144">Это единственное свойство, которое можно указать в запросе.</span><span class="sxs-lookup"><span data-stu-id="a68ea-144">This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="a68ea-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="a68ea-145">Response</span></span>

<span data-ttu-id="a68ea-146">В случае успеха этот метод возвратит код отклика `201 Created` и объект [directoryRole](../resources/directoryrole.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a68ea-146">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a68ea-147">Пример</span><span class="sxs-lookup"><span data-stu-id="a68ea-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a68ea-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="a68ea-148">Request</span></span>

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
<span data-ttu-id="a68ea-149">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a68ea-149">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a68ea-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="a68ea-150">Response</span></span>
<span data-ttu-id="a68ea-p106">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a68ea-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
