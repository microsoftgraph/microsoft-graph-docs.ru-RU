---
title: 'domain: verify'
description: Проверка права собственности на домен.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c4289e6c67844238460be9e706b8ff2f51c55035
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519159"
---
# <a name="domain-verify"></a><span data-ttu-id="19ff0-103">domain: verify</span><span class="sxs-lookup"><span data-stu-id="19ff0-103">domain: verify</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19ff0-104">Проверка права собственности на домен.</span><span class="sxs-lookup"><span data-stu-id="19ff0-104">Validates the ownership of the domain.</span></span>

> <span data-ttu-id="19ff0-p101">**Важно!** Применяется только к непроверенному домену. Для непроверенного домена свойство isVerified объекта [domain](../resources/domain.md) будет иметь значение false.</span><span class="sxs-lookup"><span data-stu-id="19ff0-p101">**Important:** Only applies to an unverified domain. For an unverified domain, the isVerified property of the [domain](../resources/domain.md) is false.</span></span>

## <a name="permissions"></a><span data-ttu-id="19ff0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="19ff0-107">Permissions</span></span>

<span data-ttu-id="19ff0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19ff0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="19ff0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19ff0-110">Permission type</span></span>      | <span data-ttu-id="19ff0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="19ff0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19ff0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19ff0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="19ff0-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="19ff0-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="19ff0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19ff0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19ff0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19ff0-115">Not supported.</span></span>    |
|<span data-ttu-id="19ff0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19ff0-116">Application</span></span> | <span data-ttu-id="19ff0-117">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19ff0-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="19ff0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19ff0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> <span data-ttu-id="19ff0-119">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="19ff0-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19ff0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19ff0-120">Request headers</span></span>

| <span data-ttu-id="19ff0-121">Имя</span><span class="sxs-lookup"><span data-stu-id="19ff0-121">Name</span></span>       | <span data-ttu-id="19ff0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="19ff0-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="19ff0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19ff0-123">Authorization</span></span>  | <span data-ttu-id="19ff0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19ff0-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="19ff0-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="19ff0-126">Content-Type</span></span>  | <span data-ttu-id="19ff0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="19ff0-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="19ff0-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19ff0-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="19ff0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="19ff0-129">Response</span></span>

<span data-ttu-id="19ff0-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [domain](../resources/domain.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="19ff0-130">If successful, this method returns `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19ff0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="19ff0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="19ff0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="19ff0-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/verify
```

##### <a name="response"></a><span data-ttu-id="19ff0-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="19ff0-133">Response</span></span>
<span data-ttu-id="19ff0-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19ff0-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "name": "contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domain: verify",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-verify.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
