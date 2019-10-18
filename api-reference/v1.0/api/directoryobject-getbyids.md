---
title: Получение объектов каталога из списка идентификаторов
description: Параметр запроса select недоступен для этой операции.
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 55782b87569b4d153178c604af88126202c88f98
ms.sourcegitcommit: 25884c00cbfa2aa5c001cf777fd0ffa3c9a5ed68
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36758302"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="34d2d-103">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="34d2d-103">Get directory objects from a list of ids</span></span>

<span data-ttu-id="34d2d-104">Возвращает объекты каталогов, указанные в списке идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="34d2d-104">Returns the directory objects specified in a list of IDs.</span></span>

>[!NOTE]
><span data-ttu-id="34d2d-105">Возвращаемые объекты каталогов представляют собой полные объекты, содержащие все свойства.</span><span class="sxs-lookup"><span data-stu-id="34d2d-105">The directory objects returned are the full objects containing all their properties.</span></span> <span data-ttu-id="34d2d-106">Параметр запроса `$select` недоступен для этой операции.</span><span class="sxs-lookup"><span data-stu-id="34d2d-106">select\` query option is not available for this operation.</span></span>

>[!NOTE]
><span data-ttu-id="34d2d-107">У этого API есть [известная проблема](/graph/known-issues#incomplete-objects-when-using-getbyids-request).</span><span class="sxs-lookup"><span data-stu-id="34d2d-107">This API has a [known issue](/graph/known-issues#incomplete-objects-when-using-getbyids-request).</span></span> <span data-ttu-id="34d2d-108">Не все возвращаемые объекты каталогов представляют собой полные объекты, содержащие все свойства.</span><span class="sxs-lookup"><span data-stu-id="34d2d-108">Not all directory objects returned are the full objects containing all their properties.</span></span>

<span data-ttu-id="34d2d-109">Ниже перечислены некоторые распространенные случаи использования этой функции.</span><span class="sxs-lookup"><span data-stu-id="34d2d-109">Some common uses for this function are to:</span></span>

* <span data-ttu-id="34d2d-110">Разрешение идентификаторов, возвращаемых как часть коллекций идентификаторов функциями, например [getMemberObjects](directoryobject-getmemberobjects.md) или [getMemberGroups](directoryobject-getmembergroups.md), в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="34d2d-110">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](directoryobject-getmemberobjects.md) or [getMemberGroups](directoryobject-getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="34d2d-111">Разрешение идентификаторов, которые приложение хранит во внешнем хранилище, в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="34d2d-111">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="34d2d-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="34d2d-112">Permissions</span></span>

<span data-ttu-id="34d2d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34d2d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="34d2d-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34d2d-115">Permission type</span></span>      | <span data-ttu-id="34d2d-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="34d2d-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34d2d-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34d2d-117">Delegated (work or school account)</span></span> | <span data-ttu-id="34d2d-118">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="34d2d-118">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="34d2d-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34d2d-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34d2d-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34d2d-120">Not supported.</span></span>    |
|<span data-ttu-id="34d2d-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34d2d-121">Application</span></span> | <span data-ttu-id="34d2d-122">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="34d2d-122">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="34d2d-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34d2d-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="34d2d-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34d2d-124">Request headers</span></span>

| <span data-ttu-id="34d2d-125">Имя</span><span class="sxs-lookup"><span data-stu-id="34d2d-125">Name</span></span>       | <span data-ttu-id="34d2d-126">Тип</span><span class="sxs-lookup"><span data-stu-id="34d2d-126">Type</span></span> | <span data-ttu-id="34d2d-127">Описание</span><span class="sxs-lookup"><span data-stu-id="34d2d-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="34d2d-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="34d2d-128">Authorization</span></span>  | <span data-ttu-id="34d2d-129">string</span><span class="sxs-lookup"><span data-stu-id="34d2d-129">string</span></span>  | <span data-ttu-id="34d2d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34d2d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="34d2d-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="34d2d-132">Content-Type</span></span>  | <span data-ttu-id="34d2d-133">string</span><span class="sxs-lookup"><span data-stu-id="34d2d-133">string</span></span> | <span data-ttu-id="34d2d-134">application/json</span><span class="sxs-lookup"><span data-stu-id="34d2d-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="34d2d-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="34d2d-135">Request body</span></span>

<span data-ttu-id="34d2d-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="34d2d-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="34d2d-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="34d2d-137">Parameter</span></span>   | <span data-ttu-id="34d2d-138">Тип</span><span class="sxs-lookup"><span data-stu-id="34d2d-138">Type</span></span> |<span data-ttu-id="34d2d-139">Описание</span><span class="sxs-lookup"><span data-stu-id="34d2d-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34d2d-140">ids</span><span class="sxs-lookup"><span data-stu-id="34d2d-140">ids</span></span>|<span data-ttu-id="34d2d-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="34d2d-141">String collection</span></span>| <span data-ttu-id="34d2d-142">Коллекция идентификаторов, для которой необходимо возвратить объекты.</span><span class="sxs-lookup"><span data-stu-id="34d2d-142">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> <span data-ttu-id="34d2d-143">Вы можете указать до 1000 идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="34d2d-143">You can specify up to 1000 IDs.</span></span> |
|<span data-ttu-id="34d2d-144">types</span><span class="sxs-lookup"><span data-stu-id="34d2d-144">types</span></span>|<span data-ttu-id="34d2d-145">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="34d2d-145">String collection</span></span>| <span data-ttu-id="34d2d-146">Коллекция типов ресурсов, указывающая набор коллекций ресурсов, в котором необходимо выполнить поиск.</span><span class="sxs-lookup"><span data-stu-id="34d2d-146">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="34d2d-147">Если аргумент не указан, по умолчанию используется объект [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), который содержит все типы ресурсов, определенные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="34d2d-147">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="34d2d-148">В коллекции можно указать любой объект, производный от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0). Пример: [user](/graph/api/resources/user?view=graph-rest-v1.0), [group](/graph/api/resources/group?view=graph-rest-v1.0), [device](/graph/api/resources/device?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="34d2d-148">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-v1.0), [group](/graph/api/resources/group?view=graph-rest-v1.0), [device](/graph/api/resources/device?view=graph-rest-v1.0), and so on.</span></span> <span data-ttu-id="34d2d-149">Для поиска ссылок на партнерскую организацию, [поставляющую облачные решения](https://partner.microsoft.com/ru-RU/cloud-solution-provider), укажите ресурс [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="34d2d-149">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/ru-RU/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0).</span></span> <span data-ttu-id="34d2d-150">Если аргумент не указан, по умолчанию используется объект [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), который содержит все типы ресурсов, определенные в каталоге, кроме ссылок на партнерскую организацию, [поставляющую облачные решения](https://partner.microsoft.com/ru-RU/cloud-solution-provider).</span><span class="sxs-lookup"><span data-stu-id="34d2d-150">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/ru-RU/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="34d2d-151">В значениях не учитывается регистр символов.</span><span class="sxs-lookup"><span data-stu-id="34d2d-151">The following values are not case sensitive:</span></span>|

## <a name="response"></a><span data-ttu-id="34d2d-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="34d2d-152">Response</span></span>

<span data-ttu-id="34d2d-153">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="34d2d-153">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34d2d-154">Пример</span><span class="sxs-lookup"><span data-stu-id="34d2d-154">Example</span></span>

##### <a name="request"></a><span data-ttu-id="34d2d-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="34d2d-155">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="34d2d-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="34d2d-156">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="34d2d-157">C#</span><span class="sxs-lookup"><span data-stu-id="34d2d-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getbyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="34d2d-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="34d2d-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getbyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="34d2d-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="34d2d-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getbyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="34d2d-160">Java</span><span class="sxs-lookup"><span data-stu-id="34d2d-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getbyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="34d2d-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="34d2d-161">Response</span></span>

<span data-ttu-id="34d2d-p107">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="34d2d-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
