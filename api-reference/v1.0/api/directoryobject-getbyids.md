---
title: Получение объектов каталога из списка идентификаторов
description: Выберите "параметр запроса не поддерживается для этой операции.
author: lleonard-msft
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2fab85844d810627ca4e44395477716eb0828ffa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986819"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="cf619-103">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="cf619-103">Get directory objects from a list of ids</span></span>

<span data-ttu-id="cf619-p101">Возвращает объекты каталогов, указанные в списке идентификаторов.  ПРИМЕЧАНИЕ. Возвращаемые объекты каталогов представляют собой полные объекты, содержащие **все** свойства. Параметр запроса `$select` недоступен для этой операции.</span><span class="sxs-lookup"><span data-stu-id="cf619-p101">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="cf619-107">Ниже перечислены некоторые распространенные случаи использования этой функции.</span><span class="sxs-lookup"><span data-stu-id="cf619-107">Some common uses for this function are to:</span></span>

* <span data-ttu-id="cf619-108">Разрешение идентификаторов, возвращаемых как часть коллекций идентификаторов функциями, например [getMemberObjects](directoryobject-getmemberobjects.md) или [getMemberGroups](directoryobject-getmembergroups.md), в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="cf619-108">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](directoryobject-getmemberobjects.md) or [getMemberGroups](directoryobject-getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="cf619-109">Разрешение идентификаторов, которые приложение хранит во внешнем хранилище, в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="cf619-109">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf619-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cf619-110">Permissions</span></span>

<span data-ttu-id="cf619-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf619-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cf619-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf619-113">Permission type</span></span>      | <span data-ttu-id="cf619-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf619-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf619-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf619-115">Delegated (work or school account)</span></span> | <span data-ttu-id="cf619-116">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cf619-116">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cf619-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf619-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf619-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf619-118">Not supported.</span></span>    |
|<span data-ttu-id="cf619-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf619-119">Application</span></span> | <span data-ttu-id="cf619-120">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf619-120">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf619-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf619-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="cf619-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf619-122">Request headers</span></span>

| <span data-ttu-id="cf619-123">Имя</span><span class="sxs-lookup"><span data-stu-id="cf619-123">Name</span></span>       | <span data-ttu-id="cf619-124">Тип</span><span class="sxs-lookup"><span data-stu-id="cf619-124">Type</span></span> | <span data-ttu-id="cf619-125">Описание</span><span class="sxs-lookup"><span data-stu-id="cf619-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cf619-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf619-126">Authorization</span></span>  | <span data-ttu-id="cf619-127">string</span><span class="sxs-lookup"><span data-stu-id="cf619-127">string</span></span>  | <span data-ttu-id="cf619-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf619-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cf619-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cf619-130">Content-Type</span></span>  | <span data-ttu-id="cf619-131">строка</span><span class="sxs-lookup"><span data-stu-id="cf619-131">string</span></span> | <span data-ttu-id="cf619-132">application/json</span><span class="sxs-lookup"><span data-stu-id="cf619-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cf619-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cf619-133">Request body</span></span>

<span data-ttu-id="cf619-134">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="cf619-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cf619-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="cf619-135">Parameter</span></span>   | <span data-ttu-id="cf619-136">Тип</span><span class="sxs-lookup"><span data-stu-id="cf619-136">Type</span></span> |<span data-ttu-id="cf619-137">Описание</span><span class="sxs-lookup"><span data-stu-id="cf619-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cf619-138">ids</span><span class="sxs-lookup"><span data-stu-id="cf619-138">ids</span></span>|<span data-ttu-id="cf619-139">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cf619-139">String collection</span></span>| <span data-ttu-id="cf619-p104">Коллекция идентификаторов, для которой необходимо возвратить объекты. Вы можете указать до 1000 идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="cf619-p104">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="cf619-142">types</span><span class="sxs-lookup"><span data-stu-id="cf619-142">types</span></span>|<span data-ttu-id="cf619-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cf619-143">String collection</span></span>| <span data-ttu-id="cf619-144">Коллекция типов ресурсов, определяющий набор ресурсов семейств сайтов для поиска.</span><span class="sxs-lookup"><span data-stu-id="cf619-144">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="cf619-145">Если не указан, по умолчанию — [directoryObject](../resources/directoryobject.md), которая содержит все типы ресурсов, определенные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="cf619-145">If not specified, the default is [directoryObject](../resources/directoryobject.md), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="cf619-146">Любого объекта, производного от `directoryObject` может быть указано в коллекции; Например: [пользователей](../resources/user.md), [группы](../resources/group.md), [устройства](../resources/device.md)и т. д.</span><span class="sxs-lookup"><span data-stu-id="cf619-146">Any object that derives from `directoryObject` may be specified in the collection; for example: [user](../resources/user.md), [group](../resources/group.md), [device](../resources/device.md), and so on.</span></span> <span data-ttu-id="cf619-147">Значения не учитывают регистр.</span><span class="sxs-lookup"><span data-stu-id="cf619-147">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="cf619-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf619-148">Response</span></span>

<span data-ttu-id="cf619-149">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cf619-149">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf619-150">Пример</span><span class="sxs-lookup"><span data-stu-id="cf619-150">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cf619-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf619-151">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="cf619-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf619-152">Response</span></span>

<span data-ttu-id="cf619-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cf619-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
