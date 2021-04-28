---
title: 'directoryObject: getByIds'
description: Возвращает объекты каталогов, указанные в списке идентификаторов.
author: keylimesoda
localization_priority: Priority
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: bcd1e20de65f6ddefc08310572ff596865d438da
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051496"
---
# <a name="directoryobject-getbyids"></a><span data-ttu-id="d336a-103">directoryObject: getByIds</span><span class="sxs-lookup"><span data-stu-id="d336a-103">directoryObject: getByIds</span></span>

<span data-ttu-id="d336a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d336a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d336a-105">Возвращение объектов каталогов, указанных в списке идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="d336a-105">Return the directory objects specified in a list of IDs.</span></span>

>[!NOTE]
><span data-ttu-id="d336a-106">У этого API есть [известная проблема](/graph/known-issues#incomplete-objects-when-using-getbyids-request).</span><span class="sxs-lookup"><span data-stu-id="d336a-106">This API has a [known issue](/graph/known-issues#incomplete-objects-when-using-getbyids-request).</span></span> <span data-ttu-id="d336a-107">Не все возвращаемые объекты каталогов представляют собой полные объекты, содержащие все свойства.</span><span class="sxs-lookup"><span data-stu-id="d336a-107">Not all directory objects returned are the full objects containing all their properties.</span></span>

<span data-ttu-id="d336a-108">Ниже перечислены некоторые распространенные случаи использования этой функции.</span><span class="sxs-lookup"><span data-stu-id="d336a-108">Some common uses for this function are to:</span></span>

* <span data-ttu-id="d336a-109">Разрешение идентификаторов, возвращаемых как часть коллекций идентификаторов функциями, например [getMemberObjects](directoryobject-getmemberobjects.md) или [getMemberGroups](directoryobject-getmembergroups.md), в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="d336a-109">Resolve IDs returned by functions (that return collections of IDs) such as [getMemberObjects](directoryobject-getmemberobjects.md) or [getMemberGroups](directoryobject-getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="d336a-110">Разрешение идентификаторов, которые приложение хранит во внешнем хранилище, в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="d336a-110">Resolve IDs persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d336a-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d336a-111">Permissions</span></span>

<span data-ttu-id="d336a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d336a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d336a-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d336a-114">Permission type</span></span>      | <span data-ttu-id="d336a-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d336a-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d336a-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d336a-116">Delegated (work or school account)</span></span> | <span data-ttu-id="d336a-117">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d336a-117">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d336a-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d336a-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d336a-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d336a-119">Not supported.</span></span>    |
|<span data-ttu-id="d336a-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d336a-120">Application</span></span> | <span data-ttu-id="d336a-121">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d336a-121">Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="d336a-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d336a-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="d336a-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d336a-123">Request headers</span></span>

| <span data-ttu-id="d336a-124">Имя</span><span class="sxs-lookup"><span data-stu-id="d336a-124">Name</span></span>       | <span data-ttu-id="d336a-125">Тип</span><span class="sxs-lookup"><span data-stu-id="d336a-125">Type</span></span> | <span data-ttu-id="d336a-126">Описание</span><span class="sxs-lookup"><span data-stu-id="d336a-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d336a-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d336a-127">Authorization</span></span>  | <span data-ttu-id="d336a-128">string</span><span class="sxs-lookup"><span data-stu-id="d336a-128">string</span></span>  | <span data-ttu-id="d336a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d336a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d336a-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d336a-131">Content-type</span></span>  | <span data-ttu-id="d336a-132">строка</span><span class="sxs-lookup"><span data-stu-id="d336a-132">string</span></span> | <span data-ttu-id="d336a-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d336a-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d336a-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d336a-135">Request body</span></span>

<span data-ttu-id="d336a-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d336a-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d336a-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="d336a-137">Parameter</span></span>   | <span data-ttu-id="d336a-138">Тип</span><span class="sxs-lookup"><span data-stu-id="d336a-138">Type</span></span> |<span data-ttu-id="d336a-139">Описание</span><span class="sxs-lookup"><span data-stu-id="d336a-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d336a-140">ids</span><span class="sxs-lookup"><span data-stu-id="d336a-140">ids</span></span>|<span data-ttu-id="d336a-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d336a-141">String collection</span></span>| <span data-ttu-id="d336a-142">Коллекция идентификаторов, для которой необходимо возвратить объекты.</span><span class="sxs-lookup"><span data-stu-id="d336a-142">A collection of IDs for which to return objects.</span></span>  <span data-ttu-id="d336a-143">Идентификаторы имеют формат GUID и представлены в виде строк.</span><span class="sxs-lookup"><span data-stu-id="d336a-143">The IDs are GUIDs, represented as strings.</span></span>  <span data-ttu-id="d336a-144">Вы можете указать до 1000 идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="d336a-144">You can specify up to 1000 IDs.</span></span> |
|<span data-ttu-id="d336a-145">types</span><span class="sxs-lookup"><span data-stu-id="d336a-145">types</span></span>|<span data-ttu-id="d336a-146">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="d336a-146">String collection</span></span>| <span data-ttu-id="d336a-147">Коллекция типов ресурсов, указывающая набор коллекций ресурсов, в котором необходимо выполнить поиск.</span><span class="sxs-lookup"><span data-stu-id="d336a-147">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="d336a-148">Если аргумент не указан, по умолчанию используется объект [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), который содержит все типы ресурсов, определенные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="d336a-148">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="d336a-149">В коллекции можно указать любой объект, производный от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0). Пример: [user](/graph/api/resources/user?view=graph-rest-v1.0), [group](/graph/api/resources/group?view=graph-rest-v1.0), [device](/graph/api/resources/device?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="d336a-149">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-v1.0), [group](/graph/api/resources/group?view=graph-rest-v1.0), [device](/graph/api/resources/device?view=graph-rest-v1.0), and so on.</span></span> <span data-ttu-id="d336a-150">Для поиска ссылок на партнерскую организацию, [поставляющую облачные решения](https://partner.microsoft.com/cloud-solution-provider), укажите ресурс [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="d336a-150">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0).</span></span> <span data-ttu-id="d336a-151">Если аргумент не указан, по умолчанию используется объект [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), который содержит все типы ресурсов, определенные в каталоге, кроме ссылок на партнерскую организацию, [поставляющую облачные решения](https://partner.microsoft.com/cloud-solution-provider).</span><span class="sxs-lookup"><span data-stu-id="d336a-151">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="d336a-152">В значениях не учитывается регистр символов.</span><span class="sxs-lookup"><span data-stu-id="d336a-152">The values are not case sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="d336a-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="d336a-153">Response</span></span>

<span data-ttu-id="d336a-154">В случае успеха этот метод возвращает код ответа `200 OK` и объект коллекции строк в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d336a-154">If successful, this method returns a `200 OK` response code and a string collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d336a-155">Пример</span><span class="sxs-lookup"><span data-stu-id="d336a-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="d336a-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="d336a-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d336a-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="d336a-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getById"
}-->

```http
POST https://graph.microsoft.com/v1.0/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893874940a3-97b7-68513b600544","5d6059b6368d-45f8-91e18e07d485f1d0"],
    "types":["user"]
}
```
# <a name="c"></a>[<span data-ttu-id="d336a-158">C#</span><span class="sxs-lookup"><span data-stu-id="d336a-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getbyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d336a-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d336a-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getbyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d336a-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d336a-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getbyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d336a-161">Java</span><span class="sxs-lookup"><span data-stu-id="d336a-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getbyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d336a-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="d336a-162">Response</span></span>

><span data-ttu-id="d336a-163">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d336a-163">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
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
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

