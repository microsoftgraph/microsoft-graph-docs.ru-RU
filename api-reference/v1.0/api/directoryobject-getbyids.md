---
title: Получение объектов каталога из списка идентификаторов
description: Выберите "параметр запроса не поддерживается для этой операции.
author: lleonard-msft
localization_priority: Priority
ms.openlocfilehash: b504fc69deecd6688f61c20c30e17133f80b1dc8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889651"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="4985c-103">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="4985c-103">Get directory objects from a list of ids</span></span>

<span data-ttu-id="4985c-p101">Возвращает объекты каталогов, указанные в списке идентификаторов.  ПРИМЕЧАНИЕ. Возвращаемые объекты каталогов представляют собой полные объекты, содержащие **все** свойства. Параметр запроса `$select` недоступен для этой операции.</span><span class="sxs-lookup"><span data-stu-id="4985c-p101">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="4985c-107">Ниже перечислены некоторые распространенные случаи использования этой функции.</span><span class="sxs-lookup"><span data-stu-id="4985c-107">Some common uses for this function are to:</span></span>

* <span data-ttu-id="4985c-108">Разрешение идентификаторов, возвращаемых как часть коллекций идентификаторов функциями, например [getMemberObjects](directoryobject-getmemberobjects.md) или [getMemberGroups](directoryobject-getmembergroups.md), в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="4985c-108">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](directoryobject-getmemberobjects.md) or [getMemberGroups](directoryobject-getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="4985c-109">Разрешение идентификаторов, которые приложение хранит во внешнем хранилище, в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="4985c-109">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="4985c-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4985c-110">Permissions</span></span>

<span data-ttu-id="4985c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4985c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4985c-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4985c-113">Permission type</span></span>      | <span data-ttu-id="4985c-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4985c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4985c-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4985c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="4985c-116">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4985c-116">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4985c-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4985c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4985c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4985c-118">Not supported.</span></span>    |
|<span data-ttu-id="4985c-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4985c-119">Application</span></span> | <span data-ttu-id="4985c-120">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4985c-120">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4985c-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4985c-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="4985c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4985c-122">Request headers</span></span>

| <span data-ttu-id="4985c-123">Имя</span><span class="sxs-lookup"><span data-stu-id="4985c-123">Name</span></span>       | <span data-ttu-id="4985c-124">Тип</span><span class="sxs-lookup"><span data-stu-id="4985c-124">Type</span></span> | <span data-ttu-id="4985c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="4985c-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4985c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="4985c-126">Authorization</span></span>  | <span data-ttu-id="4985c-127">string</span><span class="sxs-lookup"><span data-stu-id="4985c-127">string</span></span>  | <span data-ttu-id="4985c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4985c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4985c-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4985c-130">Content-Type</span></span>  | <span data-ttu-id="4985c-131">строка</span><span class="sxs-lookup"><span data-stu-id="4985c-131">string</span></span> | <span data-ttu-id="4985c-132">application/json</span><span class="sxs-lookup"><span data-stu-id="4985c-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4985c-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4985c-133">Request body</span></span>

<span data-ttu-id="4985c-134">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4985c-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4985c-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="4985c-135">Parameter</span></span>   | <span data-ttu-id="4985c-136">Тип</span><span class="sxs-lookup"><span data-stu-id="4985c-136">Type</span></span> |<span data-ttu-id="4985c-137">Описание</span><span class="sxs-lookup"><span data-stu-id="4985c-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4985c-138">ids</span><span class="sxs-lookup"><span data-stu-id="4985c-138">ids</span></span>|<span data-ttu-id="4985c-139">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4985c-139">String collection</span></span>| <span data-ttu-id="4985c-p104">Коллекция идентификаторов, для которой необходимо возвратить объекты. Вы можете указать до 1000 идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="4985c-p104">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="4985c-142">types</span><span class="sxs-lookup"><span data-stu-id="4985c-142">types</span></span>|<span data-ttu-id="4985c-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4985c-143">String collection</span></span>| <span data-ttu-id="4985c-144">Коллекция типов ресурсов, определяющий набор ресурсов семейств сайтов для поиска.</span><span class="sxs-lookup"><span data-stu-id="4985c-144">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="4985c-145">Если не указан, по умолчанию — [directoryObject](../resources/directoryobject.md), которая содержит все типы ресурсов, определенные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="4985c-145">If not specified, the default is [directoryObject](../resources/directoryobject.md), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="4985c-146">Любого объекта, производного от `directoryObject` может быть указано в коллекции; Например: [пользователей](../resources/user.md), [группы](../resources/group.md), [устройства](../resources/device.md)и т. д.</span><span class="sxs-lookup"><span data-stu-id="4985c-146">Any object that derives from `directoryObject` may be specified in the collection; for example: [user](../resources/user.md), [group](../resources/group.md), [device](../resources/device.md), and so on.</span></span> <span data-ttu-id="4985c-147">Значения не учитывают регистр.</span><span class="sxs-lookup"><span data-stu-id="4985c-147">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="4985c-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="4985c-148">Response</span></span>

<span data-ttu-id="4985c-149">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4985c-149">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4985c-150">Пример</span><span class="sxs-lookup"><span data-stu-id="4985c-150">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4985c-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="4985c-151">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="4985c-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="4985c-152">Response</span></span>

<span data-ttu-id="4985c-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4985c-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
