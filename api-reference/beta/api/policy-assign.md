---
title: Назначение политики
description: Назначает политику для приложения или участника службы.
localization_priority: Normal
ms.openlocfilehash: c690aa85d7471aa6ef5da6d1281dfc679e63a09f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337549"
---
# <a name="assign-policy"></a><span data-ttu-id="c61cf-103">Назначение политики</span><span class="sxs-lookup"><span data-stu-id="c61cf-103">Assign Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c61cf-104">Назначает [политику](../resources/policy.md) для приложения или участника службы.</span><span class="sxs-lookup"><span data-stu-id="c61cf-104">Assigns a [policy](../resources/policy.md) to an application or service principal.</span></span>

><span data-ttu-id="c61cf-105">Примечание. в настоящее время назначение политики применяется только к политике времени жизни маркеров.</span><span class="sxs-lookup"><span data-stu-id="c61cf-105">Note: Currently, policy assignment only applies to Token lifetime Policy.</span></span> <span data-ttu-id="c61cf-106">Этот тип политики описан в разделе [Политика](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="c61cf-106">This type of policy is described in [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c61cf-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c61cf-107">Permissions</span></span>
<span data-ttu-id="c61cf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c61cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c61cf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c61cf-110">Permission type</span></span>      | <span data-ttu-id="c61cf-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c61cf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c61cf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c61cf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c61cf-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c61cf-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c61cf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c61cf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c61cf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c61cf-115">Not supported.</span></span>    |
|<span data-ttu-id="c61cf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c61cf-116">Application</span></span> | <span data-ttu-id="c61cf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c61cf-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c61cf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c61cf-118">HTTP request</span></span>

```http
POST /applications/{id}/policies/$ref
POST /serviceprincipals/{id}/policies/$ref
```

> <span data-ttu-id="c61cf-119">Note: "ID" в запросе — это свойство "ID" приложения или субъекта-службы, а не свойство AppID.</span><span class="sxs-lookup"><span data-stu-id="c61cf-119">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c61cf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c61cf-120">Request headers</span></span>
| <span data-ttu-id="c61cf-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c61cf-121">Name</span></span>       | <span data-ttu-id="c61cf-122">Тип</span><span class="sxs-lookup"><span data-stu-id="c61cf-122">Type</span></span> | <span data-ttu-id="c61cf-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c61cf-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c61cf-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c61cf-124">Authorization</span></span>  | <span data-ttu-id="c61cf-125">string</span><span class="sxs-lookup"><span data-stu-id="c61cf-125">string</span></span>  | <span data-ttu-id="c61cf-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c61cf-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c61cf-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c61cf-128">Content-Type</span></span> | <span data-ttu-id="c61cf-129">application/json</span><span class="sxs-lookup"><span data-stu-id="c61cf-129">application/json</span></span>  | <span data-ttu-id="c61cf-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c61cf-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c61cf-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c61cf-132">Request body</span></span>
<span data-ttu-id="c61cf-133">В тексте запроса предоставьте представление объекта политики, который необходимо добавить, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c61cf-133">In the request body, provide a JSON representation of the policy object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="c61cf-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="c61cf-134">Response</span></span>

<span data-ttu-id="c61cf-135">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c61cf-135">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="c61cf-136">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="c61cf-136">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="c61cf-137">Пример</span><span class="sxs-lookup"><span data-stu-id="c61cf-137">Example</span></span>
<span data-ttu-id="c61cf-138">В следующем примере для приложения назначается политика.</span><span class="sxs-lookup"><span data-stu-id="c61cf-138">The following example assigns a policy to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="c61cf-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c61cf-139">Request</span></span>
<span data-ttu-id="c61cf-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c61cf-140">Here is an example of the request.</span></span>

```http
POST /applications/{id}/policies/$ref
Content-type: application/json
{
    "@odata.id":"https://graph.microsoft.com/beta/policies/{policyid}"
}
```

##### <a name="response"></a><span data-ttu-id="c61cf-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c61cf-141">Response</span></span>
<span data-ttu-id="c61cf-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c61cf-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
