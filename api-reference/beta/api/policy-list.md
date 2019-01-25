---
title: Список политик
description: Извлечение всех объектов политики в каталоге.
localization_priority: Normal
ms.openlocfilehash: 292eb457b87629d0034b97b3c781d75adc0da4e8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510024"
---
# <a name="list-policies"></a><span data-ttu-id="89589-103">Список политик</span><span class="sxs-lookup"><span data-stu-id="89589-103">List Policies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89589-104">Извлечение всех объектов [политики](../resources/policy.md) в каталоге.</span><span class="sxs-lookup"><span data-stu-id="89589-104">Retrieve all [policy](../resources/policy.md) objects in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="89589-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="89589-105">Permissions</span></span>
<span data-ttu-id="89589-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89589-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89589-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89589-108">Permission type</span></span>      | <span data-ttu-id="89589-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="89589-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89589-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89589-110">Delegated (work or school account)</span></span> | <span data-ttu-id="89589-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="89589-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="89589-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89589-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89589-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89589-113">Not supported.</span></span>    |
|<span data-ttu-id="89589-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89589-114">Application</span></span> | <span data-ttu-id="89589-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89589-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="89589-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89589-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies
```
## <a name="request-headers"></a><span data-ttu-id="89589-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89589-117">Request headers</span></span>
| <span data-ttu-id="89589-118">Имя</span><span class="sxs-lookup"><span data-stu-id="89589-118">Name</span></span>       | <span data-ttu-id="89589-119">Тип</span><span class="sxs-lookup"><span data-stu-id="89589-119">Type</span></span> | <span data-ttu-id="89589-120">Описание</span><span class="sxs-lookup"><span data-stu-id="89589-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="89589-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="89589-121">Authorization</span></span>  | <span data-ttu-id="89589-122">string</span><span class="sxs-lookup"><span data-stu-id="89589-122">string</span></span>  | <span data-ttu-id="89589-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89589-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89589-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89589-125">Request body</span></span>
<span data-ttu-id="89589-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="89589-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89589-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="89589-127">Response</span></span>

<span data-ttu-id="89589-128">Успешно завершена, этот метод возвращает `200 OK` ответа кода и [политики](../resources/policy.md) объекты в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="89589-128">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="89589-129">В случае неудачи...</span><span class="sxs-lookup"><span data-stu-id="89589-129">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="89589-130">Пример</span><span class="sxs-lookup"><span data-stu-id="89589-130">Example</span></span>
<span data-ttu-id="89589-131">В следующем примере извлекается всех политик.</span><span class="sxs-lookup"><span data-stu-id="89589-131">The following example retrieves all policies.</span></span>

##### <a name="request"></a><span data-ttu-id="89589-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="89589-132">Request</span></span>
<span data-ttu-id="89589-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89589-133">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies
```

##### <a name="response"></a><span data-ttu-id="89589-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="89589-134">Response</span></span>
<span data-ttu-id="89589-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="89589-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
