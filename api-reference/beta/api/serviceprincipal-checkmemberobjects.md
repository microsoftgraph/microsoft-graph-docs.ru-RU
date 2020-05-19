---
title: 'servicePrincipal: Чеккмемберобжектс'
description: Проверка членства в списке групп, ролей каталогов или административных единиц для указанного объекта участника службы.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 452f1bb58c870f0edaf6ebecc49346220c20db14
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289716"
---
# <a name="serviceprincipal-checkmemberobjects"></a><span data-ttu-id="ca32e-103">servicePrincipal: Чеккмемберобжектс</span><span class="sxs-lookup"><span data-stu-id="ca32e-103">servicePrincipal: checkMemberObjects</span></span>

<span data-ttu-id="ca32e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca32e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca32e-105">Проверка членства в списке групп, ролей каталогов или административных единиц для указанного объекта [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="ca32e-105">Check for membership in a list of groups, directory roles, or administrative units for the specified [servicePrincipal](../resources/serviceprincipal.md) object.</span></span> <span data-ttu-id="ca32e-106">Этот метод является транзитивным.</span><span class="sxs-lookup"><span data-stu-id="ca32e-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca32e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca32e-107">Permissions</span></span>

<span data-ttu-id="ca32e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca32e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ca32e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca32e-110">Permission type</span></span>                        | <span data-ttu-id="ca32e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca32e-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ca32e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca32e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ca32e-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ca32e-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>|
| <span data-ttu-id="ca32e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca32e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca32e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca32e-115">Not supported.</span></span> |
| <span data-ttu-id="ca32e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca32e-116">Application</span></span>                            | <span data-ttu-id="ca32e-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca32e-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca32e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca32e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="ca32e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca32e-119">Request headers</span></span>

| <span data-ttu-id="ca32e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ca32e-120">Name</span></span>          | <span data-ttu-id="ca32e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ca32e-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ca32e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca32e-122">Authorization</span></span> | <span data-ttu-id="ca32e-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="ca32e-123">Bearer {token}</span></span> |
| <span data-ttu-id="ca32e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ca32e-124">Content-Type</span></span>  | <span data-ttu-id="ca32e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ca32e-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca32e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ca32e-126">Request body</span></span>

<span data-ttu-id="ca32e-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ca32e-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ca32e-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="ca32e-128">Parameter</span></span>    | <span data-ttu-id="ca32e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ca32e-129">Type</span></span>        | <span data-ttu-id="ca32e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ca32e-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ca32e-131">ids</span><span class="sxs-lookup"><span data-stu-id="ca32e-131">ids</span></span>|<span data-ttu-id="ca32e-132">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ca32e-132">String collection</span></span>|<span data-ttu-id="ca32e-133">Коллекция, содержащая идентификаторы объектов групп, ролей каталогов, административных единиц или идентификаторов Ролетемплате ролей каталогов, в которых проверяется членство.</span><span class="sxs-lookup"><span data-stu-id="ca32e-133">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="ca32e-134">Можно указать до 20 объектов.</span><span class="sxs-lookup"><span data-stu-id="ca32e-134">Up to 20 objects may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="ca32e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca32e-135">Response</span></span>

<span data-ttu-id="ca32e-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ca32e-136">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ca32e-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="ca32e-137">Examples</span></span>

<span data-ttu-id="ca32e-138">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="ca32e-138">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="ca32e-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca32e-139">Request</span></span>

<span data-ttu-id="ca32e-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca32e-140">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/checkMemberObjects
Content-type: application/json

{
  "ids": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0",
    "62e90394-69f5-4237-9190-012177145e10",
    "86a64f51-3a64-4cc6-a8c8-6b8f000c0f52",
    "ac38546e-ddf3-437a-ac5c-27a94cd7a0f1"
  ]
}
```

### <a name="response"></a><span data-ttu-id="ca32e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca32e-141">Response</span></span>

<span data-ttu-id="ca32e-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ca32e-142">The following is an example of the response.</span></span> 

> <span data-ttu-id="ca32e-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ca32e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "String",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0", 
    "62e90394-69f5-4237-9190-012177145e10"
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
