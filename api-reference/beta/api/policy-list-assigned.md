---
title: Список политики, назначенные для приложения или участника-службы
description: Получение объектов политики, назначенных для приложения или участника службы.
localization_priority: Normal
ms.openlocfilehash: 1ed39f376b7d090b784f867a59fcb93558bd5f1a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518585"
---
# <a name="list-policies-assigned-to-application-or-service-principal"></a><span data-ttu-id="6c42e-103">Список политики, назначенные для приложения или участника-службы</span><span class="sxs-lookup"><span data-stu-id="6c42e-103">List Policies assigned to Application or Service Principal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c42e-104">Получение объектов [политики](../resources/policy.md) , назначенных для приложения или участника службы.</span><span class="sxs-lookup"><span data-stu-id="6c42e-104">Retrieve the [policy](../resources/policy.md) objects assigned to an application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c42e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c42e-105">Permissions</span></span>
<span data-ttu-id="6c42e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c42e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c42e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c42e-108">Permission type</span></span>      | <span data-ttu-id="6c42e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c42e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c42e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c42e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6c42e-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6c42e-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6c42e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c42e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c42e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c42e-113">Not supported.</span></span>    |
|<span data-ttu-id="6c42e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c42e-114">Application</span></span> | <span data-ttu-id="6c42e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c42e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c42e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c42e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/policies
```

> <span data-ttu-id="6c42e-117">Примечание: «Код» в запросе является свойство «id» приложения или службы участника, не свойство «appid».</span><span class="sxs-lookup"><span data-stu-id="6c42e-117">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c42e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c42e-118">Request headers</span></span>
| <span data-ttu-id="6c42e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6c42e-119">Name</span></span>       | <span data-ttu-id="6c42e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="6c42e-120">Type</span></span> | <span data-ttu-id="6c42e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6c42e-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6c42e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c42e-122">Authorization</span></span>  | <span data-ttu-id="6c42e-123">string</span><span class="sxs-lookup"><span data-stu-id="6c42e-123">string</span></span>  | <span data-ttu-id="6c42e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c42e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c42e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6c42e-126">Request body</span></span>
<span data-ttu-id="6c42e-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6c42e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c42e-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="6c42e-128">Response</span></span>

<span data-ttu-id="6c42e-129">Успешно завершена, этот метод возвращает `200 OK` ответа кода и [политики](../resources/policy.md) объекты в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6c42e-129">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="6c42e-130">В случае неудачи `4xx` будут возвращены с подробные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="6c42e-130">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="6c42e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6c42e-131">Example</span></span>
<span data-ttu-id="6c42e-132">В следующем примере извлекается политики, назначенные для приложения.</span><span class="sxs-lookup"><span data-stu-id="6c42e-132">The following example retrieves the policies assigned to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="6c42e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c42e-133">Request</span></span>
<span data-ttu-id="6c42e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c42e-134">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/applications/{id}/policies
```

##### <a name="response"></a><span data-ttu-id="6c42e-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="6c42e-135">Response</span></span>
<span data-ttu-id="6c42e-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="6c42e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Cache-Control: private
Content-Type: application/json

{
    "value":[
        {
            "@odata.type":"#microsoft.graph.policy",
            "id":"id-value",
            "alternativeIdentifier":null,
            "definition":["policy-definition"],
            "displayName":"name-value",
            "isOrganizationDefault":boolean-value,
            "keyCredentials":[key-credentials],
            "type":"type-value"
        }
    ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-list-assigned.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
