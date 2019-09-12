---
title: 'servicePrincipal: Чеккмемберобжектс'
description: Проверка членства в списке групп, ролей каталогов или административных единиц для указанного объекта участника службы.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f0bcc7dd5c32ebe27e55169a8170069335607444
ms.sourcegitcommit: 4ce5060cddfa92cc282321bd9cfbf0a39de51aae
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2019
ms.locfileid: "36853883"
---
# <a name="serviceprincipal-checkmemberobjects"></a><span data-ttu-id="6819d-103">servicePrincipal: Чеккмемберобжектс</span><span class="sxs-lookup"><span data-stu-id="6819d-103">servicePrincipal: checkMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6819d-104">Проверка членства в списке групп, ролей каталогов или административных единиц для указанного объекта участника службы.</span><span class="sxs-lookup"><span data-stu-id="6819d-104">Check for membership in a list of groups, directory roles, or administrative units for the specified service principle object.</span></span> <span data-ttu-id="6819d-105">Этот метод является транзитивным.</span><span class="sxs-lookup"><span data-stu-id="6819d-105">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="6819d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6819d-106">Permissions</span></span>

<span data-ttu-id="6819d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6819d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6819d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6819d-109">Permission type</span></span>                        | <span data-ttu-id="6819d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6819d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6819d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6819d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6819d-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6819d-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>|
| <span data-ttu-id="6819d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6819d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6819d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6819d-114">Not supported.</span></span> |
| <span data-ttu-id="6819d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6819d-115">Application</span></span>                            | <span data-ttu-id="6819d-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6819d-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6819d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6819d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="6819d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6819d-118">Request headers</span></span>

| <span data-ttu-id="6819d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6819d-119">Name</span></span>          | <span data-ttu-id="6819d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6819d-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6819d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6819d-121">Authorization</span></span> | <span data-ttu-id="6819d-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="6819d-122">Bearer {token}</span></span> |
| <span data-ttu-id="6819d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6819d-123">Content-Type</span></span>  | <span data-ttu-id="6819d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6819d-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6819d-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6819d-125">Request body</span></span>

<span data-ttu-id="6819d-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6819d-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6819d-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="6819d-127">Parameter</span></span>    | <span data-ttu-id="6819d-128">Тип</span><span class="sxs-lookup"><span data-stu-id="6819d-128">Type</span></span>        | <span data-ttu-id="6819d-129">Описание</span><span class="sxs-lookup"><span data-stu-id="6819d-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6819d-130">ids</span><span class="sxs-lookup"><span data-stu-id="6819d-130">ids</span></span>|<span data-ttu-id="6819d-131">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6819d-131">String collection</span></span>|<span data-ttu-id="6819d-132">Коллекция, содержащая идентификаторы объектов групп, ролей каталогов, административных единиц или идентификаторов Ролетемплате ролей каталогов, в которых проверяется членство.</span><span class="sxs-lookup"><span data-stu-id="6819d-132">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="6819d-133">Можно указать до 20 объектов.</span><span class="sxs-lookup"><span data-stu-id="6819d-133">Up to 20 objects may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="6819d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6819d-134">Response</span></span>

<span data-ttu-id="6819d-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6819d-135">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6819d-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="6819d-136">Examples</span></span>

<span data-ttu-id="6819d-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="6819d-137">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="6819d-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="6819d-138">Request</span></span>

<span data-ttu-id="6819d-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6819d-139">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6819d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6819d-140">Response</span></span>

<span data-ttu-id="6819d-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6819d-141">The following is an example of the response.</span></span> 

> <span data-ttu-id="6819d-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6819d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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