---
title: Получение объектов каталога из списка идентификаторов
description: Параметр запроса select недоступен для этой операции.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 71bb9a63318dd586021dfdb2b0e3e2ddd4737630
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33326027"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="e6329-103">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="e6329-103">Get directory objects from a list of ids</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6329-p101">Возвращает объекты каталогов, указанные в списке идентификаторов.  ПРИМЕЧАНИЕ. Возвращаемые объекты каталогов представляют собой полные объекты, содержащие **все** свойства. Параметр запроса `$select` недоступен для этой операции.</span><span class="sxs-lookup"><span data-stu-id="e6329-p101">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="e6329-107">Ниже перечислены некоторые распространенные случаи использования этой функции.</span><span class="sxs-lookup"><span data-stu-id="e6329-107">Some common uses for this function are to:</span></span>

* <span data-ttu-id="e6329-108">Разрешение идентификаторов, возвращаемых как часть коллекций идентификаторов функциями, например [getMemberObjects](/graph/api/directoryobject-getmemberobjects.md?view=graph-rest-beta) или [getMemberGroups](/graph/api/directoryobject-getmembergroups.md?view=graph-rest-beta), в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="e6329-108">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](/graph/api/directoryobject-getmemberobjects.md?view=graph-rest-beta) or [getMemberGroups](/graph/api/directoryobject-getmembergroups.md?view=graph-rest-beta)  to their backing directory objects.</span></span>
* <span data-ttu-id="e6329-109">Разрешение идентификаторов, которые приложение хранит во внешнем хранилище, в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="e6329-109">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6329-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e6329-110">Permissions</span></span>

<span data-ttu-id="e6329-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6329-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e6329-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6329-113">Permission type</span></span>      | <span data-ttu-id="e6329-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6329-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6329-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6329-115">Delegated (work or school account)</span></span> | <span data-ttu-id="e6329-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6329-116">Directory.Read.All</span></span>    |
|<span data-ttu-id="e6329-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6329-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6329-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6329-118">Not supported.</span></span>    |
|<span data-ttu-id="e6329-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6329-119">Application</span></span> | <span data-ttu-id="e6329-120">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6329-120">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6329-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6329-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="e6329-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6329-122">Request headers</span></span>

| <span data-ttu-id="e6329-123">Имя</span><span class="sxs-lookup"><span data-stu-id="e6329-123">Name</span></span>       | <span data-ttu-id="e6329-124">Тип</span><span class="sxs-lookup"><span data-stu-id="e6329-124">Type</span></span> | <span data-ttu-id="e6329-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e6329-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e6329-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6329-126">Authorization</span></span>  | <span data-ttu-id="e6329-127">string</span><span class="sxs-lookup"><span data-stu-id="e6329-127">string</span></span>  | <span data-ttu-id="e6329-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6329-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e6329-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e6329-130">Content-Type</span></span>  | <span data-ttu-id="e6329-131">application/json</span><span class="sxs-lookup"><span data-stu-id="e6329-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e6329-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e6329-132">Request body</span></span>

<span data-ttu-id="e6329-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e6329-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e6329-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="e6329-134">Parameter</span></span>   | <span data-ttu-id="e6329-135">Тип</span><span class="sxs-lookup"><span data-stu-id="e6329-135">Type</span></span> |<span data-ttu-id="e6329-136">Описание</span><span class="sxs-lookup"><span data-stu-id="e6329-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6329-137">ids</span><span class="sxs-lookup"><span data-stu-id="e6329-137">ids</span></span>|<span data-ttu-id="e6329-138">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e6329-138">String collection</span></span>| <span data-ttu-id="e6329-p104">Коллекция идентификаторов, для которой необходимо возвратить объекты. Вы можете указать до 1000 идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="e6329-p104">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="e6329-141">types</span><span class="sxs-lookup"><span data-stu-id="e6329-141">types</span></span>|<span data-ttu-id="e6329-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="e6329-142">String collection</span></span>| <span data-ttu-id="e6329-143">Коллекция типов ресурсов, указывающая набор коллекций ресурсов, в котором необходимо выполнить поиск.</span><span class="sxs-lookup"><span data-stu-id="e6329-143">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="e6329-144">Если аргумент не указан, по умолчанию используется объект [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), который содержит все типы ресурсов, определенные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="e6329-144">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="e6329-145">В коллекции можно указать любой объект, производный от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta). Пример: [user](/graph/api/resources/user?view=graph-rest-beta), [group](/graph/api/resources/group?view=graph-rest-beta), [device](/graph/api/resources/device?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="e6329-145">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-beta), [group](/graph/api/resources/group?view=graph-rest-beta), [device](/graph/api/resources/device?view=graph-rest-beta), and so on.</span></span> <span data-ttu-id="e6329-146">Для поиска ссылок на партнерскую организацию, [поставляющую облачные решения](https://partner.microsoft.com/en-us/cloud-solution-provider), укажите ресурс [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="e6329-146">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta).</span></span> <span data-ttu-id="e6329-147">Если аргумент не указан, по умолчанию используется объект [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), который содержит все типы ресурсов, определенные в каталоге, кроме ссылок на партнерскую организацию, [поставляющую облачные решения](https://partner.microsoft.com/en-us/cloud-solution-provider).</span><span class="sxs-lookup"><span data-stu-id="e6329-147">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="e6329-148">В значениях не учитывается регистр символов.</span><span class="sxs-lookup"><span data-stu-id="e6329-148">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="e6329-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6329-149">Response</span></span>

<span data-ttu-id="e6329-150">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e6329-150">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6329-151">Пример</span><span class="sxs-lookup"><span data-stu-id="e6329-151">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e6329-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6329-152">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="e6329-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6329-153">Response</span></span>

<span data-ttu-id="e6329-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e6329-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->
