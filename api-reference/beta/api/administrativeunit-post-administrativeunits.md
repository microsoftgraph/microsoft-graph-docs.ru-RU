---
title: Создание administrativeUnit
description: Используйте этот API для создания нового администратораUnit.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 898b8a2c63310743a6c2fcfec3c044d96d5b4f57
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048241"
---
# <a name="create-administrativeunit"></a><span data-ttu-id="3fa67-103">Создание administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="3fa67-103">Create administrativeUnit</span></span>

<span data-ttu-id="3fa67-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fa67-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3fa67-105">Используйте этот API для создания нового [администратораUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="3fa67-105">Use this API to create a new [administrativeUnit](../resources/administrativeunit.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="3fa67-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3fa67-106">Permissions</span></span>
<span data-ttu-id="3fa67-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fa67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3fa67-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3fa67-109">Permission type</span></span>      | <span data-ttu-id="3fa67-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3fa67-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3fa67-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3fa67-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3fa67-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3fa67-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3fa67-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3fa67-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3fa67-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fa67-114">Not supported.</span></span>    |
|<span data-ttu-id="3fa67-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="3fa67-115">Application</span></span> | <span data-ttu-id="3fa67-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fa67-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3fa67-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3fa67-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits

```
## <a name="request-headers"></a><span data-ttu-id="3fa67-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3fa67-118">Request headers</span></span>
| <span data-ttu-id="3fa67-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3fa67-119">Name</span></span>      |<span data-ttu-id="3fa67-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3fa67-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3fa67-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3fa67-121">Authorization</span></span>  | <span data-ttu-id="3fa67-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fa67-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3fa67-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3fa67-124">Content-type</span></span> | <span data-ttu-id="3fa67-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fa67-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3fa67-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3fa67-127">Request body</span></span>
<span data-ttu-id="3fa67-128">В теле запроса поставляем представление JSON объекта [administrativeUnit.](../resources/administrativeunit.md)</span><span class="sxs-lookup"><span data-stu-id="3fa67-128">In the request body, supply a JSON representation of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="3fa67-129">Так как **ресурс administrativeUnit** поддерживает [расширения,](/graph/extensibility-overview)можно использовать операцию и добавлять настраиваемые свойства с собственными данными в административный блок при `POST` его создании.</span><span class="sxs-lookup"><span data-stu-id="3fa67-129">Because the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the administrative unit while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="3fa67-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fa67-130">Response</span></span>

<span data-ttu-id="3fa67-131">В случае успешной работы этот метод возвращает код ответа и `201 Created` объект [administrativeUnit](../resources/administrativeunit.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3fa67-131">If successful, this method returns a `201 Created` response code and an [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fa67-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3fa67-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3fa67-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3fa67-133">Request</span></span>

<span data-ttu-id="3fa67-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3fa67-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3fa67-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3fa67-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3fa67-136">C#</span><span class="sxs-lookup"><span data-stu-id="3fa67-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-administrativeunit-from-administrativeunits-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3fa67-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3fa67-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-administrativeunit-from-administrativeunits-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3fa67-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3fa67-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-administrativeunit-from-administrativeunits-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3fa67-139">Java</span><span class="sxs-lookup"><span data-stu-id="3fa67-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-administrativeunit-from-administrativeunits-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="3fa67-140">В теле запроса поставляем представление JSON объекта [administrativeUnit.](../resources/administrativeunit.md)</span><span class="sxs-lookup"><span data-stu-id="3fa67-140">In the request body, supply a JSON representation of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="3fa67-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fa67-141">Response</span></span>

<span data-ttu-id="3fa67-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3fa67-142">The following is an example of the response.</span></span> 
> <span data-ttu-id="3fa67-143">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3fa67-143">Note: The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="3fa67-144">См. также</span><span class="sxs-lookup"><span data-stu-id="3fa67-144">See also</span></span>

- [<span data-ttu-id="3fa67-145">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="3fa67-145">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="3fa67-146">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="3fa67-146">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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


