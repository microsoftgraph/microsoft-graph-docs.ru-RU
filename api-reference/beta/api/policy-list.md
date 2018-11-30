---
title: Список политик
description: Извлечение всех объектов политики в каталоге.
ms.openlocfilehash: 5abff0973a53dc3bddfd256dbc43faad519e20e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081942"
---
# <a name="list-policies"></a><span data-ttu-id="77ae5-103">Список политик</span><span class="sxs-lookup"><span data-stu-id="77ae5-103">List Policies</span></span>

> <span data-ttu-id="77ae5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="77ae5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77ae5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77ae5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="77ae5-106">Извлечение всех объектов [политики](../resources/policy.md) в каталоге.</span><span class="sxs-lookup"><span data-stu-id="77ae5-106">Retrieve all [policy](../resources/policy.md) objects in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="77ae5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="77ae5-107">Permissions</span></span>
<span data-ttu-id="77ae5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77ae5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77ae5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77ae5-110">Permission type</span></span>      | <span data-ttu-id="77ae5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77ae5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77ae5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77ae5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="77ae5-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="77ae5-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="77ae5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77ae5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77ae5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77ae5-115">Not supported.</span></span>    |
|<span data-ttu-id="77ae5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77ae5-116">Application</span></span> | <span data-ttu-id="77ae5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77ae5-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="77ae5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77ae5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies
```
## <a name="request-headers"></a><span data-ttu-id="77ae5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77ae5-119">Request headers</span></span>
| <span data-ttu-id="77ae5-120">Имя</span><span class="sxs-lookup"><span data-stu-id="77ae5-120">Name</span></span>       | <span data-ttu-id="77ae5-121">Тип</span><span class="sxs-lookup"><span data-stu-id="77ae5-121">Type</span></span> | <span data-ttu-id="77ae5-122">Описание</span><span class="sxs-lookup"><span data-stu-id="77ae5-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="77ae5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="77ae5-123">Authorization</span></span>  | <span data-ttu-id="77ae5-124">string</span><span class="sxs-lookup"><span data-stu-id="77ae5-124">string</span></span>  | <span data-ttu-id="77ae5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77ae5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="77ae5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77ae5-127">Request body</span></span>
<span data-ttu-id="77ae5-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="77ae5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77ae5-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="77ae5-129">Response</span></span>

<span data-ttu-id="77ae5-130">Успешно завершена, этот метод возвращает `200 OK` ответа кода и [политики](../resources/policy.md) объекты в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="77ae5-130">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="77ae5-131">В случае неудачи...</span><span class="sxs-lookup"><span data-stu-id="77ae5-131">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="77ae5-132">Пример</span><span class="sxs-lookup"><span data-stu-id="77ae5-132">Example</span></span>
<span data-ttu-id="77ae5-133">В следующем примере извлекается всех политик.</span><span class="sxs-lookup"><span data-stu-id="77ae5-133">The following example retrieves all policies.</span></span>

##### <a name="request"></a><span data-ttu-id="77ae5-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="77ae5-134">Request</span></span>
<span data-ttu-id="77ae5-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77ae5-135">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies
```

##### <a name="response"></a><span data-ttu-id="77ae5-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="77ae5-136">Response</span></span>
<span data-ttu-id="77ae5-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="77ae5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
