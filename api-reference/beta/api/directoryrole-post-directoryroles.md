---
title: Активация directoryRole
description: Активация роли каталога. Для чтения роли каталога или обновите его члены, необходимо активировать в клиентов. Только администраторы организации и неявных directory роли пользователей активируется по умолчанию. Для доступа и добавления членов в другой каталог роли, вам необходимо активировать его с ее directory роль шаблон (directoryRoleTemplate).
ms.openlocfilehash: 2a81bedaf4998e44825abc5e2cf0a93ec8708f96
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077237"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="61122-106">Активация directoryRole</span><span class="sxs-lookup"><span data-stu-id="61122-106">Activate directoryRole</span></span>

> <span data-ttu-id="61122-107">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="61122-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61122-108">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61122-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="61122-109">Активация роли каталога.</span><span class="sxs-lookup"><span data-stu-id="61122-109">Activate a directory role.</span></span> <span data-ttu-id="61122-110">Для чтения роли каталога или обновите его члены, необходимо активировать в клиентов.</span><span class="sxs-lookup"><span data-stu-id="61122-110">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="61122-111">Только администраторы организации и неявных directory роли пользователей активируется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="61122-111">Only the Company Administrators  and the implicit Users directory roles are activated by default.</span></span> <span data-ttu-id="61122-112">Для доступа и добавления членов в другой каталог роли, вам необходимо активировать его с ее directory роль шаблон ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="61122-112">To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="61122-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="61122-113">Permissions</span></span>
<span data-ttu-id="61122-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61122-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61122-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="61122-116">Permission type</span></span>      | <span data-ttu-id="61122-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="61122-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61122-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="61122-118">Delegated (work or school account)</span></span> | <span data-ttu-id="61122-119">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="61122-119">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="61122-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="61122-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61122-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61122-121">Not supported.</span></span>    |
|<span data-ttu-id="61122-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="61122-122">Application</span></span> | <span data-ttu-id="61122-123">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61122-123">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="61122-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61122-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="61122-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="61122-125">Request headers</span></span>
| <span data-ttu-id="61122-126">Имя</span><span class="sxs-lookup"><span data-stu-id="61122-126">Name</span></span>       | <span data-ttu-id="61122-127">Тип</span><span class="sxs-lookup"><span data-stu-id="61122-127">Type</span></span> | <span data-ttu-id="61122-128">Описание</span><span class="sxs-lookup"><span data-stu-id="61122-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="61122-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="61122-129">Authorization</span></span>  | <span data-ttu-id="61122-130">string</span><span class="sxs-lookup"><span data-stu-id="61122-130">string</span></span>  | <span data-ttu-id="61122-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="61122-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61122-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="61122-133">Request body</span></span>
<span data-ttu-id="61122-134">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61122-134">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="61122-135">В приведенной ниже таблице показаны обязательные свойства при активации роли каталога.</span><span class="sxs-lookup"><span data-stu-id="61122-135">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="61122-136">Обязательный параметр</span><span class="sxs-lookup"><span data-stu-id="61122-136">Required parameter</span></span> | <span data-ttu-id="61122-137">Тип</span><span class="sxs-lookup"><span data-stu-id="61122-137">Type</span></span> | <span data-ttu-id="61122-138">Описание</span><span class="sxs-lookup"><span data-stu-id="61122-138">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="61122-139">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="61122-139">roleTemplateId</span></span> | <span data-ttu-id="61122-140">string</span><span class="sxs-lookup"><span data-stu-id="61122-140">string</span></span> | <span data-ttu-id="61122-p106">Идентификатор для объекта [directoryRoleTemplate](../resources/directoryroletemplate.md), который лежит в основе роли. Это единственное свойство, которое можно указать в запросе.</span><span class="sxs-lookup"><span data-stu-id="61122-p106">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="61122-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="61122-143">Response</span></span>

<span data-ttu-id="61122-144">В случае успеха этот метод возвратит код отклика `201 Created` и объект [directoryRole](../resources/directoryrole.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="61122-144">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61122-145">Пример</span><span class="sxs-lookup"><span data-stu-id="61122-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="61122-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="61122-146">Request</span></span>
<span data-ttu-id="61122-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="61122-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryrole_from_directoryroles"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles
Content-type: application/json
Content-length: 153

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value"
}
```
<span data-ttu-id="61122-148">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61122-148">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="61122-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="61122-149">Response</span></span>
<span data-ttu-id="61122-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="61122-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 175

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
