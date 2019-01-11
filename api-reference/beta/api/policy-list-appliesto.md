---
title: Список приложений и субъектов-служб с определенным политику, назначенную
description: Получение приложения и объекты участников службы с конкретной политикой назначен.
localization_priority: Normal
ms.openlocfilehash: 21a5a9ba4260e306553f53866657a482d814b5f7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875609"
---
# <a name="list-applications-and-service-principals-with-specific-policy-assigned"></a><span data-ttu-id="0d007-103">Список приложений и субъектов-служб с определенным политику, назначенную</span><span class="sxs-lookup"><span data-stu-id="0d007-103">List Applications and Service Principals with specific Policy assigned</span></span>

> <span data-ttu-id="0d007-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0d007-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d007-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d007-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0d007-106">Получение объектов [приложения](../resources/application.md) и [участника службы](../resources/serviceprincipal.md) с конкретной политикой назначен.</span><span class="sxs-lookup"><span data-stu-id="0d007-106">Retrieve the [application](../resources/application.md) and [service principal](../resources/serviceprincipal.md) objects with the specified policy assigned.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d007-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0d007-107">Permissions</span></span>
<span data-ttu-id="0d007-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d007-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d007-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d007-110">Permission type</span></span>      | <span data-ttu-id="0d007-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d007-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d007-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d007-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0d007-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0d007-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0d007-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d007-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d007-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d007-115">Not supported.</span></span>    |
|<span data-ttu-id="0d007-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d007-116">Application</span></span> | <span data-ttu-id="0d007-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d007-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d007-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d007-118">HTTP request</span></span>
```http
GET /policies/{id}/appliesTo
```

## <a name="request-headers"></a><span data-ttu-id="0d007-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d007-119">Request headers</span></span>
| <span data-ttu-id="0d007-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0d007-120">Name</span></span>       | <span data-ttu-id="0d007-121">Тип</span><span class="sxs-lookup"><span data-stu-id="0d007-121">Type</span></span> | <span data-ttu-id="0d007-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0d007-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0d007-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d007-123">Authorization</span></span>  | <span data-ttu-id="0d007-124">string</span><span class="sxs-lookup"><span data-stu-id="0d007-124">string</span></span>  | <span data-ttu-id="0d007-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d007-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d007-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0d007-127">Request body</span></span>
<span data-ttu-id="0d007-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0d007-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d007-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d007-129">Response</span></span>

<span data-ttu-id="0d007-130">Успешно завершена, этот метод возвращает `200 OK` объекты ответа кода и [приложения](../resources/application.md) и [службы участника](../resources/serviceprincipal.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0d007-130">If successful, this method returns `200 OK` response code and [application](../resources/application.md) and [service principal](../resources/serviceprincipal.md) objects in the response body.</span></span> <span data-ttu-id="0d007-131">В случае неудачи `4xx` будут возвращены с подробные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="0d007-131">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="0d007-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0d007-132">Example</span></span>
<span data-ttu-id="0d007-133">В следующем примере извлекается приложений и субъектов-служб с определенным назначена политика.</span><span class="sxs-lookup"><span data-stu-id="0d007-133">The following example retrieves the applications and service principals with a specific policy assigned.</span></span>

##### <a name="request"></a><span data-ttu-id="0d007-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d007-134">Request</span></span>
<span data-ttu-id="0d007-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d007-135">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}/appliesTo
```

##### <a name="response"></a><span data-ttu-id="0d007-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d007-136">Response</span></span>
<span data-ttu-id="0d007-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0d007-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value":[
        {
            "@odata.type"="#microsoft.graph.application",
            "appId":"appId-value",
            "displayName":"displayName-value",
            "errorUrl":"errorUrl-value",
            "groupMembershipClaims":"groupMembershipClaims-value",
            "homepage":"homepage-value",
            "id":"id-value",
            "keyCredentials":[key-credentials],
            "logoutUrl":"logoutUrl-value",
            "replyUrls":["replyUrls-value"]
        }
    ]
}
```
