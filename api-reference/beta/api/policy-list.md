---
title: Список политик
description: Получение всех объектов Policy в каталоге.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: d7ab2de4944019eff936554cc4da2e0dc15166c2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983455"
---
# <a name="list-policies"></a><span data-ttu-id="68c8b-103">Список политик</span><span class="sxs-lookup"><span data-stu-id="68c8b-103">List Policies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68c8b-104">Получение всех объектов [Policy](../resources/policy.md) в каталоге.</span><span class="sxs-lookup"><span data-stu-id="68c8b-104">Retrieve all [policy](../resources/policy.md) objects in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="68c8b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="68c8b-105">Permissions</span></span>
<span data-ttu-id="68c8b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68c8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68c8b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68c8b-108">Permission type</span></span>      | <span data-ttu-id="68c8b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68c8b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68c8b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68c8b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="68c8b-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="68c8b-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="68c8b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68c8b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68c8b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68c8b-113">Not supported.</span></span>    |
|<span data-ttu-id="68c8b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68c8b-114">Application</span></span> | <span data-ttu-id="68c8b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68c8b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="68c8b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68c8b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies
```
## <a name="request-headers"></a><span data-ttu-id="68c8b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68c8b-117">Request headers</span></span>
| <span data-ttu-id="68c8b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="68c8b-118">Name</span></span>       | <span data-ttu-id="68c8b-119">Тип</span><span class="sxs-lookup"><span data-stu-id="68c8b-119">Type</span></span> | <span data-ttu-id="68c8b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="68c8b-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="68c8b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="68c8b-121">Authorization</span></span>  | <span data-ttu-id="68c8b-122">string</span><span class="sxs-lookup"><span data-stu-id="68c8b-122">string</span></span>  | <span data-ttu-id="68c8b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68c8b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68c8b-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="68c8b-125">Request body</span></span>
<span data-ttu-id="68c8b-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="68c8b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68c8b-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="68c8b-127">Response</span></span>

<span data-ttu-id="68c8b-128">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объекты [политики](../resources/policy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="68c8b-128">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="68c8b-129">В случае неудачного завершения...</span><span class="sxs-lookup"><span data-stu-id="68c8b-129">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="68c8b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="68c8b-130">Example</span></span>
<span data-ttu-id="68c8b-131">В следующем примере извлекаются все политики.</span><span class="sxs-lookup"><span data-stu-id="68c8b-131">The following example retrieves all policies.</span></span>

##### <a name="request"></a><span data-ttu-id="68c8b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="68c8b-132">Request</span></span>
<span data-ttu-id="68c8b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68c8b-133">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies
```

##### <a name="response"></a><span data-ttu-id="68c8b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="68c8b-134">Response</span></span>
<span data-ttu-id="68c8b-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68c8b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
