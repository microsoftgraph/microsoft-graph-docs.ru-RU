---
title: Список политик, назначенных для приложения или участника службы
description: Получение объектов политики, назначенных приложению или участнику службы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: dkershaw10
ms.openlocfilehash: 6aa20deefa63325bf369fc2c59db97add4732569
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289709"
---
# <a name="list-policies-assigned-to-application-or-service-principal"></a><span data-ttu-id="29d39-103">Список политик, назначенных для приложения или участника службы</span><span class="sxs-lookup"><span data-stu-id="29d39-103">List Policies assigned to Application or Service Principal</span></span>

<span data-ttu-id="29d39-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29d39-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29d39-105">Получение объектов [политики](../resources/policy.md) , назначенных приложению или участнику службы.</span><span class="sxs-lookup"><span data-stu-id="29d39-105">Get the [policy](../resources/policy.md) objects assigned to an application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="29d39-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="29d39-106">Permissions</span></span>
<span data-ttu-id="29d39-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29d39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29d39-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29d39-109">Permission type</span></span>      | <span data-ttu-id="29d39-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="29d39-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29d39-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29d39-111">Delegated (work or school account)</span></span> | <span data-ttu-id="29d39-112">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="29d39-112">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="29d39-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29d39-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29d39-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29d39-114">Not supported.</span></span>    |
|<span data-ttu-id="29d39-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29d39-115">Application</span></span> | <span data-ttu-id="29d39-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="29d39-116">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29d39-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29d39-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/policies
```

> <span data-ttu-id="29d39-118">Note: "ID" в запросе — это свойство "ID" приложения или субъекта-службы, а не свойство AppID.</span><span class="sxs-lookup"><span data-stu-id="29d39-118">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="29d39-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="29d39-119">Request headers</span></span>
| <span data-ttu-id="29d39-120">Имя</span><span class="sxs-lookup"><span data-stu-id="29d39-120">Name</span></span>           | <span data-ttu-id="29d39-121">Описание</span><span class="sxs-lookup"><span data-stu-id="29d39-121">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="29d39-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="29d39-122">Authorization</span></span>  | <span data-ttu-id="29d39-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29d39-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="29d39-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="29d39-125">Request body</span></span>
<span data-ttu-id="29d39-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="29d39-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29d39-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="29d39-127">Response</span></span>

<span data-ttu-id="29d39-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объекты [политики](../resources/policy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="29d39-128">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="29d39-129">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="29d39-129">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="29d39-130">Пример</span><span class="sxs-lookup"><span data-stu-id="29d39-130">Example</span></span>
<span data-ttu-id="29d39-131">В следующем примере извлекаются политики, назначенные приложению.</span><span class="sxs-lookup"><span data-stu-id="29d39-131">The following example retrieves the policies assigned to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="29d39-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="29d39-132">Request</span></span>
<span data-ttu-id="29d39-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="29d39-133">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/applications/{id}/policies
```

##### <a name="response"></a><span data-ttu-id="29d39-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="29d39-134">Response</span></span>
<span data-ttu-id="29d39-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="29d39-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
