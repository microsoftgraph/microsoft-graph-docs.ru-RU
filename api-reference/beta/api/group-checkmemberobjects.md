---
title: 'Группа: Чеккмемберобжектс'
description: Проверка членства в списке групп, ролей каталогов или административных единиц для указанного объекта Group.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 38f2a460dc147416604f52d092e4cf2f99cc20c7
ms.sourcegitcommit: 4ce5060cddfa92cc282321bd9cfbf0a39de51aae
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2019
ms.locfileid: "36853878"
---
# <a name="group-checkmemberobjects"></a><span data-ttu-id="ff109-103">Группа: Чеккмемберобжектс</span><span class="sxs-lookup"><span data-stu-id="ff109-103">group: checkMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff109-104">Проверка членства в списке групп или административных единиц для указанной группы.</span><span class="sxs-lookup"><span data-stu-id="ff109-104">Check for membership in a list of groups or administrative units for the specified group.</span></span> <span data-ttu-id="ff109-105">Этот метод является транзитивным.</span><span class="sxs-lookup"><span data-stu-id="ff109-105">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff109-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ff109-106">Permissions</span></span>

<span data-ttu-id="ff109-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff109-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ff109-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff109-109">Permission type</span></span>                        | <span data-ttu-id="ff109-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff109-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ff109-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff109-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ff109-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff109-112">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="ff109-113">С</span><span class="sxs-lookup"><span data-stu-id="ff109-113">And:</span></span><br><ul><li><span data-ttu-id="ff109-114">При проверке принадлежности к административным единицам: AdministrativeUnit. Read. ALL, AdministrativeUnit. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ff109-114">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li></ul><br><span data-ttu-id="ff109-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ff109-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="ff109-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff109-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff109-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff109-117">Not supported.</span></span> |
| <span data-ttu-id="ff109-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff109-118">Application</span></span>                            | <span data-ttu-id="ff109-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff109-119">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="ff109-120">С</span><span class="sxs-lookup"><span data-stu-id="ff109-120">And:</span></span><br><ul><li><span data-ttu-id="ff109-121">При проверке принадлежности к административным единицам: AdministrativeUnit. Read. ALL, AdministrativeUnit. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ff109-121">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></ul></li><br><span data-ttu-id="ff109-122">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff109-122">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff109-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff109-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="ff109-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff109-124">Request headers</span></span>

| <span data-ttu-id="ff109-125">Имя</span><span class="sxs-lookup"><span data-stu-id="ff109-125">Name</span></span>          | <span data-ttu-id="ff109-126">Описание</span><span class="sxs-lookup"><span data-stu-id="ff109-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ff109-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ff109-127">Authorization</span></span> | <span data-ttu-id="ff109-128">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="ff109-128">Bearer {token}</span></span> |
| <span data-ttu-id="ff109-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ff109-129">Content-Type</span></span>  | <span data-ttu-id="ff109-130">application/json</span><span class="sxs-lookup"><span data-stu-id="ff109-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff109-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ff109-131">Request body</span></span>

<span data-ttu-id="ff109-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ff109-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ff109-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="ff109-133">Parameter</span></span>    | <span data-ttu-id="ff109-134">Тип</span><span class="sxs-lookup"><span data-stu-id="ff109-134">Type</span></span>        | <span data-ttu-id="ff109-135">Описание</span><span class="sxs-lookup"><span data-stu-id="ff109-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ff109-136">ids</span><span class="sxs-lookup"><span data-stu-id="ff109-136">ids</span></span>|<span data-ttu-id="ff109-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ff109-137">String collection</span></span>| <span data-ttu-id="ff109-138">Коллекция, содержащая идентификаторы объектов групп, ролей каталогов, административных единиц или идентификаторов Ролетемплате ролей каталогов, в которых проверяется членство.</span><span class="sxs-lookup"><span data-stu-id="ff109-138">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="ff109-139">Можно указать до 20 объектов.</span><span class="sxs-lookup"><span data-stu-id="ff109-139">Up to 20 objects may be specified.</span></span> |

## <a name="response"></a><span data-ttu-id="ff109-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff109-140">Response</span></span>

<span data-ttu-id="ff109-141">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ff109-141">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ff109-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="ff109-142">Examples</span></span>

<span data-ttu-id="ff109-143">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="ff109-143">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="ff109-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff109-144">Request</span></span>

<span data-ttu-id="ff109-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff109-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/checkMemberObjects
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

### <a name="response"></a><span data-ttu-id="ff109-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff109-146">Response</span></span>

<span data-ttu-id="ff109-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ff109-147">The following is an example of the response.</span></span> 

> <span data-ttu-id="ff109-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ff109-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "group: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->