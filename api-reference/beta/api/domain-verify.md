---
title: 'domain: verify'
description: Проверка права собственности на домен.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e61456ccf7e47283464bddb4103a02dbfdb9bdb3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950629"
---
# <a name="domain-verify"></a><span data-ttu-id="70c18-103">domain: verify</span><span class="sxs-lookup"><span data-stu-id="70c18-103">domain: verify</span></span>

> <span data-ttu-id="70c18-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="70c18-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70c18-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70c18-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="70c18-106">Проверка права собственности на домен.</span><span class="sxs-lookup"><span data-stu-id="70c18-106">Validates the ownership of the domain.</span></span>

> <span data-ttu-id="70c18-p102">**Важно!** Применяется только к непроверенному домену. Для непроверенного домена свойство isVerified объекта [domain](../resources/domain.md) будет иметь значение false.</span><span class="sxs-lookup"><span data-stu-id="70c18-p102">**Important:** Only applies to an unverified domain. For an unverified domain, the isVerified property of the [domain](../resources/domain.md) is false.</span></span>

## <a name="permissions"></a><span data-ttu-id="70c18-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70c18-109">Permissions</span></span>

<span data-ttu-id="70c18-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70c18-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="70c18-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70c18-112">Permission type</span></span>      | <span data-ttu-id="70c18-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70c18-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70c18-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70c18-114">Delegated (work or school account)</span></span> | <span data-ttu-id="70c18-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="70c18-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="70c18-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70c18-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70c18-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70c18-117">Not supported.</span></span>    |
|<span data-ttu-id="70c18-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70c18-118">Application</span></span> | <span data-ttu-id="70c18-119">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70c18-119">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70c18-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70c18-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> <span data-ttu-id="70c18-121">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="70c18-121">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="70c18-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70c18-122">Request headers</span></span>

| <span data-ttu-id="70c18-123">Имя</span><span class="sxs-lookup"><span data-stu-id="70c18-123">Name</span></span>       | <span data-ttu-id="70c18-124">Описание</span><span class="sxs-lookup"><span data-stu-id="70c18-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="70c18-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70c18-125">Authorization</span></span>  | <span data-ttu-id="70c18-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70c18-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="70c18-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="70c18-128">Content-Type</span></span>  | <span data-ttu-id="70c18-129">application/json</span><span class="sxs-lookup"><span data-stu-id="70c18-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="70c18-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="70c18-130">Request body</span></span>

## <a name="response"></a><span data-ttu-id="70c18-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="70c18-131">Response</span></span>

<span data-ttu-id="70c18-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [domain](../resources/domain.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="70c18-132">If successful, this method returns `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70c18-133">Пример</span><span class="sxs-lookup"><span data-stu-id="70c18-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70c18-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="70c18-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/verify
```

##### <a name="response"></a><span data-ttu-id="70c18-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="70c18-135">Response</span></span>
<span data-ttu-id="70c18-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70c18-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "domain: verify",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
