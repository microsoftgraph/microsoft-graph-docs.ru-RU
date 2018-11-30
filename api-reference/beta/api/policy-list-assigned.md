---
title: Список политики, назначенные для приложения или участника-службы
description: Получение объектов политики, назначенных для приложения или участника службы.
ms.openlocfilehash: cfdcf3d8e6709080f4c8f7bfc3e2dbc256789f6f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077347"
---
# <a name="list-policies-assigned-to-application-or-service-principal"></a><span data-ttu-id="440fe-103">Список политики, назначенные для приложения или участника-службы</span><span class="sxs-lookup"><span data-stu-id="440fe-103">List Policies assigned to Application or Service Principal</span></span>

> <span data-ttu-id="440fe-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="440fe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="440fe-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="440fe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="440fe-106">Получение объектов [политики](../resources/policy.md) , назначенных для приложения или участника службы.</span><span class="sxs-lookup"><span data-stu-id="440fe-106">Retrieve the [policy](../resources/policy.md) objects assigned to an application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="440fe-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="440fe-107">Permissions</span></span>
<span data-ttu-id="440fe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="440fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="440fe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="440fe-110">Permission type</span></span>      | <span data-ttu-id="440fe-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="440fe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="440fe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="440fe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="440fe-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="440fe-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="440fe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="440fe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="440fe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="440fe-115">Not supported.</span></span>    |
|<span data-ttu-id="440fe-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="440fe-116">Application</span></span> | <span data-ttu-id="440fe-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="440fe-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="440fe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="440fe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/policies
```

> <span data-ttu-id="440fe-119">Примечание: «Код» в запросе является свойство «id» приложения или службы участника, не свойство «appid».</span><span class="sxs-lookup"><span data-stu-id="440fe-119">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="440fe-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="440fe-120">Request headers</span></span>
| <span data-ttu-id="440fe-121">Имя</span><span class="sxs-lookup"><span data-stu-id="440fe-121">Name</span></span>       | <span data-ttu-id="440fe-122">Тип</span><span class="sxs-lookup"><span data-stu-id="440fe-122">Type</span></span> | <span data-ttu-id="440fe-123">Описание</span><span class="sxs-lookup"><span data-stu-id="440fe-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="440fe-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="440fe-124">Authorization</span></span>  | <span data-ttu-id="440fe-125">string</span><span class="sxs-lookup"><span data-stu-id="440fe-125">string</span></span>  | <span data-ttu-id="440fe-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="440fe-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="440fe-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="440fe-128">Request body</span></span>
<span data-ttu-id="440fe-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="440fe-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="440fe-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="440fe-130">Response</span></span>

<span data-ttu-id="440fe-131">Успешно завершена, этот метод возвращает `200 OK` ответа кода и [политики](../resources/policy.md) объекты в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="440fe-131">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="440fe-132">В случае неудачи `4xx` будут возвращены с подробные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="440fe-132">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="440fe-133">Пример</span><span class="sxs-lookup"><span data-stu-id="440fe-133">Example</span></span>
<span data-ttu-id="440fe-134">В следующем примере извлекается политики, назначенные для приложения.</span><span class="sxs-lookup"><span data-stu-id="440fe-134">The following example retrieves the policies assigned to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="440fe-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="440fe-135">Request</span></span>
<span data-ttu-id="440fe-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="440fe-136">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/applications/{id}/policies
```

##### <a name="response"></a><span data-ttu-id="440fe-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="440fe-137">Response</span></span>
<span data-ttu-id="440fe-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="440fe-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
