---
title: Создание extensionProperty
description: Создайте новый extensionProperty.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: e1266797975a3c516bff86c453cde74ea73767f1
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129102"
---
# <a name="create-extensionproperty"></a><span data-ttu-id="c49ba-103">Создание extensionProperty</span><span class="sxs-lookup"><span data-stu-id="c49ba-103">Create extensionProperty</span></span>

<span data-ttu-id="c49ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c49ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c49ba-105">Создайте новое [определение extensionProperty.](../resources/extensionproperty.md)</span><span class="sxs-lookup"><span data-stu-id="c49ba-105">Create a new [extensionProperty](../resources/extensionproperty.md) definition.</span></span> <span data-ttu-id="c49ba-106">Эту операцию можно использовать для добавления значения настраиваемого свойства к целевому типу объекта, определенному в extensionProperty, с помощью стандартных запросов на создание и обновление целевого объекта.</span><span class="sxs-lookup"><span data-stu-id="c49ba-106">You can use this operation to add a custom property value to the targeted object type defined in the extensionProperty, using standard creation and update requests to the target object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c49ba-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c49ba-107">Permissions</span></span>

<span data-ttu-id="c49ba-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c49ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c49ba-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c49ba-110">Permission type</span></span>      | <span data-ttu-id="c49ba-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c49ba-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c49ba-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c49ba-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c49ba-113">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c49ba-113">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c49ba-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c49ba-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c49ba-115">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c49ba-115">Application.ReadWrite.All</span></span>    |
|<span data-ttu-id="c49ba-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c49ba-116">Application</span></span> | <span data-ttu-id="c49ba-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c49ba-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c49ba-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c49ba-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/extensionProperties
```

## <a name="request-headers"></a><span data-ttu-id="c49ba-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c49ba-119">Request headers</span></span>
| <span data-ttu-id="c49ba-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c49ba-120">Name</span></span>       | <span data-ttu-id="c49ba-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c49ba-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="c49ba-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c49ba-122">Authorization</span></span>  | <span data-ttu-id="c49ba-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c49ba-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c49ba-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c49ba-125">Content-Type</span></span> | <span data-ttu-id="c49ba-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c49ba-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c49ba-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c49ba-128">Request body</span></span>

<span data-ttu-id="c49ba-129">В теле запроса [укажите объект extensionProperty](../resources/extensionproperty.md) следующими свойствами.</span><span class="sxs-lookup"><span data-stu-id="c49ba-129">In the request body, provide an [extensionProperty](../resources/extensionproperty.md) object with the following properties.</span></span>


| <span data-ttu-id="c49ba-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c49ba-130">Property</span></span>     | <span data-ttu-id="c49ba-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c49ba-131">Type</span></span>        | <span data-ttu-id="c49ba-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c49ba-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c49ba-133">dataType</span><span class="sxs-lookup"><span data-stu-id="c49ba-133">dataType</span></span>|<span data-ttu-id="c49ba-134">String</span><span class="sxs-lookup"><span data-stu-id="c49ba-134">String</span></span>| <span data-ttu-id="c49ba-135">Указывает тип данных значения, в который может вметь свойство расширения.</span><span class="sxs-lookup"><span data-stu-id="c49ba-135">Specifies the data type of the value the extension property can hold.</span></span> <span data-ttu-id="c49ba-136">Поддерживаются следующие значения.</span><span class="sxs-lookup"><span data-stu-id="c49ba-136">Following values are supported.</span></span> <span data-ttu-id="c49ba-137">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="c49ba-137">Not nullable.</span></span> <ul><li><span data-ttu-id="c49ba-138">`Binary` - Не более 256байт</span><span class="sxs-lookup"><span data-stu-id="c49ba-138">`Binary` - 256 bytes maximum</span></span></li><li>`Boolean`</li><li><span data-ttu-id="c49ba-139">`DateTime` - Должен быть указан в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="c49ba-139">`DateTime` - Must be specified in ISO 8601 format.</span></span> <span data-ttu-id="c49ba-140">Данные времени будут храниться в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="c49ba-140">Will be stored in UTC.</span></span></li><li><span data-ttu-id="c49ba-141">`Integer` - 32-битное значение.</span><span class="sxs-lookup"><span data-stu-id="c49ba-141">`Integer` - 32-bit value.</span></span></li><li><span data-ttu-id="c49ba-142">`LargeInteger` - 64-битное значение.</span><span class="sxs-lookup"><span data-stu-id="c49ba-142">`LargeInteger` - 64-bit value.</span></span></li><li><span data-ttu-id="c49ba-143">`String` — не более 256 символов</span><span class="sxs-lookup"><span data-stu-id="c49ba-143">`String` - 256 characters maximum</span></span></li></ul>|
|<span data-ttu-id="c49ba-144">name</span><span class="sxs-lookup"><span data-stu-id="c49ba-144">name</span></span>|<span data-ttu-id="c49ba-145">String</span><span class="sxs-lookup"><span data-stu-id="c49ba-145">String</span></span>| <span data-ttu-id="c49ba-146">Имя свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="c49ba-146">Name of the extension property.</span></span> <span data-ttu-id="c49ba-147">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="c49ba-147">Not nullable.</span></span> |
|<span data-ttu-id="c49ba-148">targetObjects</span><span class="sxs-lookup"><span data-stu-id="c49ba-148">targetObjects</span></span>|<span data-ttu-id="c49ba-149">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="c49ba-149">String collection</span></span>| <span data-ttu-id="c49ba-150">Поддерживаются следующие значения.</span><span class="sxs-lookup"><span data-stu-id="c49ba-150">Following values are supported.</span></span> <span data-ttu-id="c49ba-151">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="c49ba-151">Not nullable.</span></span> <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|


## <a name="response"></a><span data-ttu-id="c49ba-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="c49ba-152">Response</span></span>

<span data-ttu-id="c49ba-153">В случае успеха этот метод возвращает код отклика и новый `201, Created` [объект extensionProperty](../resources/extensionproperty.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c49ba-153">If successful, this method returns `201, Created` response code and a new [extensionProperty](../resources/extensionproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c49ba-154">Примеры</span><span class="sxs-lookup"><span data-stu-id="c49ba-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c49ba-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="c49ba-155">Request</span></span>

<span data-ttu-id="c49ba-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c49ba-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c49ba-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="c49ba-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_extensionproperty_from_application"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/extensionProperties
Content-type: application/json

{
    "name": "extensionName",
    "dataType": "string",
    "targetObjects": [
        "Application"
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="c49ba-158">C#</span><span class="sxs-lookup"><span data-stu-id="c49ba-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-extensionproperty-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c49ba-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c49ba-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-extensionproperty-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c49ba-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c49ba-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-extensionproperty-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c49ba-161">Java</span><span class="sxs-lookup"><span data-stu-id="c49ba-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-extensionproperty-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c49ba-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="c49ba-162">Response</span></span>

<span data-ttu-id="c49ba-163">В случае успеха этот метод возвращает код отклика и объект `201 Created` [extensionProperty](../resources/extensionProperty.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c49ba-163">If successful, this method returns a `201 Created` response code and an [extensionProperty](../resources/extensionProperty.md) object in the response body.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.extensionProperty"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "a2c459db-f5dc-4328-ae9b-118e88d04d19",
    "deletedDateTime": null,
    "appDisplayName": "Display name",
    "name": "extension_b3efaf8f68a44275abcff28ef86b2ee3_extensionName",
    "dataType": "String",
    "isSyncedFromOnPremises": false,
    "targetObjects": [
        "Application"
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create extensionProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



