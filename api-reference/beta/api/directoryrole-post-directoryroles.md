---
title: Активация directoryRole
description: Активация роли каталога. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируются только администраторы компании и роли каталога неявных пользователей. Чтобы получить доступ к членам и назначить для них другую роль каталога, сначала следует активировать ее с помощью соответствующего шаблона роли каталога (directoryRoleTemplate).
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 094374dd8aa5d68e1adaad89e9a3b46987bc7c8f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454764"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="222f9-106">Активация directoryRole</span><span class="sxs-lookup"><span data-stu-id="222f9-106">Activate directoryRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="222f9-107">Активация роли каталога.</span><span class="sxs-lookup"><span data-stu-id="222f9-107">Activate a directory role.</span></span> <span data-ttu-id="222f9-108">Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте.</span><span class="sxs-lookup"><span data-stu-id="222f9-108">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="222f9-109">По умолчанию активируются только администраторы компании и роли каталога неявных пользователей.</span><span class="sxs-lookup"><span data-stu-id="222f9-109">Only the Company Administrators  and the implicit Users directory roles are activated by default.</span></span> <span data-ttu-id="222f9-110">Чтобы получить доступ к членам и назначить для них другую роль каталога, сначала следует активировать ее с помощью соответствующего шаблона роли каталога ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="222f9-110">To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="222f9-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="222f9-111">Permissions</span></span>
<span data-ttu-id="222f9-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="222f9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="222f9-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="222f9-114">Permission type</span></span>      | <span data-ttu-id="222f9-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="222f9-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="222f9-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="222f9-116">Delegated (work or school account)</span></span> | <span data-ttu-id="222f9-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="222f9-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="222f9-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="222f9-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="222f9-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="222f9-119">Not supported.</span></span>    |
|<span data-ttu-id="222f9-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="222f9-120">Application</span></span> | <span data-ttu-id="222f9-121">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="222f9-121">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="222f9-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="222f9-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="222f9-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="222f9-123">Request headers</span></span>
| <span data-ttu-id="222f9-124">Имя</span><span class="sxs-lookup"><span data-stu-id="222f9-124">Name</span></span>       | <span data-ttu-id="222f9-125">Тип</span><span class="sxs-lookup"><span data-stu-id="222f9-125">Type</span></span> | <span data-ttu-id="222f9-126">Описание</span><span class="sxs-lookup"><span data-stu-id="222f9-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="222f9-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="222f9-127">Authorization</span></span>  | <span data-ttu-id="222f9-128">string</span><span class="sxs-lookup"><span data-stu-id="222f9-128">string</span></span>  | <span data-ttu-id="222f9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="222f9-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="222f9-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="222f9-131">Request body</span></span>
<span data-ttu-id="222f9-132">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="222f9-132">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="222f9-133">В приведенной ниже таблице показаны обязательные свойства при активации роли каталога.</span><span class="sxs-lookup"><span data-stu-id="222f9-133">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="222f9-134">Обязательный параметр</span><span class="sxs-lookup"><span data-stu-id="222f9-134">Required parameter</span></span> | <span data-ttu-id="222f9-135">Тип</span><span class="sxs-lookup"><span data-stu-id="222f9-135">Type</span></span> | <span data-ttu-id="222f9-136">Описание</span><span class="sxs-lookup"><span data-stu-id="222f9-136">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="222f9-137">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="222f9-137">roleTemplateId</span></span> | <span data-ttu-id="222f9-138">string</span><span class="sxs-lookup"><span data-stu-id="222f9-138">string</span></span> | <span data-ttu-id="222f9-p105">Идентификатор для объекта [directoryRoleTemplate](../resources/directoryroletemplate.md), который лежит в основе роли. Это единственное свойство, которое можно указать в запросе.</span><span class="sxs-lookup"><span data-stu-id="222f9-p105">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="222f9-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="222f9-141">Response</span></span>

<span data-ttu-id="222f9-142">В случае успеха этот метод возвратит код отклика `201 Created` и объект [directoryRole](../resources/directoryrole.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="222f9-142">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="222f9-143">Пример</span><span class="sxs-lookup"><span data-stu-id="222f9-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="222f9-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="222f9-144">Request</span></span>
<span data-ttu-id="222f9-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="222f9-145">Here is an example of the request.</span></span>
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
<span data-ttu-id="222f9-146">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="222f9-146">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="222f9-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="222f9-147">Response</span></span>
<span data-ttu-id="222f9-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="222f9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
