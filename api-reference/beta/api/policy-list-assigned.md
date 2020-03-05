---
title: Список политик, назначенных для приложения или участника службы
description: Получение объектов политики, назначенных приложению или участнику службы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 12e252067c7f7c8672543292a65b8650a43d45c4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455517"
---
# <a name="list-policies-assigned-to-application-or-service-principal"></a><span data-ttu-id="00db5-103">Список политик, назначенных для приложения или участника службы</span><span class="sxs-lookup"><span data-stu-id="00db5-103">List Policies assigned to Application or Service Principal</span></span>

<span data-ttu-id="00db5-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="00db5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00db5-105">Получение объектов [политики](../resources/policy.md) , назначенных приложению или участнику службы.</span><span class="sxs-lookup"><span data-stu-id="00db5-105">Get the [policy](../resources/policy.md) objects assigned to an application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="00db5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="00db5-106">Permissions</span></span>
<span data-ttu-id="00db5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00db5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00db5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00db5-109">Permission type</span></span>      | <span data-ttu-id="00db5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="00db5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00db5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00db5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="00db5-112">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="00db5-112">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="00db5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00db5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00db5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00db5-114">Not supported.</span></span>    |
|<span data-ttu-id="00db5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00db5-115">Application</span></span> | <span data-ttu-id="00db5-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="00db5-116">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="00db5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00db5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/policies
```

> <span data-ttu-id="00db5-118">Note: "ID" в запросе — это свойство "ID" приложения или субъекта-службы, а не свойство AppID.</span><span class="sxs-lookup"><span data-stu-id="00db5-118">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="00db5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00db5-119">Request headers</span></span>
| <span data-ttu-id="00db5-120">Имя</span><span class="sxs-lookup"><span data-stu-id="00db5-120">Name</span></span>       | <span data-ttu-id="00db5-121">Тип</span><span class="sxs-lookup"><span data-stu-id="00db5-121">Type</span></span> | <span data-ttu-id="00db5-122">Описание</span><span class="sxs-lookup"><span data-stu-id="00db5-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="00db5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="00db5-123">Authorization</span></span>  | <span data-ttu-id="00db5-124">string</span><span class="sxs-lookup"><span data-stu-id="00db5-124">string</span></span>  | <span data-ttu-id="00db5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00db5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="00db5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00db5-127">Request body</span></span>
<span data-ttu-id="00db5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="00db5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00db5-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="00db5-129">Response</span></span>

<span data-ttu-id="00db5-130">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объекты [политики](../resources/policy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="00db5-130">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="00db5-131">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="00db5-131">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="00db5-132">Пример</span><span class="sxs-lookup"><span data-stu-id="00db5-132">Example</span></span>
<span data-ttu-id="00db5-133">В следующем примере извлекаются политики, назначенные приложению.</span><span class="sxs-lookup"><span data-stu-id="00db5-133">The following example retrieves the policies assigned to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="00db5-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="00db5-134">Request</span></span>
<span data-ttu-id="00db5-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00db5-135">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/applications/{id}/policies
```

##### <a name="response"></a><span data-ttu-id="00db5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="00db5-136">Response</span></span>
<span data-ttu-id="00db5-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="00db5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
