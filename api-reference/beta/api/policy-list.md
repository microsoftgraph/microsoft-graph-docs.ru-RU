---
title: Список политик
description: Получение всех объектов Policy в каталоге.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: dkershaw10
ms.openlocfilehash: 9af05ec8655f3b8561352596f62c9dbedd270ca2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43408350"
---
# <a name="list-policies"></a><span data-ttu-id="1e245-103">Список политик</span><span class="sxs-lookup"><span data-stu-id="1e245-103">List Policies</span></span>

<span data-ttu-id="1e245-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e245-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e245-105">Получение всех объектов [Policy](../resources/policy.md) в каталоге.</span><span class="sxs-lookup"><span data-stu-id="1e245-105">Get all [policy](../resources/policy.md) objects in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e245-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1e245-106">Permissions</span></span>
<span data-ttu-id="1e245-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e245-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e245-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e245-109">Permission type</span></span>      | <span data-ttu-id="1e245-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e245-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e245-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e245-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1e245-112">Policy. Read. ALL, Directory. Read. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="1e245-112">Policy.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1e245-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e245-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e245-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e245-114">Not supported.</span></span>    |
|<span data-ttu-id="1e245-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="1e245-115">Application</span></span> | <span data-ttu-id="1e245-116">Policy. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="1e245-116">Policy.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e245-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e245-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies
```
## <a name="request-headers"></a><span data-ttu-id="1e245-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1e245-118">Request headers</span></span>
| <span data-ttu-id="1e245-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1e245-119">Name</span></span>       | <span data-ttu-id="1e245-120">Тип</span><span class="sxs-lookup"><span data-stu-id="1e245-120">Type</span></span> | <span data-ttu-id="1e245-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1e245-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1e245-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e245-122">Authorization</span></span>  | <span data-ttu-id="1e245-123">string</span><span class="sxs-lookup"><span data-stu-id="1e245-123">string</span></span>  | <span data-ttu-id="1e245-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e245-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e245-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1e245-126">Request body</span></span>
<span data-ttu-id="1e245-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1e245-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e245-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="1e245-128">Response</span></span>

<span data-ttu-id="1e245-129">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объекты [политики](../resources/policy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1e245-129">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="1e245-130">В случае неудачного завершения...</span><span class="sxs-lookup"><span data-stu-id="1e245-130">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="1e245-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1e245-131">Example</span></span>
<span data-ttu-id="1e245-132">В следующем примере извлекаются все политики.</span><span class="sxs-lookup"><span data-stu-id="1e245-132">The following example retrieves all policies.</span></span>

##### <a name="request"></a><span data-ttu-id="1e245-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e245-133">Request</span></span>
<span data-ttu-id="1e245-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1e245-134">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies
```

##### <a name="response"></a><span data-ttu-id="1e245-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e245-135">Response</span></span>
<span data-ttu-id="1e245-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1e245-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
