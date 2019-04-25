---
title: Назначение политики
description: Назначает политику для приложения или участника службы.
localization_priority: Normal
ms.openlocfilehash: 15ba6a42f5c5d39caf57b25ebafc5dd4bc7990fc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546800"
---
# <a name="assign-policy"></a><span data-ttu-id="9df0d-103">Назначение политики</span><span class="sxs-lookup"><span data-stu-id="9df0d-103">Assign Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9df0d-104">Назначает [политику](../resources/policy.md) для приложения или участника службы.</span><span class="sxs-lookup"><span data-stu-id="9df0d-104">Assigns a [policy](../resources/policy.md) to an application or service principal.</span></span>

><span data-ttu-id="9df0d-105">Примечание. в настоящее время назначение политики применяется только к политике времени жизни маркеров.</span><span class="sxs-lookup"><span data-stu-id="9df0d-105">Note: Currently, policy assignment only applies to Token lifetime Policy.</span></span> <span data-ttu-id="9df0d-106">Этот тип политики описан в разделе [Политика](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="9df0d-106">This type of policy is described in [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9df0d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9df0d-107">Permissions</span></span>
<span data-ttu-id="9df0d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9df0d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9df0d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9df0d-110">Permission type</span></span>      | <span data-ttu-id="9df0d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9df0d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9df0d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9df0d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9df0d-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9df0d-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9df0d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9df0d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9df0d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9df0d-115">Not supported.</span></span>    |
|<span data-ttu-id="9df0d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9df0d-116">Application</span></span> | <span data-ttu-id="9df0d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9df0d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9df0d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9df0d-118">HTTP request</span></span>

```http
POST /applications/{id}/policies/$ref
POST /serviceprincipals/{id}/policies/$ref
```

> <span data-ttu-id="9df0d-119">Note: "ID" в запросе — это свойство "ID" приложения или субъекта-службы, а не свойство AppID.</span><span class="sxs-lookup"><span data-stu-id="9df0d-119">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9df0d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9df0d-120">Request headers</span></span>
| <span data-ttu-id="9df0d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="9df0d-121">Name</span></span>       | <span data-ttu-id="9df0d-122">Тип</span><span class="sxs-lookup"><span data-stu-id="9df0d-122">Type</span></span> | <span data-ttu-id="9df0d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="9df0d-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9df0d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9df0d-124">Authorization</span></span>  | <span data-ttu-id="9df0d-125">string</span><span class="sxs-lookup"><span data-stu-id="9df0d-125">string</span></span>  | <span data-ttu-id="9df0d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9df0d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9df0d-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9df0d-128">Content-Type</span></span> | <span data-ttu-id="9df0d-129">application/json</span><span class="sxs-lookup"><span data-stu-id="9df0d-129">application/json</span></span>  | <span data-ttu-id="9df0d-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9df0d-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9df0d-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9df0d-132">Request body</span></span>
<span data-ttu-id="9df0d-133">В тексте запроса предоставьте представление объекта политики, который необходимо добавить, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9df0d-133">In the request body, provide a JSON representation of the policy object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="9df0d-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="9df0d-134">Response</span></span>

<span data-ttu-id="9df0d-135">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9df0d-135">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="9df0d-136">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="9df0d-136">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="9df0d-137">Пример</span><span class="sxs-lookup"><span data-stu-id="9df0d-137">Example</span></span>
<span data-ttu-id="9df0d-138">В следующем примере для приложения назначается политика.</span><span class="sxs-lookup"><span data-stu-id="9df0d-138">The following example assigns a policy to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="9df0d-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="9df0d-139">Request</span></span>
<span data-ttu-id="9df0d-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9df0d-140">Here is an example of the request.</span></span>

```http
POST /applications/{id}/policies/$ref
Content-type: application/json
{
    "@odata.id":"https://graph.microsoft.com/beta/policies/{policyid}"
}
```

##### <a name="response"></a><span data-ttu-id="9df0d-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="9df0d-141">Response</span></span>
<span data-ttu-id="9df0d-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9df0d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-assign.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
