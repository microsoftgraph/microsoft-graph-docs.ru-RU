---
title: Список приложений и субъектов служб с назначенной определенной политикой
description: Получение объектов приложения и субъекта службы с указанной политикой.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 7959f8b286f1068de454f6d0d36a182f190efafd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455524"
---
# <a name="list-applications-and-service-principals-with-specific-policy-assigned"></a><span data-ttu-id="33a0b-103">Список приложений и субъектов служб с назначенной определенной политикой</span><span class="sxs-lookup"><span data-stu-id="33a0b-103">List applications and service principals with specific policy assigned</span></span>

<span data-ttu-id="33a0b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="33a0b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33a0b-105">Получение объектов [приложения](../resources/application.md) и [субъекта службы](../resources/serviceprincipal.md) с указанной политикой.</span><span class="sxs-lookup"><span data-stu-id="33a0b-105">Get the [application](../resources/application.md) and [service principal](../resources/serviceprincipal.md) objects with the specified policy assigned.</span></span>

## <a name="permissions"></a><span data-ttu-id="33a0b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="33a0b-106">Permissions</span></span>
<span data-ttu-id="33a0b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33a0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33a0b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33a0b-109">Permission type</span></span>      | <span data-ttu-id="33a0b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="33a0b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33a0b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33a0b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="33a0b-112">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="33a0b-112">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="33a0b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33a0b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33a0b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33a0b-114">Not supported.</span></span>    |
|<span data-ttu-id="33a0b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33a0b-115">Application</span></span> | <span data-ttu-id="33a0b-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="33a0b-116">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33a0b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33a0b-117">HTTP request</span></span>
```http
GET /policies/{id}/appliesTo
```

## <a name="request-headers"></a><span data-ttu-id="33a0b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33a0b-118">Request headers</span></span>
| <span data-ttu-id="33a0b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="33a0b-119">Name</span></span>       | <span data-ttu-id="33a0b-120">Тип</span><span class="sxs-lookup"><span data-stu-id="33a0b-120">Type</span></span> | <span data-ttu-id="33a0b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="33a0b-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="33a0b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="33a0b-122">Authorization</span></span>  | <span data-ttu-id="33a0b-123">string</span><span class="sxs-lookup"><span data-stu-id="33a0b-123">string</span></span>  | <span data-ttu-id="33a0b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33a0b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33a0b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="33a0b-126">Request body</span></span>
<span data-ttu-id="33a0b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="33a0b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33a0b-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="33a0b-128">Response</span></span>

<span data-ttu-id="33a0b-129">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объекты [Application](../resources/application.md) и [servicePrincipal](../resources/serviceprincipal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="33a0b-129">If successful, this method returns `200 OK` response code and [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span> <span data-ttu-id="33a0b-130">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="33a0b-130">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="33a0b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="33a0b-131">Example</span></span>
<span data-ttu-id="33a0b-132">В следующем примере извлекаются приложения и субъекты служб с назначенной определенной политикой.</span><span class="sxs-lookup"><span data-stu-id="33a0b-132">The following example retrieves the applications and service principals with a specific policy assigned.</span></span>

##### <a name="request"></a><span data-ttu-id="33a0b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="33a0b-133">Request</span></span>
<span data-ttu-id="33a0b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33a0b-134">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}/appliesTo
```

##### <a name="response"></a><span data-ttu-id="33a0b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="33a0b-135">Response</span></span>
<span data-ttu-id="33a0b-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="33a0b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
