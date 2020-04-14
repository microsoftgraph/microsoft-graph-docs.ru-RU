---
title: Список приложений и субъектов служб с назначенной определенной политикой
description: Получение объектов приложения и субъекта службы с указанной политикой.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: dkershaw10
ms.openlocfilehash: 07d7a8cd1029de5205b1b2332d70bae868e6d614
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450874"
---
# <a name="list-applications-and-service-principals-with-specific-policy-assigned"></a><span data-ttu-id="9fc23-103">Список приложений и субъектов служб с назначенной определенной политикой</span><span class="sxs-lookup"><span data-stu-id="9fc23-103">List applications and service principals with specific policy assigned</span></span>

<span data-ttu-id="9fc23-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fc23-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fc23-105">Получение объектов [приложения](../resources/application.md) и [субъекта службы](../resources/serviceprincipal.md) с указанной политикой.</span><span class="sxs-lookup"><span data-stu-id="9fc23-105">Get the [application](../resources/application.md) and [service principal](../resources/serviceprincipal.md) objects with the specified policy assigned.</span></span>

## <a name="permissions"></a><span data-ttu-id="9fc23-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9fc23-106">Permissions</span></span>
<span data-ttu-id="9fc23-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fc23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fc23-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9fc23-109">Permission type</span></span>      | <span data-ttu-id="9fc23-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9fc23-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fc23-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9fc23-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9fc23-112">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9fc23-112">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9fc23-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9fc23-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fc23-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fc23-114">Not supported.</span></span>    |
|<span data-ttu-id="9fc23-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9fc23-115">Application</span></span> | <span data-ttu-id="9fc23-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fc23-116">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9fc23-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9fc23-117">HTTP request</span></span>
```http
GET /policies/{id}/appliesTo
```

## <a name="request-headers"></a><span data-ttu-id="9fc23-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9fc23-118">Request headers</span></span>
| <span data-ttu-id="9fc23-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9fc23-119">Name</span></span>       | <span data-ttu-id="9fc23-120">Тип</span><span class="sxs-lookup"><span data-stu-id="9fc23-120">Type</span></span> | <span data-ttu-id="9fc23-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9fc23-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9fc23-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fc23-122">Authorization</span></span>  | <span data-ttu-id="9fc23-123">string</span><span class="sxs-lookup"><span data-stu-id="9fc23-123">string</span></span>  | <span data-ttu-id="9fc23-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9fc23-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9fc23-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9fc23-126">Request body</span></span>
<span data-ttu-id="9fc23-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9fc23-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9fc23-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="9fc23-128">Response</span></span>

<span data-ttu-id="9fc23-129">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объекты [Application](../resources/application.md) и [servicePrincipal](../resources/serviceprincipal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9fc23-129">If successful, this method returns `200 OK` response code and [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span> <span data-ttu-id="9fc23-130">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="9fc23-130">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="9fc23-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9fc23-131">Example</span></span>
<span data-ttu-id="9fc23-132">В следующем примере извлекаются приложения и субъекты служб с назначенной определенной политикой.</span><span class="sxs-lookup"><span data-stu-id="9fc23-132">The following example retrieves the applications and service principals with a specific policy assigned.</span></span>

##### <a name="request"></a><span data-ttu-id="9fc23-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9fc23-133">Request</span></span>
<span data-ttu-id="9fc23-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9fc23-134">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}/appliesTo
```

##### <a name="response"></a><span data-ttu-id="9fc23-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fc23-135">Response</span></span>
<span data-ttu-id="9fc23-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9fc23-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
