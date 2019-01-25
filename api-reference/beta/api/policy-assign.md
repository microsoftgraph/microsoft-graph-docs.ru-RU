---
title: Назначение политики
description: Назначает политику для приложения или участников-служб.
localization_priority: Normal
ms.openlocfilehash: 15ba6a42f5c5d39caf57b25ebafc5dd4bc7990fc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528216"
---
# <a name="assign-policy"></a><span data-ttu-id="0c4cc-103">Назначение политики</span><span class="sxs-lookup"><span data-stu-id="0c4cc-103">Assign Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c4cc-104">Назначает [политику](../resources/policy.md) для приложения или участников-служб.</span><span class="sxs-lookup"><span data-stu-id="0c4cc-104">Assigns a [policy](../resources/policy.md) to an application or service principal.</span></span>

><span data-ttu-id="0c4cc-105">Примечание: В настоящее время назначения политики применяется только к времени жизни маркера политики.</span><span class="sxs-lookup"><span data-stu-id="0c4cc-105">Note: Currently, policy assignment only applies to Token lifetime Policy.</span></span> <span data-ttu-id="0c4cc-106">Этот тип политики описана в [политике](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="0c4cc-106">This type of policy is described in [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0c4cc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c4cc-107">Permissions</span></span>
<span data-ttu-id="0c4cc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c4cc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c4cc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c4cc-110">Permission type</span></span>      | <span data-ttu-id="0c4cc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c4cc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c4cc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c4cc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0c4cc-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0c4cc-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0c4cc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c4cc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c4cc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c4cc-115">Not supported.</span></span>    |
|<span data-ttu-id="0c4cc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c4cc-116">Application</span></span> | <span data-ttu-id="0c4cc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c4cc-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c4cc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c4cc-118">HTTP request</span></span>

```http
POST /applications/{id}/policies/$ref
POST /serviceprincipals/{id}/policies/$ref
```

> <span data-ttu-id="0c4cc-119">Примечание: «Код» в запросе является свойство «id» приложения или службы участника, не свойство «appid».</span><span class="sxs-lookup"><span data-stu-id="0c4cc-119">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0c4cc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c4cc-120">Request headers</span></span>
| <span data-ttu-id="0c4cc-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0c4cc-121">Name</span></span>       | <span data-ttu-id="0c4cc-122">Тип</span><span class="sxs-lookup"><span data-stu-id="0c4cc-122">Type</span></span> | <span data-ttu-id="0c4cc-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0c4cc-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0c4cc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c4cc-124">Authorization</span></span>  | <span data-ttu-id="0c4cc-125">string</span><span class="sxs-lookup"><span data-stu-id="0c4cc-125">string</span></span>  | <span data-ttu-id="0c4cc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c4cc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0c4cc-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0c4cc-128">Content-Type</span></span> | <span data-ttu-id="0c4cc-129">application/json</span><span class="sxs-lookup"><span data-stu-id="0c4cc-129">application/json</span></span>  | <span data-ttu-id="0c4cc-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c4cc-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0c4cc-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c4cc-132">Request body</span></span>
<span data-ttu-id="0c4cc-133">В тексте запроса для представления JSON добавляемый объект политики.</span><span class="sxs-lookup"><span data-stu-id="0c4cc-133">In the request body, provide a JSON representation of the policy object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="0c4cc-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="0c4cc-134">Response</span></span>

<span data-ttu-id="0c4cc-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0c4cc-135">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="0c4cc-136">В случае неудачи `4xx` будут возвращены с подробные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="0c4cc-136">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="0c4cc-137">Пример</span><span class="sxs-lookup"><span data-stu-id="0c4cc-137">Example</span></span>
<span data-ttu-id="0c4cc-138">Следующий пример назначает политику для приложения.</span><span class="sxs-lookup"><span data-stu-id="0c4cc-138">The following example assigns a policy to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="0c4cc-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c4cc-139">Request</span></span>
<span data-ttu-id="0c4cc-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c4cc-140">Here is an example of the request.</span></span>

```http
POST /applications/{id}/policies/$ref
Content-type: application/json
{
    "@odata.id":"https://graph.microsoft.com/beta/policies/{policyid}"
}
```

##### <a name="response"></a><span data-ttu-id="0c4cc-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="0c4cc-141">Response</span></span>
<span data-ttu-id="0c4cc-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="0c4cc-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
