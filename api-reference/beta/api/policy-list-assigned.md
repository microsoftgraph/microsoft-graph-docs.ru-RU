---
title: Список политик, назначенных для приложения или участника службы
description: Получение объектов политики, назначенных приложению или участнику службы.
localization_priority: Normal
ms.openlocfilehash: 24833a42a8b3df2dfde6894cbcdae89a20c6e1cc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332228"
---
# <a name="list-policies-assigned-to-application-or-service-principal"></a><span data-ttu-id="90a15-103">Список политик, назначенных для приложения или участника службы</span><span class="sxs-lookup"><span data-stu-id="90a15-103">List Policies assigned to Application or Service Principal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90a15-104">Получение объектов [политики](../resources/policy.md) , назначенных приложению или участнику службы.</span><span class="sxs-lookup"><span data-stu-id="90a15-104">Retrieve the [policy](../resources/policy.md) objects assigned to an application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="90a15-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90a15-105">Permissions</span></span>
<span data-ttu-id="90a15-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90a15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90a15-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90a15-108">Permission type</span></span>      | <span data-ttu-id="90a15-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90a15-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90a15-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90a15-110">Delegated (work or school account)</span></span> | <span data-ttu-id="90a15-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="90a15-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="90a15-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90a15-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90a15-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90a15-113">Not supported.</span></span>    |
|<span data-ttu-id="90a15-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90a15-114">Application</span></span> | <span data-ttu-id="90a15-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90a15-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="90a15-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90a15-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/policies
```

> <span data-ttu-id="90a15-117">Note: "ID" в запросе — это свойство "ID" приложения или субъекта-службы, а не свойство AppID.</span><span class="sxs-lookup"><span data-stu-id="90a15-117">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="90a15-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90a15-118">Request headers</span></span>
| <span data-ttu-id="90a15-119">Имя</span><span class="sxs-lookup"><span data-stu-id="90a15-119">Name</span></span>       | <span data-ttu-id="90a15-120">Тип</span><span class="sxs-lookup"><span data-stu-id="90a15-120">Type</span></span> | <span data-ttu-id="90a15-121">Описание</span><span class="sxs-lookup"><span data-stu-id="90a15-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="90a15-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="90a15-122">Authorization</span></span>  | <span data-ttu-id="90a15-123">string</span><span class="sxs-lookup"><span data-stu-id="90a15-123">string</span></span>  | <span data-ttu-id="90a15-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90a15-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90a15-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90a15-126">Request body</span></span>
<span data-ttu-id="90a15-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90a15-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90a15-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="90a15-128">Response</span></span>

<span data-ttu-id="90a15-129">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объекты [политики](../resources/policy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="90a15-129">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="90a15-130">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="90a15-130">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="90a15-131">Пример</span><span class="sxs-lookup"><span data-stu-id="90a15-131">Example</span></span>
<span data-ttu-id="90a15-132">В следующем примере извлекаются политики, назначенные приложению.</span><span class="sxs-lookup"><span data-stu-id="90a15-132">The following example retrieves the policies assigned to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="90a15-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="90a15-133">Request</span></span>
<span data-ttu-id="90a15-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90a15-134">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/applications/{id}/policies
```

##### <a name="response"></a><span data-ttu-id="90a15-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="90a15-135">Response</span></span>
<span data-ttu-id="90a15-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90a15-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
