---
title: Список политик
description: Извлечение всех объектов политики в каталоге.
localization_priority: Normal
ms.openlocfilehash: ea97146b646068515ab6fdc7fab4b3cefb16031e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836059"
---
# <a name="list-policies"></a><span data-ttu-id="2629f-103">Список политик</span><span class="sxs-lookup"><span data-stu-id="2629f-103">List Policies</span></span>

> <span data-ttu-id="2629f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2629f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2629f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2629f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2629f-106">Извлечение всех объектов [политики](../resources/policy.md) в каталоге.</span><span class="sxs-lookup"><span data-stu-id="2629f-106">Retrieve all [policy](../resources/policy.md) objects in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="2629f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2629f-107">Permissions</span></span>
<span data-ttu-id="2629f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2629f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2629f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2629f-110">Permission type</span></span>      | <span data-ttu-id="2629f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2629f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2629f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2629f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2629f-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2629f-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2629f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2629f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2629f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2629f-115">Not supported.</span></span>    |
|<span data-ttu-id="2629f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2629f-116">Application</span></span> | <span data-ttu-id="2629f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2629f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2629f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2629f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies
```
## <a name="request-headers"></a><span data-ttu-id="2629f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2629f-119">Request headers</span></span>
| <span data-ttu-id="2629f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2629f-120">Name</span></span>       | <span data-ttu-id="2629f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="2629f-121">Type</span></span> | <span data-ttu-id="2629f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2629f-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2629f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2629f-123">Authorization</span></span>  | <span data-ttu-id="2629f-124">string</span><span class="sxs-lookup"><span data-stu-id="2629f-124">string</span></span>  | <span data-ttu-id="2629f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2629f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2629f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2629f-127">Request body</span></span>
<span data-ttu-id="2629f-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2629f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2629f-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="2629f-129">Response</span></span>

<span data-ttu-id="2629f-130">Успешно завершена, этот метод возвращает `200 OK` ответа кода и [политики](../resources/policy.md) объекты в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2629f-130">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="2629f-131">В случае неудачи...</span><span class="sxs-lookup"><span data-stu-id="2629f-131">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="2629f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="2629f-132">Example</span></span>
<span data-ttu-id="2629f-133">В следующем примере извлекается всех политик.</span><span class="sxs-lookup"><span data-stu-id="2629f-133">The following example retrieves all policies.</span></span>

##### <a name="request"></a><span data-ttu-id="2629f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2629f-134">Request</span></span>
<span data-ttu-id="2629f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2629f-135">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies
```

##### <a name="response"></a><span data-ttu-id="2629f-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="2629f-136">Response</span></span>
<span data-ttu-id="2629f-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2629f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "value":[
        {
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
