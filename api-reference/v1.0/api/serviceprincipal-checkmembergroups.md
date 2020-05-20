---
title: 'servicePrincipal: Чеккмемберграупс'
description: Проверка участия в указанном списке групп. Возвращает из списка те группы, для которых у участника службы есть прямое или транзитивное членство.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 8eb007a3922084ab4a13b3fe390cb1b0cc3ac094
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289909"
---
# <a name="serviceprincipal-checkmembergroups"></a><span data-ttu-id="a2c0b-104">servicePrincipal: Чеккмемберграупс</span><span class="sxs-lookup"><span data-stu-id="a2c0b-104">servicePrincipal: checkMemberGroups</span></span>

<span data-ttu-id="a2c0b-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2c0b-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a2c0b-106">Проверка участия в указанном списке групп.</span><span class="sxs-lookup"><span data-stu-id="a2c0b-106">Check for membership in the specified list of groups.</span></span> <span data-ttu-id="a2c0b-107">Возвращает из списка те группы, для которых у [servicePrincipal](../resources/serviceprincipal.md) есть прямое или транзитивное членство.</span><span class="sxs-lookup"><span data-stu-id="a2c0b-107">Returns from the list those groups of which the [servicePrincipal](../resources/serviceprincipal.md) has a direct or transitive membership.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2c0b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a2c0b-108">Permissions</span></span>
<span data-ttu-id="a2c0b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2c0b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2c0b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2c0b-111">Permission type</span></span>      | <span data-ttu-id="a2c0b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2c0b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2c0b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2c0b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a2c0b-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a2c0b-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a2c0b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2c0b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2c0b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2c0b-116">Not supported.</span></span>    |
|<span data-ttu-id="a2c0b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2c0b-117">Application</span></span> | <span data-ttu-id="a2c0b-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2c0b-118">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2c0b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2c0b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="a2c0b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2c0b-120">Request headers</span></span>
| <span data-ttu-id="a2c0b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a2c0b-121">Name</span></span>       | <span data-ttu-id="a2c0b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a2c0b-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="a2c0b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a2c0b-123">Authorization</span></span> | <span data-ttu-id="a2c0b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2c0b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a2c0b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a2c0b-126">Content-Type</span></span> | <span data-ttu-id="a2c0b-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2c0b-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2c0b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2c0b-129">Request body</span></span>
<span data-ttu-id="a2c0b-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a2c0b-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a2c0b-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="a2c0b-131">Parameter</span></span>    | <span data-ttu-id="a2c0b-132">Тип</span><span class="sxs-lookup"><span data-stu-id="a2c0b-132">Type</span></span>   |<span data-ttu-id="a2c0b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="a2c0b-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2c0b-134">groupIds</span><span class="sxs-lookup"><span data-stu-id="a2c0b-134">groupIds</span></span>|<span data-ttu-id="a2c0b-135">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a2c0b-135">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="a2c0b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2c0b-136">Response</span></span>

<span data-ttu-id="a2c0b-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a2c0b-137">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a2c0b-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="a2c0b-138">Examples</span></span>
<span data-ttu-id="a2c0b-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a2c0b-139">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="a2c0b-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2c0b-140">Request</span></span>
<span data-ttu-id="a2c0b-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2c0b-141">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
### <a name="response"></a><span data-ttu-id="a2c0b-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2c0b-142">Response</span></span>
<span data-ttu-id="a2c0b-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a2c0b-143">Here is an example of the response.</span></span> 
><span data-ttu-id="a2c0b-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2c0b-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "servicePrincipal: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
