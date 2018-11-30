---
title: Получение объектов каталога из списка идентификаторов
description: Выберите "параметр запроса не поддерживается для этой операции.
ms.openlocfilehash: 87fa774910c1ea6795b6df65ee0f5538d12296bb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075736"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="fe04c-103">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="fe04c-103">Get directory objects from a list of ids</span></span>

> <span data-ttu-id="fe04c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fe04c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe04c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe04c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fe04c-p102">Возвращает объекты каталогов, указанные в списке идентификаторов.  ПРИМЕЧАНИЕ. Возвращаемые объекты каталогов представляют собой полные объекты, содержащие **все** свойства. Параметр запроса `$select` недоступен для этой операции.</span><span class="sxs-lookup"><span data-stu-id="fe04c-p102">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="fe04c-109">Ниже перечислены некоторые распространенные случаи использования этой функции.</span><span class="sxs-lookup"><span data-stu-id="fe04c-109">Some common uses for this function are to:</span></span>

* <span data-ttu-id="fe04c-110">Разрешение идентификаторов, возвращаемых как часть коллекций идентификаторов функциями, например [getMemberObjects](directoryobject-getmemberobjects.md) или [getMemberGroups](directoryobject-getmembergroups.md), в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="fe04c-110">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](directoryobject-getmemberobjects.md) or [getMemberGroups](directoryobject-getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="fe04c-111">Разрешение идентификаторов, которые приложение хранит во внешнем хранилище, в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="fe04c-111">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe04c-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fe04c-112">Permissions</span></span>

<span data-ttu-id="fe04c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe04c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fe04c-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe04c-115">Permission type</span></span>      | <span data-ttu-id="fe04c-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe04c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe04c-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe04c-117">Delegated (work or school account)</span></span> | <span data-ttu-id="fe04c-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe04c-118">Directory.Read.All</span></span>    |
|<span data-ttu-id="fe04c-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe04c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe04c-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe04c-120">Not supported.</span></span>    |
|<span data-ttu-id="fe04c-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe04c-121">Application</span></span> | <span data-ttu-id="fe04c-122">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe04c-122">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe04c-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe04c-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getById
```

## <a name="request-headers"></a><span data-ttu-id="fe04c-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe04c-124">Request headers</span></span>

| <span data-ttu-id="fe04c-125">Имя</span><span class="sxs-lookup"><span data-stu-id="fe04c-125">Name</span></span>       | <span data-ttu-id="fe04c-126">Тип</span><span class="sxs-lookup"><span data-stu-id="fe04c-126">Type</span></span> | <span data-ttu-id="fe04c-127">Описание</span><span class="sxs-lookup"><span data-stu-id="fe04c-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fe04c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe04c-128">Authorization</span></span>  | <span data-ttu-id="fe04c-129">string</span><span class="sxs-lookup"><span data-stu-id="fe04c-129">string</span></span>  | <span data-ttu-id="fe04c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe04c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fe04c-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fe04c-132">Content-Type</span></span>  | <span data-ttu-id="fe04c-133">application/json</span><span class="sxs-lookup"><span data-stu-id="fe04c-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fe04c-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe04c-134">Request body</span></span>

<span data-ttu-id="fe04c-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="fe04c-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fe04c-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="fe04c-136">Parameter</span></span>   | <span data-ttu-id="fe04c-137">Тип</span><span class="sxs-lookup"><span data-stu-id="fe04c-137">Type</span></span> |<span data-ttu-id="fe04c-138">Описание</span><span class="sxs-lookup"><span data-stu-id="fe04c-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe04c-139">ids</span><span class="sxs-lookup"><span data-stu-id="fe04c-139">ids</span></span>|<span data-ttu-id="fe04c-140">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fe04c-140">String collection</span></span>| <span data-ttu-id="fe04c-p105">Коллекция идентификаторов, для которой необходимо возвратить объекты. Вы можете указать до 1000 идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="fe04c-p105">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="fe04c-143">types</span><span class="sxs-lookup"><span data-stu-id="fe04c-143">types</span></span>|<span data-ttu-id="fe04c-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fe04c-144">String collection</span></span>| <span data-ttu-id="fe04c-145">Коллекция типов ресурсов, определяющий набор ресурсов семейств сайтов для поиска.</span><span class="sxs-lookup"><span data-stu-id="fe04c-145">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="fe04c-146">Если не указан, по умолчанию — [directoryObject](../resources/directoryobject.md), которая содержит все типы ресурсов, определенные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="fe04c-146">If not specified, the default is [directoryObject](../resources/directoryobject.md), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="fe04c-147">Любого объекта, производного от `directoryObject` может быть указано в коллекции; Например: [пользователей](../resources/user.md), [группы](../resources/group.md), [устройства](../resources/device.md)и т. д.</span><span class="sxs-lookup"><span data-stu-id="fe04c-147">Any object that derives from `directoryObject` may be specified in the collection; for example: [user](../resources/user.md), [group](../resources/group.md), [device](../resources/device.md), and so on.</span></span> <span data-ttu-id="fe04c-148">Значения не учитывают регистр.</span><span class="sxs-lookup"><span data-stu-id="fe04c-148">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="fe04c-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe04c-149">Response</span></span>

<span data-ttu-id="fe04c-150">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fe04c-150">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe04c-151">Пример</span><span class="sxs-lookup"><span data-stu-id="fe04c-151">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fe04c-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe04c-152">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getById"
}-->

```http
POST https://graph.microsoft.com/beta/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893-8749-40a3-97b7-68513b600544","5d6059b6-368d-45f8-91e1-8e07d485f1d0"],
    "types":["user"]
}
```

##### <a name="response"></a><span data-ttu-id="fe04c-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe04c-153">Response</span></span>

<span data-ttu-id="fe04c-p107">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fe04c-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
