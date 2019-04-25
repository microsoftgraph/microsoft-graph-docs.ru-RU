---
title: Список приложений и субъектов служб с назначенной определенной политикой
description: Получение объектов приложения и субъекта службы с указанной политикой.
localization_priority: Normal
ms.openlocfilehash: d7449428216a2e68d9ab8bb8399ca0e8dc4b72fd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538755"
---
# <a name="list-applications-and-service-principals-with-specific-policy-assigned"></a><span data-ttu-id="ced25-103">Список приложений и субъектов служб с назначенной определенной политикой</span><span class="sxs-lookup"><span data-stu-id="ced25-103">List Applications and Service Principals with specific Policy assigned</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ced25-104">Получение объектов [приложения](../resources/application.md) и [субъекта службы](../resources/serviceprincipal.md) с указанной политикой.</span><span class="sxs-lookup"><span data-stu-id="ced25-104">Retrieve the [application](../resources/application.md) and [service principal](../resources/serviceprincipal.md) objects with the specified policy assigned.</span></span>

## <a name="permissions"></a><span data-ttu-id="ced25-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ced25-105">Permissions</span></span>
<span data-ttu-id="ced25-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ced25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ced25-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ced25-108">Permission type</span></span>      | <span data-ttu-id="ced25-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ced25-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ced25-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ced25-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ced25-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ced25-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ced25-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ced25-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ced25-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ced25-113">Not supported.</span></span>    |
|<span data-ttu-id="ced25-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ced25-114">Application</span></span> | <span data-ttu-id="ced25-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ced25-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ced25-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ced25-116">HTTP request</span></span>
```http
GET /policies/{id}/appliesTo
```

## <a name="request-headers"></a><span data-ttu-id="ced25-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ced25-117">Request headers</span></span>
| <span data-ttu-id="ced25-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ced25-118">Name</span></span>       | <span data-ttu-id="ced25-119">Тип</span><span class="sxs-lookup"><span data-stu-id="ced25-119">Type</span></span> | <span data-ttu-id="ced25-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ced25-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ced25-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ced25-121">Authorization</span></span>  | <span data-ttu-id="ced25-122">string</span><span class="sxs-lookup"><span data-stu-id="ced25-122">string</span></span>  | <span data-ttu-id="ced25-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ced25-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ced25-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ced25-125">Request body</span></span>
<span data-ttu-id="ced25-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ced25-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ced25-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="ced25-127">Response</span></span>

<span data-ttu-id="ced25-128">В случае успеха этот метод возвращает `200 OK` код отклика и объекты [приложения](../resources/application.md) и [участника службы](../resources/serviceprincipal.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ced25-128">If successful, this method returns `200 OK` response code and [application](../resources/application.md) and [service principal](../resources/serviceprincipal.md) objects in the response body.</span></span> <span data-ttu-id="ced25-129">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="ced25-129">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="ced25-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ced25-130">Example</span></span>
<span data-ttu-id="ced25-131">В следующем примере извлекаются приложения и субъекты служб с назначенной определенной политикой.</span><span class="sxs-lookup"><span data-stu-id="ced25-131">The following example retrieves the applications and service principals with a specific policy assigned.</span></span>

##### <a name="request"></a><span data-ttu-id="ced25-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ced25-132">Request</span></span>
<span data-ttu-id="ced25-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ced25-133">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}/appliesTo
```

##### <a name="response"></a><span data-ttu-id="ced25-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ced25-134">Response</span></span>
<span data-ttu-id="ced25-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ced25-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-list-appliesto.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
