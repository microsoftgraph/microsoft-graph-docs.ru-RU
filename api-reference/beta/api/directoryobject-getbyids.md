---
title: 'directoryObject: getByIds'
description: 'Возвращает объекты каталогов, указанные в списке идентификаторов. '
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b4bf049ed135b1dd563d640827360ddf91db0d47
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48312878"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="d9514-103">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="d9514-103">Get directory objects from a list of ids</span></span>

<span data-ttu-id="d9514-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9514-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9514-105">Возвращение объектов каталогов, указанных в списке идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="d9514-105">Return the directory objects specified in a list of IDs.</span></span>

<span data-ttu-id="d9514-106">Ниже перечислены некоторые распространенные случаи использования этой функции.</span><span class="sxs-lookup"><span data-stu-id="d9514-106">Some common uses for this function are to:</span></span>

* <span data-ttu-id="d9514-107">Разрешение идентификаторов, возвращаемых как часть коллекций идентификаторов функциями, например [getMemberObjects](./directoryobject-getmemberobjects.md) или [getMemberGroups](./directoryobject-getmembergroups.md), в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="d9514-107">Resolve IDs returned by functions (that return collections of IDs) such as [getMemberObjects](./directoryobject-getmemberobjects.md) or [getMemberGroups](./directoryobject-getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="d9514-108">Разрешение идентификаторов, которые приложение хранит во внешнем хранилище, в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="d9514-108">Resolve IDs persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9514-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9514-109">Permissions</span></span>

<span data-ttu-id="d9514-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9514-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d9514-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9514-112">Permission type</span></span>      | <span data-ttu-id="d9514-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9514-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9514-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9514-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d9514-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9514-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="d9514-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9514-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9514-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9514-117">Not supported.</span></span>    |
|<span data-ttu-id="d9514-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9514-118">Application</span></span> | <span data-ttu-id="d9514-119">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9514-119">Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="d9514-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9514-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="d9514-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9514-121">Request headers</span></span>

| <span data-ttu-id="d9514-122">Имя</span><span class="sxs-lookup"><span data-stu-id="d9514-122">Name</span></span>       | <span data-ttu-id="d9514-123">Тип</span><span class="sxs-lookup"><span data-stu-id="d9514-123">Type</span></span> | <span data-ttu-id="d9514-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d9514-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d9514-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9514-125">Authorization</span></span>  | <span data-ttu-id="d9514-126">string</span><span class="sxs-lookup"><span data-stu-id="d9514-126">string</span></span>  | <span data-ttu-id="d9514-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9514-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d9514-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d9514-129">Content-type</span></span>  | <span data-ttu-id="d9514-130">строка</span><span class="sxs-lookup"><span data-stu-id="d9514-130">string</span></span> | <span data-ttu-id="d9514-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9514-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d9514-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d9514-133">Request body</span></span>

<span data-ttu-id="d9514-134">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d9514-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d9514-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="d9514-135">Parameter</span></span>   | <span data-ttu-id="d9514-136">Тип</span><span class="sxs-lookup"><span data-stu-id="d9514-136">Type</span></span> |<span data-ttu-id="d9514-137">Описание</span><span class="sxs-lookup"><span data-stu-id="d9514-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9514-138">ids</span><span class="sxs-lookup"><span data-stu-id="d9514-138">ids</span></span>|<span data-ttu-id="d9514-139">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d9514-139">String collection</span></span>| <span data-ttu-id="d9514-140">Коллекция идентификаторов, для которой необходимо возвратить объекты.</span><span class="sxs-lookup"><span data-stu-id="d9514-140">A collection of IDs for which to return objects.</span></span> <span data-ttu-id="d9514-141">Идентификаторы имеют формат GUID и представлены в виде строк.</span><span class="sxs-lookup"><span data-stu-id="d9514-141">The IDs are GUIDs, represented as strings.</span></span> <span data-ttu-id="d9514-142">Вы можете указать до 1000 идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="d9514-142">You can specify up to 1000 IDs.</span></span> |
|<span data-ttu-id="d9514-143">types</span><span class="sxs-lookup"><span data-stu-id="d9514-143">types</span></span>|<span data-ttu-id="d9514-144">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="d9514-144">String collection</span></span>| <span data-ttu-id="d9514-145">Коллекция типов ресурсов, указывающая набор коллекций ресурсов, в котором необходимо выполнить поиск.</span><span class="sxs-lookup"><span data-stu-id="d9514-145">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="d9514-146">Если аргумент не указан, по умолчанию используется объект [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), который содержит все типы ресурсов, определенные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="d9514-146">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="d9514-147">В коллекции можно указать любой объект, производный от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta). Пример: [user](/graph/api/resources/user?view=graph-rest-beta), [group](/graph/api/resources/group?view=graph-rest-beta), [device](/graph/api/resources/device?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="d9514-147">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-beta), [group](/graph/api/resources/group?view=graph-rest-beta), [device](/graph/api/resources/device?view=graph-rest-beta), and so on.</span></span> <span data-ttu-id="d9514-148">Для поиска ссылок на партнерскую организацию, [поставляющую облачные решения](https://partner.microsoft.com/cloud-solution-provider), укажите ресурс [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="d9514-148">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta).</span></span> <span data-ttu-id="d9514-149">Если аргумент не указан, по умолчанию используется объект [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), который содержит все типы ресурсов, определенные в каталоге, кроме ссылок на партнерскую организацию, [поставляющую облачные решения](https://partner.microsoft.com/cloud-solution-provider).</span><span class="sxs-lookup"><span data-stu-id="d9514-149">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="d9514-150">В значениях не учитывается регистр символов.</span><span class="sxs-lookup"><span data-stu-id="d9514-150">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="d9514-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9514-151">Response</span></span>

<span data-ttu-id="d9514-152">В случае успеха этот метод возвращает код ответа `200 OK` и объект коллекции строк в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d9514-152">If successful, this method returns a `200 OK` response code and a string collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9514-153">Пример</span><span class="sxs-lookup"><span data-stu-id="d9514-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9514-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9514-154">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d9514-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9514-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getByIds"
}-->

```http
POST https://graph.microsoft.com/beta/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893-8749-40a3-97b7-68513b600544","5d6059b6-368d-45f8-91e1-8e07d485f1d0"],
    "types":["user"]
}
```
# <a name="c"></a>[<span data-ttu-id="d9514-156">C#</span><span class="sxs-lookup"><span data-stu-id="d9514-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getbyids-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9514-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9514-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getbyids-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9514-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9514-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getbyids-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d9514-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9514-159">Response</span></span>

><span data-ttu-id="d9514-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d9514-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects",
    "value": [
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Trevor Jones"
      },
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Billy Smith"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
