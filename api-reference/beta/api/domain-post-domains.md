---
title: Создание домена
description: Добавление домена в клиент.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d4c6e9731285f5e28829dc2bb5c77faae30775c4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436486"
---
# <a name="create-domain"></a><span data-ttu-id="429a8-103">Создание домена</span><span class="sxs-lookup"><span data-stu-id="429a8-103">Create domain</span></span>

<span data-ttu-id="429a8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="429a8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="429a8-105">Добавление домена в клиент.</span><span class="sxs-lookup"><span data-stu-id="429a8-105">Adds a domain to the tenant.</span></span>

<span data-ttu-id="429a8-p101">**Важно!** Вам не удастся использовать сопоставленный домен с вашим клиентом Azure AD, пока не будет проверено владение доменом. Дополнительные сведения см. в статье [Перечисление verificationDnsRecords](domain-list-verificationdnsrecords.md). Для корневых доменов требуется проверка. Например, для домена contoso.com требуется проверка. Если корневой домен проверен, то его дочерние домены будут автоматически считаться проверенными. Например, если домен contoso.com проверен, то его дочерний домен subdomain.contoso.com будет автоматически считаться проверенным.</span><span class="sxs-lookup"><span data-stu-id="429a8-p101">**Important**: You cannot use an associated domain with your Azure AD tenant until ownership is verified. See [List verificationDnsRecords](domain-list-verificationdnsrecords.md) for details. Root domains require verification. For example, contoso.com requires verification. If a root domain is verified, subdomains of the root domain are automatically verified. For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="429a8-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="429a8-112">Permissions</span></span>

<span data-ttu-id="429a8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="429a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="429a8-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="429a8-115">Permission type</span></span>      | <span data-ttu-id="429a8-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="429a8-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="429a8-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="429a8-117">Delegated (work or school account)</span></span> | <span data-ttu-id="429a8-118">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="429a8-118">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="429a8-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="429a8-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="429a8-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="429a8-120">Not supported.</span></span>    |
|<span data-ttu-id="429a8-121">Приложение</span><span class="sxs-lookup"><span data-stu-id="429a8-121">Application</span></span> | <span data-ttu-id="429a8-122">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="429a8-122">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="429a8-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="429a8-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains
```
## <a name="request-headers"></a><span data-ttu-id="429a8-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="429a8-124">Request headers</span></span>
| <span data-ttu-id="429a8-125">Имя</span><span class="sxs-lookup"><span data-stu-id="429a8-125">Name</span></span>       | <span data-ttu-id="429a8-126">Описание</span><span class="sxs-lookup"><span data-stu-id="429a8-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="429a8-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="429a8-127">Authorization</span></span>  | <span data-ttu-id="429a8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="429a8-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="429a8-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="429a8-130">Content-Type</span></span>  | <span data-ttu-id="429a8-131">application/json</span><span class="sxs-lookup"><span data-stu-id="429a8-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="429a8-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="429a8-132">Request body</span></span>
<span data-ttu-id="429a8-133">В теле запроса укажите представление JSON объекта [domain](../resources/domain.md).</span><span class="sxs-lookup"><span data-stu-id="429a8-133">In the request body, supply a JSON representation of [domain](../resources/domain.md) object.</span></span>

> <span data-ttu-id="429a8-p104">Тело запроса содержит свойство id для нового домена. id — это единственное свойство, которое можно указать, и оно является обязательным. Значение свойства id — полное доменное имя, которое необходимо создать.</span><span class="sxs-lookup"><span data-stu-id="429a8-p104">The request body contains the id property for the new domain. Id is the only property that can be specified and it is required. The id property value is the fully qualified domain name to create.</span></span>

## <a name="response"></a><span data-ttu-id="429a8-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="429a8-137">Response</span></span>

<span data-ttu-id="429a8-138">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [domain](../resources/domain.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="429a8-138">If successful, this method returns `201 Created` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="429a8-139">Пример</span><span class="sxs-lookup"><span data-stu-id="429a8-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="429a8-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="429a8-140">Request</span></span>

<span data-ttu-id="429a8-141">В теле запроса укажите представление JSON объекта [domain](../resources/domain.md).</span><span class="sxs-lookup"><span data-stu-id="429a8-141">In the request body, supply a JSON representation of [domain](../resources/domain.md) object.</span></span>

<!-- {
  "blockType": "request",
  "id": "create_domain_from_domains"
}-->
```http
POST https://graph.microsoft.com/beta/domains
Content-type: application/json
Content-length: 192

{
  "id": "contoso.com"
}
```

##### <a name="response"></a><span data-ttu-id="429a8-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="429a8-142">Response</span></span>
<span data-ttu-id="429a8-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="429a8-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


