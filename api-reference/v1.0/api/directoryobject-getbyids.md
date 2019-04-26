---
title: Получение объектов каталога из списка идентификаторов
description: Параметр запроса select недоступен для этой операции.
author: lleonard-msft
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a209d391c72edd453bbfe9232b7d02121ca98128
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572012"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="c2f88-103">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="c2f88-103">Get directory objects from a list of ids</span></span>

<span data-ttu-id="c2f88-p101">Возвращает объекты каталогов, указанные в списке идентификаторов.  ПРИМЕЧАНИЕ. Возвращаемые объекты каталогов представляют собой полные объекты, содержащие **все** свойства. Параметр запроса `$select` недоступен для этой операции.</span><span class="sxs-lookup"><span data-stu-id="c2f88-p101">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="c2f88-107">Ниже перечислены некоторые распространенные случаи использования этой функции.</span><span class="sxs-lookup"><span data-stu-id="c2f88-107">Some common uses for this function are to:</span></span>

* <span data-ttu-id="c2f88-108">Разрешение идентификаторов, возвращаемых как часть коллекций идентификаторов функциями, например [getMemberObjects](directoryobject-getmemberobjects.md) или [getMemberGroups](directoryobject-getmembergroups.md), в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="c2f88-108">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](directoryobject-getmemberobjects.md) or [getMemberGroups](directoryobject-getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="c2f88-109">Разрешение идентификаторов, которые приложение хранит во внешнем хранилище, в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="c2f88-109">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2f88-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2f88-110">Permissions</span></span>

<span data-ttu-id="c2f88-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2f88-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c2f88-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2f88-113">Permission type</span></span>      | <span data-ttu-id="c2f88-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2f88-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2f88-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2f88-115">Delegated (work or school account)</span></span> | <span data-ttu-id="c2f88-116">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c2f88-116">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c2f88-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2f88-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2f88-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2f88-118">Not supported.</span></span>    |
|<span data-ttu-id="c2f88-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2f88-119">Application</span></span> | <span data-ttu-id="c2f88-120">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2f88-120">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2f88-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2f88-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="c2f88-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2f88-122">Request headers</span></span>

| <span data-ttu-id="c2f88-123">Имя</span><span class="sxs-lookup"><span data-stu-id="c2f88-123">Name</span></span>       | <span data-ttu-id="c2f88-124">Тип</span><span class="sxs-lookup"><span data-stu-id="c2f88-124">Type</span></span> | <span data-ttu-id="c2f88-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c2f88-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c2f88-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2f88-126">Authorization</span></span>  | <span data-ttu-id="c2f88-127">string</span><span class="sxs-lookup"><span data-stu-id="c2f88-127">string</span></span>  | <span data-ttu-id="c2f88-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2f88-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c2f88-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c2f88-130">Content-Type</span></span>  | <span data-ttu-id="c2f88-131">string</span><span class="sxs-lookup"><span data-stu-id="c2f88-131">string</span></span> | <span data-ttu-id="c2f88-132">application/json</span><span class="sxs-lookup"><span data-stu-id="c2f88-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c2f88-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c2f88-133">Request body</span></span>

<span data-ttu-id="c2f88-134">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c2f88-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c2f88-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="c2f88-135">Parameter</span></span>   | <span data-ttu-id="c2f88-136">Тип</span><span class="sxs-lookup"><span data-stu-id="c2f88-136">Type</span></span> |<span data-ttu-id="c2f88-137">Описание</span><span class="sxs-lookup"><span data-stu-id="c2f88-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2f88-138">ids</span><span class="sxs-lookup"><span data-stu-id="c2f88-138">ids</span></span>|<span data-ttu-id="c2f88-139">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c2f88-139">String collection</span></span>| <span data-ttu-id="c2f88-p104">Коллекция идентификаторов, для которой необходимо возвратить объекты. Вы можете указать до 1000 идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="c2f88-p104">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="c2f88-142">types</span><span class="sxs-lookup"><span data-stu-id="c2f88-142">types</span></span>|<span data-ttu-id="c2f88-143">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="c2f88-143">String collection</span></span>| <span data-ttu-id="c2f88-144">Коллекция типов ресурсов, указывающая набор коллекций ресурсов, в котором необходимо выполнить поиск.</span><span class="sxs-lookup"><span data-stu-id="c2f88-144">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="c2f88-145">Если аргумент не указан, по умолчанию используется объект [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), который содержит все типы ресурсов, определенные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="c2f88-145">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="c2f88-146">В коллекции можно указать любой объект, производный от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0). Пример: [user](/graph/api/resources/user?view=graph-rest-v1.0), [group](/graph/api/resources/group?view=graph-rest-v1.0), [device](/graph/api/resources/device?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="c2f88-146">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-v1.0), [group](/graph/api/resources/group?view=graph-rest-v1.0), [device](/graph/api/resources/device?view=graph-rest-v1.0), and so on.</span></span> <span data-ttu-id="c2f88-147">Для поиска ссылок на партнерскую организацию, [поставляющую облачные решения](https://partner.microsoft.com/ru-RU/cloud-solution-provider), укажите ресурс [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="c2f88-147">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/ru-RU/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0).</span></span> <span data-ttu-id="c2f88-148">Если аргумент не указан, по умолчанию используется объект [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), который содержит все типы ресурсов, определенные в каталоге, кроме ссылок на партнерскую организацию, [поставляющую облачные решения](https://partner.microsoft.com/ru-RU/cloud-solution-provider).</span><span class="sxs-lookup"><span data-stu-id="c2f88-148">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/ru-RU/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="c2f88-149">В значениях не учитывается регистр символов.</span><span class="sxs-lookup"><span data-stu-id="c2f88-149">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="c2f88-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2f88-150">Response</span></span>

<span data-ttu-id="c2f88-151">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c2f88-151">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2f88-152">Пример</span><span class="sxs-lookup"><span data-stu-id="c2f88-152">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c2f88-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2f88-153">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="c2f88-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2f88-154">Response</span></span>

<span data-ttu-id="c2f88-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2f88-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
