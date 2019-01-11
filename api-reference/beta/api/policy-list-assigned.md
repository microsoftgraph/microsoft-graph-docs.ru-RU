---
title: Список политики, назначенные для приложения или участника-службы
description: Получение объектов политики, назначенных для приложения или участника службы.
localization_priority: Normal
ms.openlocfilehash: 3c66eece645313f7039f12aec708cba4581fb4bb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875357"
---
# <a name="list-policies-assigned-to-application-or-service-principal"></a><span data-ttu-id="1d28d-103">Список политики, назначенные для приложения или участника-службы</span><span class="sxs-lookup"><span data-stu-id="1d28d-103">List Policies assigned to Application or Service Principal</span></span>

> <span data-ttu-id="1d28d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1d28d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d28d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d28d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1d28d-106">Получение объектов [политики](../resources/policy.md) , назначенных для приложения или участника службы.</span><span class="sxs-lookup"><span data-stu-id="1d28d-106">Retrieve the [policy](../resources/policy.md) objects assigned to an application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d28d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1d28d-107">Permissions</span></span>
<span data-ttu-id="1d28d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d28d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d28d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d28d-110">Permission type</span></span>      | <span data-ttu-id="1d28d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d28d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d28d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d28d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1d28d-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1d28d-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1d28d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d28d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d28d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d28d-115">Not supported.</span></span>    |
|<span data-ttu-id="1d28d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d28d-116">Application</span></span> | <span data-ttu-id="1d28d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d28d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d28d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d28d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/policies
```

> <span data-ttu-id="1d28d-119">Примечание: «Код» в запросе является свойство «id» приложения или службы участника, не свойство «appid».</span><span class="sxs-lookup"><span data-stu-id="1d28d-119">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1d28d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d28d-120">Request headers</span></span>
| <span data-ttu-id="1d28d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1d28d-121">Name</span></span>       | <span data-ttu-id="1d28d-122">Тип</span><span class="sxs-lookup"><span data-stu-id="1d28d-122">Type</span></span> | <span data-ttu-id="1d28d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1d28d-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1d28d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d28d-124">Authorization</span></span>  | <span data-ttu-id="1d28d-125">string</span><span class="sxs-lookup"><span data-stu-id="1d28d-125">string</span></span>  | <span data-ttu-id="1d28d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d28d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d28d-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1d28d-128">Request body</span></span>
<span data-ttu-id="1d28d-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1d28d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d28d-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d28d-130">Response</span></span>

<span data-ttu-id="1d28d-131">Успешно завершена, этот метод возвращает `200 OK` ответа кода и [политики](../resources/policy.md) объекты в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1d28d-131">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="1d28d-132">В случае неудачи `4xx` будут возвращены с подробные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="1d28d-132">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="1d28d-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1d28d-133">Example</span></span>
<span data-ttu-id="1d28d-134">В следующем примере извлекается политики, назначенные для приложения.</span><span class="sxs-lookup"><span data-stu-id="1d28d-134">The following example retrieves the policies assigned to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="1d28d-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d28d-135">Request</span></span>
<span data-ttu-id="1d28d-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d28d-136">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/applications/{id}/policies
```

##### <a name="response"></a><span data-ttu-id="1d28d-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d28d-137">Response</span></span>
<span data-ttu-id="1d28d-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1d28d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
