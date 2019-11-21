---
title: 'Группа: Чеккмемберобжектс'
description: Проверка членства в списке групп или ролей каталогов для указанного объекта Group.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e4f6bb2f940cd32940391799ff4a93387ab8ac32
ms.sourcegitcommit: c25828c596b7e0939fa164a3d7754722943152c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2019
ms.locfileid: "38757331"
---
# <a name="group-checkmemberobjects"></a><span data-ttu-id="aca3e-103">Группа: Чеккмемберобжектс</span><span class="sxs-lookup"><span data-stu-id="aca3e-103">group: checkMemberObjects</span></span>

<span data-ttu-id="aca3e-104">Проверка членства в списке групп или ролей каталогов для указанной группы.</span><span class="sxs-lookup"><span data-stu-id="aca3e-104">Check for membership in a list of groups or directory roles for the specified group.</span></span> <span data-ttu-id="aca3e-105">Этот метод является транзитивным.</span><span class="sxs-lookup"><span data-stu-id="aca3e-105">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="aca3e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aca3e-106">Permissions</span></span>

<span data-ttu-id="aca3e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aca3e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aca3e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aca3e-109">Permission type</span></span>                        | <span data-ttu-id="aca3e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aca3e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="aca3e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aca3e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="aca3e-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aca3e-112">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="aca3e-113">С</span><span class="sxs-lookup"><span data-stu-id="aca3e-113">And:</span></span><br><ul><li><span data-ttu-id="aca3e-114">При проверке принадлежности к административным единицам: AdministrativeUnit. Read. ALL, AdministrativeUnit. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="aca3e-114">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li></ul><br><span data-ttu-id="aca3e-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aca3e-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="aca3e-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aca3e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aca3e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aca3e-117">Not supported.</span></span> |
| <span data-ttu-id="aca3e-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aca3e-118">Application</span></span>                            | <span data-ttu-id="aca3e-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aca3e-119">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="aca3e-120">С</span><span class="sxs-lookup"><span data-stu-id="aca3e-120">And:</span></span><br><ul><li><span data-ttu-id="aca3e-121">При проверке принадлежности к административным единицам: AdministrativeUnit. Read. ALL, AdministrativeUnit. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="aca3e-121">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></ul></li><br><span data-ttu-id="aca3e-122">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aca3e-122">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aca3e-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aca3e-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="aca3e-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aca3e-124">Request headers</span></span>

| <span data-ttu-id="aca3e-125">Имя</span><span class="sxs-lookup"><span data-stu-id="aca3e-125">Name</span></span>          | <span data-ttu-id="aca3e-126">Описание</span><span class="sxs-lookup"><span data-stu-id="aca3e-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="aca3e-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aca3e-127">Authorization</span></span> | <span data-ttu-id="aca3e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aca3e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aca3e-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aca3e-130">Content-Type</span></span>  | <span data-ttu-id="aca3e-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aca3e-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aca3e-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aca3e-133">Request body</span></span>

<span data-ttu-id="aca3e-134">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="aca3e-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="aca3e-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="aca3e-135">Parameter</span></span>    | <span data-ttu-id="aca3e-136">Тип</span><span class="sxs-lookup"><span data-stu-id="aca3e-136">Type</span></span>        | <span data-ttu-id="aca3e-137">Описание</span><span class="sxs-lookup"><span data-stu-id="aca3e-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="aca3e-138">ids</span><span class="sxs-lookup"><span data-stu-id="aca3e-138">ids</span></span>|<span data-ttu-id="aca3e-139">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="aca3e-139">String collection</span></span>| <span data-ttu-id="aca3e-140">Коллекция, содержащая идентификаторы объектов групп, ролей каталогов или идентификаторов Ролетемплате для ролей каталогов, в которых проверяется членство.</span><span class="sxs-lookup"><span data-stu-id="aca3e-140">A collection that contains the object IDs of the groups, directory roles, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="aca3e-141">Можно указать до 20 объектов.</span><span class="sxs-lookup"><span data-stu-id="aca3e-141">You can specify up to 20 objects.</span></span> |

## <a name="response"></a><span data-ttu-id="aca3e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="aca3e-142">Response</span></span>

<span data-ttu-id="aca3e-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aca3e-143">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aca3e-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="aca3e-144">Examples</span></span>

<span data-ttu-id="aca3e-145">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="aca3e-145">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="aca3e-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="aca3e-146">Request</span></span>

<span data-ttu-id="aca3e-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aca3e-147">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="aca3e-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="aca3e-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/checkMemberObjects
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

### <a name="response"></a><span data-ttu-id="aca3e-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="aca3e-149">Response</span></span>

<span data-ttu-id="aca3e-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="aca3e-150">The following is an example of the response.</span></span> 

> <span data-ttu-id="aca3e-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aca3e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
