---
title: Создание домена
description: Добавление домена в клиент.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2fe4f7ded79c0b4393657ed867534ea8ba4eb78b
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43179404"
---
# <a name="create-domain"></a><span data-ttu-id="166db-103">Создание домена</span><span class="sxs-lookup"><span data-stu-id="166db-103">Create domain</span></span>

<span data-ttu-id="166db-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="166db-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="166db-105">Добавление домена в клиент.</span><span class="sxs-lookup"><span data-stu-id="166db-105">Adds a domain to the tenant.</span></span>

<span data-ttu-id="166db-p101">**Важно!** Вам не удастся использовать сопоставленный домен с вашим клиентом Azure AD, пока не будет проверено владение доменом. Дополнительные сведения см. в статье [Перечисление verificationDnsRecords](domain-list-verificationdnsrecords.md). Для корневых доменов требуется проверка. Например, для домена contoso.com требуется проверка. Если корневой домен проверен, то его дочерние домены будут автоматически считаться проверенными. Например, если домен contoso.com проверен, то его дочерний домен subdomain.contoso.com будет автоматически считаться проверенным.</span><span class="sxs-lookup"><span data-stu-id="166db-p101">**Important**: You cannot use an associated domain with your Azure AD tenant until ownership is verified. See [List verificationDnsRecords](domain-list-verificationdnsrecords.md) for details. Root domains require verification. For example, contoso.com requires verification. If a root domain is verified, subdomains of the root domain are automatically verified. For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="166db-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="166db-112">Permissions</span></span>

<span data-ttu-id="166db-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="166db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="166db-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="166db-115">Permission type</span></span>      | <span data-ttu-id="166db-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="166db-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="166db-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="166db-117">Delegated (work or school account)</span></span> | <span data-ttu-id="166db-118">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="166db-118">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="166db-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="166db-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="166db-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="166db-120">Not supported.</span></span>    |
|<span data-ttu-id="166db-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="166db-121">Application</span></span> | <span data-ttu-id="166db-122">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="166db-122">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="166db-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="166db-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains
```
## <a name="request-headers"></a><span data-ttu-id="166db-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="166db-124">Request headers</span></span>
| <span data-ttu-id="166db-125">Имя</span><span class="sxs-lookup"><span data-stu-id="166db-125">Name</span></span>       | <span data-ttu-id="166db-126">Описание</span><span class="sxs-lookup"><span data-stu-id="166db-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="166db-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="166db-127">Authorization</span></span>  | <span data-ttu-id="166db-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="166db-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="166db-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="166db-130">Content-Type</span></span>  | <span data-ttu-id="166db-131">application/json</span><span class="sxs-lookup"><span data-stu-id="166db-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="166db-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="166db-132">Request body</span></span>
<span data-ttu-id="166db-133">В теле запроса укажите представление JSON объекта [domain](../resources/domain.md).</span><span class="sxs-lookup"><span data-stu-id="166db-133">In the request body, supply a JSON representation of [domain](../resources/domain.md) object.</span></span>

> <span data-ttu-id="166db-p104">Тело запроса содержит свойство id для нового домена. id — это единственное свойство, которое можно указать, и оно является обязательным. Значение свойства id — полное доменное имя, которое необходимо создать.</span><span class="sxs-lookup"><span data-stu-id="166db-p104">The request body contains the id property for the new domain. Id is the only property that can be specified and it is required. The id property value is the fully qualified domain name to create.</span></span>

## <a name="response"></a><span data-ttu-id="166db-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="166db-137">Response</span></span>

<span data-ttu-id="166db-138">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [domain](../resources/domain.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="166db-138">If successful, this method returns `201 Created` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="166db-139">Пример</span><span class="sxs-lookup"><span data-stu-id="166db-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="166db-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="166db-140">Request</span></span>

<span data-ttu-id="166db-141">В теле запроса укажите представление JSON объекта [domain](../resources/domain.md).</span><span class="sxs-lookup"><span data-stu-id="166db-141">In the request body, supply a JSON representation of [domain](../resources/domain.md) object.</span></span>

<!-- {
  "blockType": "request",
  "id": "create_domain_from_domains"
}-->
```http
POST https://graph.microsoft.com/v1.0/domains
Content-type: application/json
Content-length: 192

{
  "id": "contoso.com"
}
```

##### <a name="response"></a><span data-ttu-id="166db-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="166db-142">Response</span></span>
<span data-ttu-id="166db-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="166db-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
