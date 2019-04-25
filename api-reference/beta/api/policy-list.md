---
title: Список политик
description: Получение всех объектов Policy в каталоге.
localization_priority: Normal
ms.openlocfilehash: 292eb457b87629d0034b97b3c781d75adc0da4e8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538713"
---
# <a name="list-policies"></a><span data-ttu-id="a8f9d-103">Список политик</span><span class="sxs-lookup"><span data-stu-id="a8f9d-103">List Policies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8f9d-104">Получение всех объектов [Policy](../resources/policy.md) в каталоге.</span><span class="sxs-lookup"><span data-stu-id="a8f9d-104">Retrieve all [policy](../resources/policy.md) objects in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8f9d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a8f9d-105">Permissions</span></span>
<span data-ttu-id="a8f9d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8f9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8f9d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8f9d-108">Permission type</span></span>      | <span data-ttu-id="a8f9d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8f9d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8f9d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8f9d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a8f9d-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a8f9d-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a8f9d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8f9d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8f9d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8f9d-113">Not supported.</span></span>    |
|<span data-ttu-id="a8f9d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8f9d-114">Application</span></span> | <span data-ttu-id="a8f9d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8f9d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8f9d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8f9d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies
```
## <a name="request-headers"></a><span data-ttu-id="a8f9d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8f9d-117">Request headers</span></span>
| <span data-ttu-id="a8f9d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a8f9d-118">Name</span></span>       | <span data-ttu-id="a8f9d-119">Тип</span><span class="sxs-lookup"><span data-stu-id="a8f9d-119">Type</span></span> | <span data-ttu-id="a8f9d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a8f9d-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a8f9d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8f9d-121">Authorization</span></span>  | <span data-ttu-id="a8f9d-122">string</span><span class="sxs-lookup"><span data-stu-id="a8f9d-122">string</span></span>  | <span data-ttu-id="a8f9d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8f9d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8f9d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a8f9d-125">Request body</span></span>
<span data-ttu-id="a8f9d-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a8f9d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8f9d-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8f9d-127">Response</span></span>

<span data-ttu-id="a8f9d-128">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объекты [политики](../resources/policy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a8f9d-128">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="a8f9d-129">В случае неудачного завершения...</span><span class="sxs-lookup"><span data-stu-id="a8f9d-129">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="a8f9d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a8f9d-130">Example</span></span>
<span data-ttu-id="a8f9d-131">В следующем примере извлекаются все политики.</span><span class="sxs-lookup"><span data-stu-id="a8f9d-131">The following example retrieves all policies.</span></span>

##### <a name="request"></a><span data-ttu-id="a8f9d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8f9d-132">Request</span></span>
<span data-ttu-id="a8f9d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8f9d-133">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies
```

##### <a name="response"></a><span data-ttu-id="a8f9d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8f9d-134">Response</span></span>
<span data-ttu-id="a8f9d-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a8f9d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
