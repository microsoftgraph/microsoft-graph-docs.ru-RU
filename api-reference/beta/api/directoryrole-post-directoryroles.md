---
title: Активация directoryRole
description: Активация роли каталога. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируются только неявные роли каталога пользователей, а также роли каталога администраторов организации. Чтобы получить доступ к членам и назначить для них другую роль каталога, сначала следует активировать ее с помощью соответствующего шаблона роли каталога (directoryRoleTemplate).
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 094374dd8aa5d68e1adaad89e9a3b46987bc7c8f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522730"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="4a56b-106">Активация directoryRole</span><span class="sxs-lookup"><span data-stu-id="4a56b-106">Activate directoryRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a56b-107">Активация роли каталога.</span><span class="sxs-lookup"><span data-stu-id="4a56b-107">Activate a directory role.</span></span> <span data-ttu-id="4a56b-108">Для чтения роли каталога или обновите его члены, необходимо активировать в клиентов.</span><span class="sxs-lookup"><span data-stu-id="4a56b-108">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="4a56b-109">Только администраторы организации и неявных directory роли пользователей активируется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a56b-109">Only the Company Administrators  and the implicit Users directory roles are activated by default.</span></span> <span data-ttu-id="4a56b-110">Для доступа и добавления членов в другой каталог роли, вам необходимо активировать его с ее directory роль шаблон ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="4a56b-110">To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="4a56b-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a56b-111">Permissions</span></span>
<span data-ttu-id="4a56b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a56b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a56b-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a56b-114">Permission type</span></span>      | <span data-ttu-id="4a56b-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a56b-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a56b-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a56b-116">Delegated (work or school account)</span></span> | <span data-ttu-id="4a56b-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4a56b-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4a56b-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a56b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a56b-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a56b-119">Not supported.</span></span>    |
|<span data-ttu-id="4a56b-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a56b-120">Application</span></span> | <span data-ttu-id="4a56b-121">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a56b-121">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a56b-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a56b-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="4a56b-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a56b-123">Request headers</span></span>
| <span data-ttu-id="4a56b-124">Имя</span><span class="sxs-lookup"><span data-stu-id="4a56b-124">Name</span></span>       | <span data-ttu-id="4a56b-125">Тип</span><span class="sxs-lookup"><span data-stu-id="4a56b-125">Type</span></span> | <span data-ttu-id="4a56b-126">Описание</span><span class="sxs-lookup"><span data-stu-id="4a56b-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4a56b-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a56b-127">Authorization</span></span>  | <span data-ttu-id="4a56b-128">string</span><span class="sxs-lookup"><span data-stu-id="4a56b-128">string</span></span>  | <span data-ttu-id="4a56b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a56b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a56b-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4a56b-131">Request body</span></span>
<span data-ttu-id="4a56b-132">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a56b-132">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="4a56b-133">В приведенной ниже таблице показаны обязательные свойства при активации роли каталога.</span><span class="sxs-lookup"><span data-stu-id="4a56b-133">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="4a56b-134">Обязательный параметр</span><span class="sxs-lookup"><span data-stu-id="4a56b-134">Required parameter</span></span> | <span data-ttu-id="4a56b-135">Тип</span><span class="sxs-lookup"><span data-stu-id="4a56b-135">Type</span></span> | <span data-ttu-id="4a56b-136">Описание</span><span class="sxs-lookup"><span data-stu-id="4a56b-136">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="4a56b-137">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="4a56b-137">roleTemplateId</span></span> | <span data-ttu-id="4a56b-138">string</span><span class="sxs-lookup"><span data-stu-id="4a56b-138">string</span></span> | <span data-ttu-id="4a56b-p105">Идентификатор для объекта [directoryRoleTemplate](../resources/directoryroletemplate.md), который лежит в основе роли. Это единственное свойство, которое можно указать в запросе.</span><span class="sxs-lookup"><span data-stu-id="4a56b-p105">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="4a56b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a56b-141">Response</span></span>

<span data-ttu-id="4a56b-142">В случае успеха этот метод возвратит код отклика `201 Created` и объект [directoryRole](../resources/directoryrole.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4a56b-142">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a56b-143">Пример</span><span class="sxs-lookup"><span data-stu-id="4a56b-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a56b-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a56b-144">Request</span></span>
<span data-ttu-id="4a56b-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a56b-145">Here is an example of the request.</span></span>
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
<span data-ttu-id="4a56b-146">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a56b-146">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4a56b-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="4a56b-147">Response</span></span>
<span data-ttu-id="4a56b-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4a56b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryrole-post-directoryroles.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
