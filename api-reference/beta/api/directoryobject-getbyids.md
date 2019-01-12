---
title: Получение объектов каталога из списка идентификаторов
description: Выберите "параметр запроса не поддерживается для этой операции.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 256292a1610972b8a8cbe6026344300af29b1c55
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945975"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="311da-103">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="311da-103">Get directory objects from a list of ids</span></span>

> <span data-ttu-id="311da-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="311da-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="311da-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="311da-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="311da-p102">Возвращает объекты каталогов, указанные в списке идентификаторов.  ПРИМЕЧАНИЕ. Возвращаемые объекты каталогов представляют собой полные объекты, содержащие **все** свойства. Параметр запроса `$select` недоступен для этой операции.</span><span class="sxs-lookup"><span data-stu-id="311da-p102">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="311da-109">Ниже перечислены некоторые распространенные случаи использования этой функции.</span><span class="sxs-lookup"><span data-stu-id="311da-109">Some common uses for this function are to:</span></span>

* <span data-ttu-id="311da-110">Разрешение идентификаторов, возвращаемых как часть коллекций идентификаторов функциями, например [getMemberObjects](/graph/api/directoryobject-getmemberobjects.md?view=graph-rest-beta) или [getMemberGroups](/graph/api/directoryobject-getmembergroups.md?view=graph-rest-beta), в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="311da-110">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](/graph/api/directoryobject-getmemberobjects.md?view=graph-rest-beta) or [getMemberGroups](/graph/api/directoryobject-getmembergroups.md?view=graph-rest-beta)  to their backing directory objects.</span></span>
* <span data-ttu-id="311da-111">Разрешение идентификаторов, которые приложение хранит во внешнем хранилище, в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="311da-111">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="311da-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="311da-112">Permissions</span></span>

<span data-ttu-id="311da-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="311da-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="311da-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="311da-115">Permission type</span></span>      | <span data-ttu-id="311da-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="311da-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="311da-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="311da-117">Delegated (work or school account)</span></span> | <span data-ttu-id="311da-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="311da-118">Directory.Read.All</span></span>    |
|<span data-ttu-id="311da-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="311da-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="311da-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="311da-120">Not supported.</span></span>    |
|<span data-ttu-id="311da-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="311da-121">Application</span></span> | <span data-ttu-id="311da-122">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="311da-122">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="311da-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="311da-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="311da-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="311da-124">Request headers</span></span>

| <span data-ttu-id="311da-125">Имя</span><span class="sxs-lookup"><span data-stu-id="311da-125">Name</span></span>       | <span data-ttu-id="311da-126">Тип</span><span class="sxs-lookup"><span data-stu-id="311da-126">Type</span></span> | <span data-ttu-id="311da-127">Описание</span><span class="sxs-lookup"><span data-stu-id="311da-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="311da-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="311da-128">Authorization</span></span>  | <span data-ttu-id="311da-129">string</span><span class="sxs-lookup"><span data-stu-id="311da-129">string</span></span>  | <span data-ttu-id="311da-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="311da-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="311da-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="311da-132">Content-Type</span></span>  | <span data-ttu-id="311da-133">application/json</span><span class="sxs-lookup"><span data-stu-id="311da-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="311da-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="311da-134">Request body</span></span>

<span data-ttu-id="311da-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="311da-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="311da-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="311da-136">Parameter</span></span>   | <span data-ttu-id="311da-137">Тип</span><span class="sxs-lookup"><span data-stu-id="311da-137">Type</span></span> |<span data-ttu-id="311da-138">Описание</span><span class="sxs-lookup"><span data-stu-id="311da-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="311da-139">ids</span><span class="sxs-lookup"><span data-stu-id="311da-139">ids</span></span>|<span data-ttu-id="311da-140">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="311da-140">String collection</span></span>| <span data-ttu-id="311da-p105">Коллекция идентификаторов, для которой необходимо возвратить объекты. Вы можете указать до 1000 идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="311da-p105">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="311da-143">types</span><span class="sxs-lookup"><span data-stu-id="311da-143">types</span></span>|<span data-ttu-id="311da-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="311da-144">String collection</span></span>| <span data-ttu-id="311da-145">Коллекция типов ресурсов, определяющий набор ресурсов семейств сайтов для поиска.</span><span class="sxs-lookup"><span data-stu-id="311da-145">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="311da-146">Если не указан, по умолчанию — [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), которая содержит все типы ресурсов, определенные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="311da-146">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="311da-147">Любого объекта, производного от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) может быть указано в коллекции; Например: [пользователей](/graph/api/resources/user?view=graph-rest-beta), [группы](/graph/api/resources/group?view=graph-rest-beta), [устройства](/graph/api/resources/device?view=graph-rest-beta)и т. д.</span><span class="sxs-lookup"><span data-stu-id="311da-147">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-beta), [group](/graph/api/resources/group?view=graph-rest-beta), [device](/graph/api/resources/device?view=graph-rest-beta), and so on.</span></span> <span data-ttu-id="311da-148">Для поиска справочных материалов, которые [Поставщик облаке решения](https://partner.microsoft.com/en-us/cloud-solution-provider) партнеров организации задается [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="311da-148">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta).</span></span> <span data-ttu-id="311da-149">Если не указан, по умолчанию — [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), которая содержит все типы ресурсов, определенные в каталоге, за исключением справочные материалы, которые [Поставщик решения облачных](https://partner.microsoft.com/en-us/cloud-solution-provider) партнерской организации.</span><span class="sxs-lookup"><span data-stu-id="311da-149">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="311da-150">Значения не учитывают регистр.</span><span class="sxs-lookup"><span data-stu-id="311da-150">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="311da-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="311da-151">Response</span></span>

<span data-ttu-id="311da-152">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="311da-152">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="311da-153">Пример</span><span class="sxs-lookup"><span data-stu-id="311da-153">Example</span></span>

##### <a name="request"></a><span data-ttu-id="311da-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="311da-154">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="311da-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="311da-155">Response</span></span>

<span data-ttu-id="311da-p107">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="311da-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
