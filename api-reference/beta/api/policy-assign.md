---
title: Назначение политики
description: Назначает политику для приложения или участника службы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2f005973677ca3e430706a7fced22e5fbf51bcd0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455540"
---
# <a name="assign-policy"></a><span data-ttu-id="8c903-103">Назначение политики</span><span class="sxs-lookup"><span data-stu-id="8c903-103">Assign Policy</span></span>

<span data-ttu-id="8c903-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8c903-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c903-105">Назначает [политику](../resources/policy.md) для приложения или участника службы.</span><span class="sxs-lookup"><span data-stu-id="8c903-105">Assigns a [policy](../resources/policy.md) to an application or service principal.</span></span>

><span data-ttu-id="8c903-106">Примечание. в настоящее время назначение политики применяется только к политике времени жизни маркеров.</span><span class="sxs-lookup"><span data-stu-id="8c903-106">Note: Currently, policy assignment only applies to Token lifetime Policy.</span></span> <span data-ttu-id="8c903-107">Этот тип политики описан в разделе [Политика](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="8c903-107">This type of policy is described in [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8c903-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c903-108">Permissions</span></span>
<span data-ttu-id="8c903-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c903-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c903-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c903-111">Permission type</span></span>      | <span data-ttu-id="8c903-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c903-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c903-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c903-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8c903-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8c903-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8c903-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c903-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c903-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c903-116">Not supported.</span></span>    |
|<span data-ttu-id="8c903-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c903-117">Application</span></span> | <span data-ttu-id="8c903-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c903-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c903-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c903-119">HTTP request</span></span>

```http
POST /applications/{id}/policies/$ref
POST /serviceprincipals/{id}/policies/$ref
```

> <span data-ttu-id="8c903-120">Note: "ID" в запросе — это свойство "ID" приложения или субъекта-службы, а не свойство AppID.</span><span class="sxs-lookup"><span data-stu-id="8c903-120">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c903-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c903-121">Request headers</span></span>
| <span data-ttu-id="8c903-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8c903-122">Name</span></span>       | <span data-ttu-id="8c903-123">Тип</span><span class="sxs-lookup"><span data-stu-id="8c903-123">Type</span></span> | <span data-ttu-id="8c903-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8c903-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8c903-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c903-125">Authorization</span></span>  | <span data-ttu-id="8c903-126">string</span><span class="sxs-lookup"><span data-stu-id="8c903-126">string</span></span>  | <span data-ttu-id="8c903-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c903-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8c903-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8c903-129">Content-Type</span></span> | <span data-ttu-id="8c903-130">application/json</span><span class="sxs-lookup"><span data-stu-id="8c903-130">application/json</span></span>  | <span data-ttu-id="8c903-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c903-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c903-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c903-133">Request body</span></span>
<span data-ttu-id="8c903-134">В тексте запроса предоставьте представление объекта политики, который необходимо добавить, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c903-134">In the request body, provide a JSON representation of the policy object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="8c903-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="8c903-135">Response</span></span>

<span data-ttu-id="8c903-136">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8c903-136">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="8c903-137">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="8c903-137">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="8c903-138">Пример</span><span class="sxs-lookup"><span data-stu-id="8c903-138">Example</span></span>
<span data-ttu-id="8c903-139">В следующем примере для приложения назначается политика.</span><span class="sxs-lookup"><span data-stu-id="8c903-139">The following example assigns a policy to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="8c903-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c903-140">Request</span></span>
<span data-ttu-id="8c903-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c903-141">Here is an example of the request.</span></span>

```http
POST /applications/{id}/policies/$ref
Content-type: application/json
{
    "@odata.id":"https://graph.microsoft.com/beta/policies/{policyid}"
}
```

##### <a name="response"></a><span data-ttu-id="8c903-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c903-142">Response</span></span>
<span data-ttu-id="8c903-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c903-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
