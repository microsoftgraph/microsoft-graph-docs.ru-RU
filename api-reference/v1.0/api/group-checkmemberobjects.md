---
title: 'Группа: Чеккмемберобжектс'
description: Проверка членства в списке групп или ролей каталогов для указанного объекта Group.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7ecfbbdf68501feba69fe4808b8632a7cc04eb09
ms.sourcegitcommit: fc9edd17aebed91768e31416e1c1ee0b64d5ce06
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/27/2019
ms.locfileid: "39621635"
---
# <a name="group-checkmemberobjects"></a><span data-ttu-id="cbede-103">Группа: Чеккмемберобжектс</span><span class="sxs-lookup"><span data-stu-id="cbede-103">group: checkMemberObjects</span></span>

<span data-ttu-id="cbede-104">Проверка членства в списке групп или ролей каталогов для указанной группы.</span><span class="sxs-lookup"><span data-stu-id="cbede-104">Check for membership in a list of groups or directory roles for the specified group.</span></span> <span data-ttu-id="cbede-105">Этот метод является транзитивным.</span><span class="sxs-lookup"><span data-stu-id="cbede-105">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="cbede-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cbede-106">Permissions</span></span>

<span data-ttu-id="cbede-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbede-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cbede-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cbede-109">Permission type</span></span>                        | <span data-ttu-id="cbede-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cbede-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cbede-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cbede-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cbede-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbede-112">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="cbede-113">С</span><span class="sxs-lookup"><span data-stu-id="cbede-113">And:</span></span><br><ul><li><span data-ttu-id="cbede-114">При проверке принадлежности к административным единицам: AdministrativeUnit. Read. ALL, AdministrativeUnit. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="cbede-114">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li></ul><br><span data-ttu-id="cbede-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cbede-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="cbede-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cbede-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbede-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbede-117">Not supported.</span></span> |
| <span data-ttu-id="cbede-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cbede-118">Application</span></span>                            | <span data-ttu-id="cbede-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbede-119">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="cbede-120">С</span><span class="sxs-lookup"><span data-stu-id="cbede-120">And:</span></span><br><ul><li><span data-ttu-id="cbede-121">При проверке принадлежности к административным единицам: AdministrativeUnit. Read. ALL, AdministrativeUnit. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="cbede-121">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></ul></li><br><span data-ttu-id="cbede-122">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbede-122">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cbede-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cbede-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="cbede-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cbede-124">Request headers</span></span>

| <span data-ttu-id="cbede-125">Имя</span><span class="sxs-lookup"><span data-stu-id="cbede-125">Name</span></span>          | <span data-ttu-id="cbede-126">Описание</span><span class="sxs-lookup"><span data-stu-id="cbede-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cbede-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cbede-127">Authorization</span></span> | <span data-ttu-id="cbede-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cbede-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cbede-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cbede-130">Content-Type</span></span>  | <span data-ttu-id="cbede-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cbede-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cbede-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cbede-133">Request body</span></span>

<span data-ttu-id="cbede-134">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="cbede-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cbede-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="cbede-135">Parameter</span></span>    | <span data-ttu-id="cbede-136">Тип</span><span class="sxs-lookup"><span data-stu-id="cbede-136">Type</span></span>        | <span data-ttu-id="cbede-137">Описание</span><span class="sxs-lookup"><span data-stu-id="cbede-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cbede-138">ids</span><span class="sxs-lookup"><span data-stu-id="cbede-138">ids</span></span>|<span data-ttu-id="cbede-139">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cbede-139">String collection</span></span>| <span data-ttu-id="cbede-140">Коллекция, содержащая идентификаторы объектов групп, ролей каталогов или идентификаторов Ролетемплате для ролей каталогов, в которых проверяется членство.</span><span class="sxs-lookup"><span data-stu-id="cbede-140">A collection that contains the object IDs of the groups, directory roles, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="cbede-141">Можно указать до 20 объектов.</span><span class="sxs-lookup"><span data-stu-id="cbede-141">You can specify up to 20 objects.</span></span> |

## <a name="response"></a><span data-ttu-id="cbede-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="cbede-142">Response</span></span>

<span data-ttu-id="cbede-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cbede-143">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cbede-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="cbede-144">Examples</span></span>

<span data-ttu-id="cbede-145">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="cbede-145">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="cbede-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="cbede-146">Request</span></span>

<span data-ttu-id="cbede-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cbede-147">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cbede-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="cbede-148">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="cbede-149">C#</span><span class="sxs-lookup"><span data-stu-id="cbede-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cbede-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cbede-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cbede-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cbede-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cbede-152">Java</span><span class="sxs-lookup"><span data-stu-id="cbede-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cbede-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbede-153">Response</span></span>

<span data-ttu-id="cbede-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cbede-154">The following is an example of the response.</span></span> 

> <span data-ttu-id="cbede-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cbede-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
