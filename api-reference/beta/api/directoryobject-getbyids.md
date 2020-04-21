---
title: 'directoryObject: Жетбидс'
description: 'Возвращает объекты каталогов, указанные в списке идентификаторов. '
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f71233b25d4ede3479960e44a4de2876b4c9a0c7
ms.sourcegitcommit: 24092bd1e38e8adfd314dfe8dfea9b24a5c21da6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2020
ms.locfileid: "43581655"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="0a8f2-103">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="0a8f2-103">Get directory objects from a list of ids</span></span>

<span data-ttu-id="0a8f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a8f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a8f2-105">Возврат объектов каталогов, указанных в списке идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="0a8f2-105">Return the directory objects specified in a list of IDs.</span></span>  

<span data-ttu-id="0a8f2-106">Ниже перечислены некоторые распространенные случаи использования этой функции.</span><span class="sxs-lookup"><span data-stu-id="0a8f2-106">Some common uses for this function are to:</span></span>

* <span data-ttu-id="0a8f2-107">Разрешение идентификаторов, возвращаемых как часть коллекций идентификаторов функциями, например [getMemberObjects](/graph/api/directoryobject-getmemberobjects.md?view=graph-rest-beta) или [getMemberGroups](/graph/api/directoryobject-getmembergroups.md?view=graph-rest-beta), в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="0a8f2-107">Resolve IDs returned by functions (that return collections of IDs) such as [getMemberObjects](/graph/api/directoryobject-getmemberobjects.md?view=graph-rest-beta) or [getMemberGroups](/graph/api/directoryobject-getmembergroups.md?view=graph-rest-beta)  to their backing directory objects.</span></span>
* <span data-ttu-id="0a8f2-108">Разрешение идентификаторов, сохраненных во внешнем хранилище приложения, в объекты каталога резервного копирования.</span><span class="sxs-lookup"><span data-stu-id="0a8f2-108">Resolve IDs persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a8f2-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0a8f2-109">Permissions</span></span>

<span data-ttu-id="0a8f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a8f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0a8f2-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a8f2-112">Permission type</span></span>      | <span data-ttu-id="0a8f2-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a8f2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a8f2-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a8f2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0a8f2-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a8f2-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="0a8f2-116">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a8f2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a8f2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a8f2-117">Not supported.</span></span>    |
|<span data-ttu-id="0a8f2-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a8f2-118">Application</span></span> | <span data-ttu-id="0a8f2-119">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a8f2-119">Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="0a8f2-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a8f2-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="0a8f2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a8f2-121">Request headers</span></span>

| <span data-ttu-id="0a8f2-122">Имя</span><span class="sxs-lookup"><span data-stu-id="0a8f2-122">Name</span></span>       | <span data-ttu-id="0a8f2-123">Тип</span><span class="sxs-lookup"><span data-stu-id="0a8f2-123">Type</span></span> | <span data-ttu-id="0a8f2-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0a8f2-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0a8f2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a8f2-125">Authorization</span></span>  | <span data-ttu-id="0a8f2-126">string</span><span class="sxs-lookup"><span data-stu-id="0a8f2-126">string</span></span>  | <span data-ttu-id="0a8f2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a8f2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0a8f2-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0a8f2-129">Content-type</span></span>  | <span data-ttu-id="0a8f2-130">string</span><span class="sxs-lookup"><span data-stu-id="0a8f2-130">string</span></span> | <span data-ttu-id="0a8f2-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a8f2-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0a8f2-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a8f2-133">Request body</span></span>

<span data-ttu-id="0a8f2-134">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0a8f2-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0a8f2-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="0a8f2-135">Parameter</span></span>   | <span data-ttu-id="0a8f2-136">Тип</span><span class="sxs-lookup"><span data-stu-id="0a8f2-136">Type</span></span> |<span data-ttu-id="0a8f2-137">Описание</span><span class="sxs-lookup"><span data-stu-id="0a8f2-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a8f2-138">ids</span><span class="sxs-lookup"><span data-stu-id="0a8f2-138">ids</span></span>|<span data-ttu-id="0a8f2-139">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0a8f2-139">String collection</span></span>| <span data-ttu-id="0a8f2-140">Коллекция идентификаторов, для которой необходимо возвратить объекты.</span><span class="sxs-lookup"><span data-stu-id="0a8f2-140">A collection of IDs for which to return objects.</span></span> <span data-ttu-id="0a8f2-141">Идентификаторы идентификаторов GUID, представленные в виде строк.</span><span class="sxs-lookup"><span data-stu-id="0a8f2-141">The IDs are GUIDs, represented as strings.</span></span> <span data-ttu-id="0a8f2-142">Вы можете указать до 1000 идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="0a8f2-142">You can specify up to 1000 IDs.</span></span> |
|<span data-ttu-id="0a8f2-143">types</span><span class="sxs-lookup"><span data-stu-id="0a8f2-143">types</span></span>|<span data-ttu-id="0a8f2-144">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="0a8f2-144">String collection</span></span>| <span data-ttu-id="0a8f2-145">Коллекция типов ресурсов, указывающая набор коллекций ресурсов, в котором необходимо выполнить поиск.</span><span class="sxs-lookup"><span data-stu-id="0a8f2-145">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="0a8f2-146">Если аргумент не указан, по умолчанию используется объект [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), который содержит все типы ресурсов, определенные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="0a8f2-146">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="0a8f2-147">В коллекции можно указать любой объект, производный от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta). Пример: [user](/graph/api/resources/user?view=graph-rest-beta), [group](/graph/api/resources/group?view=graph-rest-beta), [device](/graph/api/resources/device?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="0a8f2-147">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-beta), [group](/graph/api/resources/group?view=graph-rest-beta), [device](/graph/api/resources/device?view=graph-rest-beta), and so on.</span></span> <span data-ttu-id="0a8f2-148">Для поиска ссылок на партнерскую организацию, [поставляющую облачные решения](https://partner.microsoft.com/cloud-solution-provider), укажите ресурс [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="0a8f2-148">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta).</span></span> <span data-ttu-id="0a8f2-149">Если аргумент не указан, по умолчанию используется объект [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), который содержит все типы ресурсов, определенные в каталоге, кроме ссылок на партнерскую организацию, [поставляющую облачные решения](https://partner.microsoft.com/en-us/cloud-solution-provider).</span><span class="sxs-lookup"><span data-stu-id="0a8f2-149">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="0a8f2-150">В значениях не учитывается регистр символов.</span><span class="sxs-lookup"><span data-stu-id="0a8f2-150">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="0a8f2-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a8f2-151">Response</span></span>

<span data-ttu-id="0a8f2-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0a8f2-152">If successful, this method returns a `200 OK` response code and a string collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a8f2-153">Пример</span><span class="sxs-lookup"><span data-stu-id="0a8f2-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a8f2-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a8f2-154">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0a8f2-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a8f2-155">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0a8f2-156">C#</span><span class="sxs-lookup"><span data-stu-id="0a8f2-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getbyids-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a8f2-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a8f2-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getbyids-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a8f2-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a8f2-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getbyids-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0a8f2-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a8f2-159">Response</span></span>

><span data-ttu-id="0a8f2-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0a8f2-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
