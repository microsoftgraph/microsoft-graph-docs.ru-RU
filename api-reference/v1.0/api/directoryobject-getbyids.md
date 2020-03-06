---
title: Получение объектов каталога из списка идентификаторов
description: Параметр запроса select недоступен для этой операции.
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cf525e7251f39ca1a5a67458f4ea5e371f2601ad
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517995"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="67c56-103">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="67c56-103">Get directory objects from a list of ids</span></span>

<span data-ttu-id="67c56-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67c56-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="67c56-105">Возвращает объекты каталогов, указанные в списке идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="67c56-105">Returns the directory objects specified in a list of IDs.</span></span>

>[!NOTE]
><span data-ttu-id="67c56-106">Возвращаемые объекты каталогов представляют собой полные объекты, содержащие все свойства.</span><span class="sxs-lookup"><span data-stu-id="67c56-106">The directory objects returned are the full objects containing all their properties.</span></span> <span data-ttu-id="67c56-107">Параметр запроса `$select` недоступен для этой операции.</span><span class="sxs-lookup"><span data-stu-id="67c56-107">The `$select` query option is not available for this operation.</span></span>

>[!NOTE]
><span data-ttu-id="67c56-108">У этого API есть [известная проблема](/graph/known-issues#incomplete-objects-when-using-getbyids-request).</span><span class="sxs-lookup"><span data-stu-id="67c56-108">This API has a [known issue](/graph/known-issues#incomplete-objects-when-using-getbyids-request).</span></span> <span data-ttu-id="67c56-109">Не все возвращаемые объекты каталогов представляют собой полные объекты, содержащие все свойства.</span><span class="sxs-lookup"><span data-stu-id="67c56-109">Not all directory objects returned are the full objects containing all their properties.</span></span>

<span data-ttu-id="67c56-110">Ниже перечислены некоторые распространенные случаи использования этой функции.</span><span class="sxs-lookup"><span data-stu-id="67c56-110">Some common uses for this function are to:</span></span>

* <span data-ttu-id="67c56-111">Разрешение идентификаторов, возвращаемых как часть коллекций идентификаторов функциями, например [getMemberObjects](directoryobject-getmemberobjects.md) или [getMemberGroups](directoryobject-getmembergroups.md), в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="67c56-111">Resolve IDs returned by functions (that return collections of IDs) such as [getMemberObjects](directoryobject-getmemberobjects.md) or [getMemberGroups](directoryobject-getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="67c56-112">Разрешение идентификаторов, которые приложение хранит во внешнем хранилище, в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="67c56-112">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="67c56-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="67c56-113">Permissions</span></span>

<span data-ttu-id="67c56-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67c56-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="67c56-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67c56-116">Permission type</span></span>      | <span data-ttu-id="67c56-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="67c56-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67c56-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67c56-118">Delegated (work or school account)</span></span> | <span data-ttu-id="67c56-119">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="67c56-119">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="67c56-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67c56-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67c56-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67c56-121">Not supported.</span></span>    |
|<span data-ttu-id="67c56-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67c56-122">Application</span></span> | <span data-ttu-id="67c56-123">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="67c56-123">Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="67c56-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67c56-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="67c56-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67c56-125">Request headers</span></span>

| <span data-ttu-id="67c56-126">Имя</span><span class="sxs-lookup"><span data-stu-id="67c56-126">Name</span></span>       | <span data-ttu-id="67c56-127">Тип</span><span class="sxs-lookup"><span data-stu-id="67c56-127">Type</span></span> | <span data-ttu-id="67c56-128">Описание</span><span class="sxs-lookup"><span data-stu-id="67c56-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="67c56-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="67c56-129">Authorization</span></span>  | <span data-ttu-id="67c56-130">string</span><span class="sxs-lookup"><span data-stu-id="67c56-130">string</span></span>  | <span data-ttu-id="67c56-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67c56-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="67c56-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="67c56-133">Content-Type</span></span>  | <span data-ttu-id="67c56-134">string</span><span class="sxs-lookup"><span data-stu-id="67c56-134">string</span></span> | <span data-ttu-id="67c56-135">application/json</span><span class="sxs-lookup"><span data-stu-id="67c56-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="67c56-136">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="67c56-136">Request body</span></span>

<span data-ttu-id="67c56-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="67c56-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="67c56-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="67c56-138">Parameter</span></span>   | <span data-ttu-id="67c56-139">Тип</span><span class="sxs-lookup"><span data-stu-id="67c56-139">Type</span></span> |<span data-ttu-id="67c56-140">Описание</span><span class="sxs-lookup"><span data-stu-id="67c56-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67c56-141">ids</span><span class="sxs-lookup"><span data-stu-id="67c56-141">ids</span></span>|<span data-ttu-id="67c56-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="67c56-142">String collection</span></span>| <span data-ttu-id="67c56-143">Коллекция идентификаторов, для которой необходимо возвратить объекты.</span><span class="sxs-lookup"><span data-stu-id="67c56-143">A collection of IDs for which to return objects.</span></span> <span data-ttu-id="67c56-144">Вы можете указать до 1000 идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="67c56-144">You can specify up to 1000 IDs.</span></span> |
|<span data-ttu-id="67c56-145">types</span><span class="sxs-lookup"><span data-stu-id="67c56-145">types</span></span>|<span data-ttu-id="67c56-146">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="67c56-146">String collection</span></span>| <span data-ttu-id="67c56-147">Коллекция типов ресурсов, указывающая набор коллекций ресурсов, в котором необходимо выполнить поиск.</span><span class="sxs-lookup"><span data-stu-id="67c56-147">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="67c56-148">Если аргумент не указан, по умолчанию используется объект [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), который содержит все типы ресурсов, определенные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="67c56-148">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="67c56-149">В коллекции можно указать любой объект, производный от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0). Пример: [user](/graph/api/resources/user?view=graph-rest-v1.0), [group](/graph/api/resources/group?view=graph-rest-v1.0), [device](/graph/api/resources/device?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="67c56-149">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-v1.0), [group](/graph/api/resources/group?view=graph-rest-v1.0), [device](/graph/api/resources/device?view=graph-rest-v1.0), and so on.</span></span> <span data-ttu-id="67c56-150">Для поиска ссылок на партнерскую организацию, [поставляющую облачные решения](https://partner.microsoft.com/ru-RU/cloud-solution-provider), укажите ресурс [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="67c56-150">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/ru-RU/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0).</span></span> <span data-ttu-id="67c56-151">Если аргумент не указан, по умолчанию используется объект [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), который содержит все типы ресурсов, определенные в каталоге, кроме ссылок на партнерскую организацию, [поставляющую облачные решения](https://partner.microsoft.com/ru-RU/cloud-solution-provider).</span><span class="sxs-lookup"><span data-stu-id="67c56-151">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/ru-RU/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="67c56-152">В значениях не учитывается регистр символов.</span><span class="sxs-lookup"><span data-stu-id="67c56-152">The values are not case sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="67c56-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="67c56-153">Response</span></span>

<span data-ttu-id="67c56-154">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="67c56-154">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67c56-155">Пример</span><span class="sxs-lookup"><span data-stu-id="67c56-155">Example</span></span>

##### <a name="request"></a><span data-ttu-id="67c56-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="67c56-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="67c56-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="67c56-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="67c56-158">C#</span><span class="sxs-lookup"><span data-stu-id="67c56-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getbyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67c56-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67c56-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getbyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67c56-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67c56-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getbyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="67c56-161">Java</span><span class="sxs-lookup"><span data-stu-id="67c56-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getbyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="67c56-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="67c56-162">Response</span></span>

<span data-ttu-id="67c56-p107">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67c56-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
