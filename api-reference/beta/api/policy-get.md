---
title: Получение политики
description: Получение свойств политики.
localization_priority: Normal
ms.openlocfilehash: c2ef94c48e2b55f39cc812b9c2e3479a3352a6e6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526741"
---
# <a name="get-policy"></a><span data-ttu-id="41ac2-103">Получение политики</span><span class="sxs-lookup"><span data-stu-id="41ac2-103">Get Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41ac2-104">Получение свойств [политики](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="41ac2-104">Retrieve the properties of a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="41ac2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41ac2-105">Permissions</span></span>
<span data-ttu-id="41ac2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41ac2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41ac2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41ac2-108">Permission type</span></span>      | <span data-ttu-id="41ac2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="41ac2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41ac2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41ac2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="41ac2-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="41ac2-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="41ac2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41ac2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41ac2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41ac2-113">Not supported.</span></span>    |
|<span data-ttu-id="41ac2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41ac2-114">Application</span></span> | <span data-ttu-id="41ac2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41ac2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="41ac2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41ac2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="41ac2-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41ac2-117">Request headers</span></span>
| <span data-ttu-id="41ac2-118">Имя</span><span class="sxs-lookup"><span data-stu-id="41ac2-118">Name</span></span>       | <span data-ttu-id="41ac2-119">Тип</span><span class="sxs-lookup"><span data-stu-id="41ac2-119">Type</span></span> | <span data-ttu-id="41ac2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="41ac2-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="41ac2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="41ac2-121">Authorization</span></span>  | <span data-ttu-id="41ac2-122">string</span><span class="sxs-lookup"><span data-stu-id="41ac2-122">string</span></span>  | <span data-ttu-id="41ac2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41ac2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41ac2-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="41ac2-125">Request body</span></span>
<span data-ttu-id="41ac2-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="41ac2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41ac2-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="41ac2-127">Response</span></span>

<span data-ttu-id="41ac2-128">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [политики](../resources/policy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="41ac2-128">If successful, this method returns `200 OK` response code and a [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="41ac2-129">Если unsucccessful...</span><span class="sxs-lookup"><span data-stu-id="41ac2-129">If unsucccessful...</span></span>

## <a name="example"></a><span data-ttu-id="41ac2-130">Пример</span><span class="sxs-lookup"><span data-stu-id="41ac2-130">Example</span></span>
<span data-ttu-id="41ac2-131">В следующем примере извлекается определенной политики.</span><span class="sxs-lookup"><span data-stu-id="41ac2-131">The following example retrieves a specific policy.</span></span>

##### <a name="request"></a><span data-ttu-id="41ac2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="41ac2-132">Request</span></span>
<span data-ttu-id="41ac2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41ac2-133">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="41ac2-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="41ac2-134">Response</span></span>
<span data-ttu-id="41ac2-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="41ac2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#policies/$entity",
    "id":"id-value",
    "alternativeIdentifier":null,
    "definition":["policy-definition"],
    "displayName":"name-value",
    "isOrganizationDefault":boolean-value,
    "keyCredentials":[key-credentials],
    "type":"type-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
