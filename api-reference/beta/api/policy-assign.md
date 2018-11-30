---
title: Назначение политики
description: Назначает политику для приложения или участников-служб.
ms.openlocfilehash: 25dee4ac43716949125795114318d2571d5b8647
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081248"
---
# <a name="assign-policy"></a><span data-ttu-id="35b9f-103">Назначение политики</span><span class="sxs-lookup"><span data-stu-id="35b9f-103">Assign Policy</span></span>

> <span data-ttu-id="35b9f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="35b9f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35b9f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35b9f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="35b9f-106">Назначает [политику](../resources/policy.md) для приложения или участников-служб.</span><span class="sxs-lookup"><span data-stu-id="35b9f-106">Assigns a [policy](../resources/policy.md) to an application or service principal.</span></span>

><span data-ttu-id="35b9f-107">Примечание: В настоящее время назначения политики применяется только к времени жизни маркера политики.</span><span class="sxs-lookup"><span data-stu-id="35b9f-107">Note: Currently, policy assignment only applies to Token lifetime Policy.</span></span> <span data-ttu-id="35b9f-108">Этот тип политики описана в [политике](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="35b9f-108">This type of policy is described in [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="35b9f-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="35b9f-109">Permissions</span></span>
<span data-ttu-id="35b9f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35b9f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35b9f-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35b9f-112">Permission type</span></span>      | <span data-ttu-id="35b9f-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="35b9f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35b9f-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35b9f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="35b9f-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="35b9f-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="35b9f-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35b9f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35b9f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35b9f-117">Not supported.</span></span>    |
|<span data-ttu-id="35b9f-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35b9f-118">Application</span></span> | <span data-ttu-id="35b9f-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35b9f-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="35b9f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35b9f-120">HTTP request</span></span>

```http
POST /applications/{id}/policies/$ref
POST /serviceprincipals/{id}/policies/$ref
```

> <span data-ttu-id="35b9f-121">Примечание: «Код» в запросе является свойство «id» приложения или службы участника, не свойство «appid».</span><span class="sxs-lookup"><span data-stu-id="35b9f-121">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="35b9f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35b9f-122">Request headers</span></span>
| <span data-ttu-id="35b9f-123">Имя</span><span class="sxs-lookup"><span data-stu-id="35b9f-123">Name</span></span>       | <span data-ttu-id="35b9f-124">Тип</span><span class="sxs-lookup"><span data-stu-id="35b9f-124">Type</span></span> | <span data-ttu-id="35b9f-125">Описание</span><span class="sxs-lookup"><span data-stu-id="35b9f-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="35b9f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="35b9f-126">Authorization</span></span>  | <span data-ttu-id="35b9f-127">string</span><span class="sxs-lookup"><span data-stu-id="35b9f-127">string</span></span>  | <span data-ttu-id="35b9f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35b9f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="35b9f-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="35b9f-130">Content-Type</span></span> | <span data-ttu-id="35b9f-131">application/json</span><span class="sxs-lookup"><span data-stu-id="35b9f-131">application/json</span></span>  | <span data-ttu-id="35b9f-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35b9f-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35b9f-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="35b9f-134">Request body</span></span>
<span data-ttu-id="35b9f-135">В тексте запроса для представления JSON добавляемый объект политики.</span><span class="sxs-lookup"><span data-stu-id="35b9f-135">In the request body, provide a JSON representation of the policy object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="35b9f-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="35b9f-136">Response</span></span>

<span data-ttu-id="35b9f-137">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="35b9f-137">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="35b9f-138">В случае неудачи `4xx` будут возвращены с подробные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="35b9f-138">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="35b9f-139">Пример</span><span class="sxs-lookup"><span data-stu-id="35b9f-139">Example</span></span>
<span data-ttu-id="35b9f-140">Следующий пример назначает политику для приложения.</span><span class="sxs-lookup"><span data-stu-id="35b9f-140">The following example assigns a policy to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="35b9f-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="35b9f-141">Request</span></span>
<span data-ttu-id="35b9f-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35b9f-142">Here is an example of the request.</span></span>

```http
POST /applications/{id}/policies/$ref
Content-type: application/json
{
    "@odata.id":"https://graph.microsoft.com/beta/policies/{policyid}"
}
```

##### <a name="response"></a><span data-ttu-id="35b9f-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="35b9f-143">Response</span></span>
<span data-ttu-id="35b9f-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="35b9f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
