---
title: Получение объектов каталога из списка идентификаторов
description: Параметр запроса select недоступен для этой операции.
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 093e39a6d70193c03d0b2ae9d91b61f6bdf5bbbb
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43180946"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="12603-103">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="12603-103">Get directory objects from a list of ids</span></span>

<span data-ttu-id="12603-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12603-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12603-p101">Возвращает объекты каталогов, указанные в списке идентификаторов.  ПРИМЕЧАНИЕ. Возвращаемые объекты каталогов представляют собой полные объекты, содержащие **все** свойства. Параметр запроса `$select` недоступен для этой операции.</span><span class="sxs-lookup"><span data-stu-id="12603-p101">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="12603-108">Ниже перечислены некоторые распространенные случаи использования этой функции.</span><span class="sxs-lookup"><span data-stu-id="12603-108">Some common uses for this function are to:</span></span>

* <span data-ttu-id="12603-109">Разрешение идентификаторов, возвращаемых как часть коллекций идентификаторов функциями, например [getMemberObjects](/graph/api/directoryobject-getmemberobjects.md?view=graph-rest-beta) или [getMemberGroups](/graph/api/directoryobject-getmembergroups.md?view=graph-rest-beta), в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="12603-109">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](/graph/api/directoryobject-getmemberobjects.md?view=graph-rest-beta) or [getMemberGroups](/graph/api/directoryobject-getmembergroups.md?view=graph-rest-beta)  to their backing directory objects.</span></span>
* <span data-ttu-id="12603-110">Разрешение идентификаторов, которые приложение хранит во внешнем хранилище, в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="12603-110">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="12603-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="12603-111">Permissions</span></span>

<span data-ttu-id="12603-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12603-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="12603-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12603-114">Permission type</span></span>      | <span data-ttu-id="12603-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="12603-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12603-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12603-116">Delegated (work or school account)</span></span> | <span data-ttu-id="12603-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="12603-117">Directory.Read.All</span></span>    |
|<span data-ttu-id="12603-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12603-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12603-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12603-119">Not supported.</span></span>    |
|<span data-ttu-id="12603-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12603-120">Application</span></span> | <span data-ttu-id="12603-121">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="12603-121">Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="12603-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12603-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="12603-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12603-123">Request headers</span></span>

| <span data-ttu-id="12603-124">Имя</span><span class="sxs-lookup"><span data-stu-id="12603-124">Name</span></span>       | <span data-ttu-id="12603-125">Тип</span><span class="sxs-lookup"><span data-stu-id="12603-125">Type</span></span> | <span data-ttu-id="12603-126">Описание</span><span class="sxs-lookup"><span data-stu-id="12603-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="12603-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="12603-127">Authorization</span></span>  | <span data-ttu-id="12603-128">string</span><span class="sxs-lookup"><span data-stu-id="12603-128">string</span></span>  | <span data-ttu-id="12603-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12603-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="12603-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="12603-131">Content-Type</span></span>  | <span data-ttu-id="12603-132">application/json</span><span class="sxs-lookup"><span data-stu-id="12603-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="12603-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12603-133">Request body</span></span>

<span data-ttu-id="12603-134">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="12603-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="12603-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="12603-135">Parameter</span></span>   | <span data-ttu-id="12603-136">Тип</span><span class="sxs-lookup"><span data-stu-id="12603-136">Type</span></span> |<span data-ttu-id="12603-137">Описание</span><span class="sxs-lookup"><span data-stu-id="12603-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12603-138">ids</span><span class="sxs-lookup"><span data-stu-id="12603-138">ids</span></span>|<span data-ttu-id="12603-139">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="12603-139">String collection</span></span>| <span data-ttu-id="12603-p104">Коллекция идентификаторов, для которой необходимо возвратить объекты. Вы можете указать до 1000 идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="12603-p104">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="12603-142">types</span><span class="sxs-lookup"><span data-stu-id="12603-142">types</span></span>|<span data-ttu-id="12603-143">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="12603-143">String collection</span></span>| <span data-ttu-id="12603-144">Коллекция типов ресурсов, указывающая набор коллекций ресурсов, в котором необходимо выполнить поиск.</span><span class="sxs-lookup"><span data-stu-id="12603-144">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="12603-145">Если аргумент не указан, по умолчанию используется объект [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), который содержит все типы ресурсов, определенные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="12603-145">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="12603-146">В коллекции можно указать любой объект, производный от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta). Пример: [user](/graph/api/resources/user?view=graph-rest-beta), [group](/graph/api/resources/group?view=graph-rest-beta), [device](/graph/api/resources/device?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="12603-146">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-beta), [group](/graph/api/resources/group?view=graph-rest-beta), [device](/graph/api/resources/device?view=graph-rest-beta), and so on.</span></span> <span data-ttu-id="12603-147">Для поиска ссылок на партнерскую организацию, [поставляющую облачные решения](https://partner.microsoft.com/en-us/cloud-solution-provider), укажите ресурс [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="12603-147">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta).</span></span> <span data-ttu-id="12603-148">Если аргумент не указан, по умолчанию используется объект [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), который содержит все типы ресурсов, определенные в каталоге, кроме ссылок на партнерскую организацию, [поставляющую облачные решения](https://partner.microsoft.com/en-us/cloud-solution-provider).</span><span class="sxs-lookup"><span data-stu-id="12603-148">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="12603-149">В значениях не учитывается регистр символов.</span><span class="sxs-lookup"><span data-stu-id="12603-149">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="12603-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="12603-150">Response</span></span>

<span data-ttu-id="12603-151">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="12603-151">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12603-152">Пример</span><span class="sxs-lookup"><span data-stu-id="12603-152">Example</span></span>

##### <a name="request"></a><span data-ttu-id="12603-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="12603-153">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="12603-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="12603-154">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="12603-155">C#</span><span class="sxs-lookup"><span data-stu-id="12603-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getbyids-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12603-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12603-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getbyids-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12603-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12603-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getbyids-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="12603-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="12603-158">Response</span></span>

<span data-ttu-id="12603-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12603-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
