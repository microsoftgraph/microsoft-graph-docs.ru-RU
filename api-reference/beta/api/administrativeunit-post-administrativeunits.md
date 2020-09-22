---
title: Создание administrativeUnit
description: Используйте этот API для создания нового administrativeUnit.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d939dc871a1a22aa426a621470fa5ebaa227e1a8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997237"
---
# <a name="create-administrativeunit"></a><span data-ttu-id="5fc69-103">Создание administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="5fc69-103">Create administrativeUnit</span></span>

<span data-ttu-id="5fc69-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fc69-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fc69-105">Используйте этот API для создания нового [administrativeUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="5fc69-105">Use this API to create a new [administrativeUnit](../resources/administrativeunit.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="5fc69-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5fc69-106">Permissions</span></span>
<span data-ttu-id="5fc69-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fc69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5fc69-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5fc69-109">Permission type</span></span>      | <span data-ttu-id="5fc69-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5fc69-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5fc69-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5fc69-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5fc69-112">AdministrativeUnit. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="5fc69-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5fc69-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5fc69-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5fc69-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fc69-114">Not supported.</span></span>    |
|<span data-ttu-id="5fc69-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5fc69-115">Application</span></span> | <span data-ttu-id="5fc69-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fc69-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5fc69-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5fc69-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits

```
## <a name="request-headers"></a><span data-ttu-id="5fc69-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5fc69-118">Request headers</span></span>
| <span data-ttu-id="5fc69-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5fc69-119">Name</span></span>      |<span data-ttu-id="5fc69-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5fc69-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5fc69-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5fc69-121">Authorization</span></span>  | <span data-ttu-id="5fc69-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5fc69-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5fc69-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5fc69-124">Content-type</span></span> | <span data-ttu-id="5fc69-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5fc69-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5fc69-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5fc69-127">Request body</span></span>
<span data-ttu-id="5fc69-128">В тексте запроса добавьте представление объекта [administrativeUnit](../resources/administrativeunit.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5fc69-128">In the request body, supply a JSON representation of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="5fc69-129">Так как ресурс **administrativeUnit** поддерживает [расширения](/graph/extensibility-overview), вы можете использовать `POST` операцию и добавлять настраиваемые свойства с собственными данными в административную единицу при создании.</span><span class="sxs-lookup"><span data-stu-id="5fc69-129">Because the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the administrative unit while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="5fc69-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="5fc69-130">Response</span></span>

<span data-ttu-id="5fc69-131">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [administrativeUnit](../resources/administrativeunit.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5fc69-131">If successful, this method returns a `201 Created` response code and an [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fc69-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5fc69-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5fc69-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5fc69-133">Request</span></span>

<span data-ttu-id="5fc69-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5fc69-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5fc69-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5fc69-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_administrativeunit_from_administrativeunits"
}-->
```http
POST https://graph.microsoft.com/beta/administrativeUnits
Content-type: application/json
Content-length: 150

{
    "displayName": "Seattle District Technical Schools",
    "description": "Seattle district technical schools administration",
    "visibility": "HiddenMembership"
}
```
# <a name="c"></a>[<span data-ttu-id="5fc69-136">C#</span><span class="sxs-lookup"><span data-stu-id="5fc69-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-administrativeunit-from-administrativeunits-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5fc69-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5fc69-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-administrativeunit-from-administrativeunits-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5fc69-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5fc69-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-administrativeunit-from-administrativeunits-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="5fc69-139">В тексте запроса добавьте представление объекта [administrativeUnit](../resources/administrativeunit.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5fc69-139">In the request body, supply a JSON representation of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="5fc69-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="5fc69-140">Response</span></span>

<span data-ttu-id="5fc69-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5fc69-141">The following is an example of the response.</span></span> 
> <span data-ttu-id="5fc69-142">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5fc69-142">Note: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5fc69-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5fc69-143">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 172

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#administrativeUnits/$entity",
    "id": "7a3dc8f3-b3a0-4164-9a99-ed36f3af039f",
    "deletedDateTime": null,
    "displayName": "Seattle District Technical Schools",
    "description": "Seattle district technical schools administration",
    "visibility": "HiddenMembership"
}
```

## <a name="see-also"></a><span data-ttu-id="5fc69-144">См. также</span><span class="sxs-lookup"><span data-stu-id="5fc69-144">See also</span></span>

- [<span data-ttu-id="5fc69-145">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="5fc69-145">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="5fc69-146">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="5fc69-146">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


