---
title: Создание Екстенсионпроперти
description: Создание нового Екстенсионпроперти.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e4cf815d66311dd022297c9c4e716e77f4e2acaa
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998993"
---
# <a name="create-extensionproperty"></a><span data-ttu-id="4db9c-103">Создание Екстенсионпроперти</span><span class="sxs-lookup"><span data-stu-id="4db9c-103">Create extensionProperty</span></span>

<span data-ttu-id="4db9c-104">Создайте новое определение [екстенсионпроперти](../resources/extensionproperty.md) .</span><span class="sxs-lookup"><span data-stu-id="4db9c-104">Create a new [extensionProperty](../resources/extensionproperty.md) definition.</span></span> <span data-ttu-id="4db9c-105">Эту операцию можно использовать для добавления настраиваемого значения свойства в целевой тип объекта, определенный в **екстенсионпроперти**, с помощью стандартных запросов на создание и обновление целевого объекта.</span><span class="sxs-lookup"><span data-stu-id="4db9c-105">You can use this operation to add a custom property value to the targeted object type defined in the **extensionProperty**, using standard creation and update requests to the target object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4db9c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4db9c-106">Permissions</span></span>

<span data-ttu-id="4db9c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4db9c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4db9c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4db9c-109">Permission type</span></span>      | <span data-ttu-id="4db9c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4db9c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4db9c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4db9c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4db9c-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4db9c-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4db9c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4db9c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4db9c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4db9c-114">Not supported.</span></span>    |
|<span data-ttu-id="4db9c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4db9c-115">Application</span></span> | <span data-ttu-id="4db9c-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4db9c-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4db9c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4db9c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/extensionProperties
```

## <a name="request-headers"></a><span data-ttu-id="4db9c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4db9c-118">Request headers</span></span>
| <span data-ttu-id="4db9c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4db9c-119">Name</span></span>       | <span data-ttu-id="4db9c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4db9c-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="4db9c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4db9c-121">Authorization</span></span>  | <span data-ttu-id="4db9c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4db9c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4db9c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4db9c-124">Content-type</span></span> | <span data-ttu-id="4db9c-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4db9c-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4db9c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4db9c-127">Request body</span></span>

<span data-ttu-id="4db9c-128">В тексте запроса укажите объект [екстенсионпроперти](../resources/extensionproperty.md) со следующими свойствами.</span><span class="sxs-lookup"><span data-stu-id="4db9c-128">In the request body, provide an [extensionProperty](../resources/extensionproperty.md) object with the following properties.</span></span>


| <span data-ttu-id="4db9c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4db9c-129">Property</span></span>     | <span data-ttu-id="4db9c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4db9c-130">Type</span></span>        | <span data-ttu-id="4db9c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4db9c-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4db9c-132">dataType</span><span class="sxs-lookup"><span data-stu-id="4db9c-132">dataType</span></span>|<span data-ttu-id="4db9c-133">String</span><span class="sxs-lookup"><span data-stu-id="4db9c-133">String</span></span>| <span data-ttu-id="4db9c-134">Задает тип данных значения, которое может содержать свойство Extension.</span><span class="sxs-lookup"><span data-stu-id="4db9c-134">Specifies the data type of the value the extension property can hold.</span></span> <span data-ttu-id="4db9c-135">Поддерживаются следующие значения:</span><span class="sxs-lookup"><span data-stu-id="4db9c-135">Following values are supported.</span></span> <span data-ttu-id="4db9c-136">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="4db9c-136">Not nullable.</span></span> <ul><li><span data-ttu-id="4db9c-137">`Binary`– 256 байт (максимум)</span><span class="sxs-lookup"><span data-stu-id="4db9c-137">`Binary` - 256 bytes maximum</span></span></li><li>`Boolean`</li><li><span data-ttu-id="4db9c-138">`DateTime`-Должен быть указан в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="4db9c-138">`DateTime` - Must be specified in ISO 8601 format.</span></span> <span data-ttu-id="4db9c-139">Данные времени будут храниться в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="4db9c-139">Will be stored in UTC.</span></span></li><li><span data-ttu-id="4db9c-140">`Integer`— значение 32 — бит.</span><span class="sxs-lookup"><span data-stu-id="4db9c-140">`Integer` - 32-bit value.</span></span></li><li><span data-ttu-id="4db9c-141">`LargeInteger`— значение 64 — бит.</span><span class="sxs-lookup"><span data-stu-id="4db9c-141">`LargeInteger` - 64-bit value.</span></span></li><li><span data-ttu-id="4db9c-142">`String`– 256 символов максимум</span><span class="sxs-lookup"><span data-stu-id="4db9c-142">`String` - 256 characters maximum</span></span></li></ul>|
|<span data-ttu-id="4db9c-143">name</span><span class="sxs-lookup"><span data-stu-id="4db9c-143">name</span></span>|<span data-ttu-id="4db9c-144">String</span><span class="sxs-lookup"><span data-stu-id="4db9c-144">String</span></span>| <span data-ttu-id="4db9c-145">Имя свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="4db9c-145">Name of the extension property.</span></span> <span data-ttu-id="4db9c-146">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="4db9c-146">Not nullable.</span></span> |
|<span data-ttu-id="4db9c-147">таржетобжектс</span><span class="sxs-lookup"><span data-stu-id="4db9c-147">targetObjects</span></span>|<span data-ttu-id="4db9c-148">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4db9c-148">String collection</span></span>| <span data-ttu-id="4db9c-149">Поддерживаются следующие значения:</span><span class="sxs-lookup"><span data-stu-id="4db9c-149">Following values are supported.</span></span> <span data-ttu-id="4db9c-150">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="4db9c-150">Not nullable.</span></span> <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|


## <a name="response"></a><span data-ttu-id="4db9c-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="4db9c-151">Response</span></span>

<span data-ttu-id="4db9c-152">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [екстенсионпроперти](../resources/extensionproperty.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4db9c-152">If successful, this method returns a `201 Created` response code and a new [extensionProperty](../resources/extensionproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4db9c-153">Примеры</span><span class="sxs-lookup"><span data-stu-id="4db9c-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4db9c-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="4db9c-154">Request</span></span>

<span data-ttu-id="4db9c-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4db9c-155">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4db9c-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="4db9c-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_extensionproperty_from_application"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/extensionProperties
Content-type: application/json

{
    "name": "extensionName",
    "dataType": "string",
    "targetObjects": [
        "Application"
    ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4db9c-157">C#</span><span class="sxs-lookup"><span data-stu-id="4db9c-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-extensionproperty-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4db9c-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4db9c-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-extensionproperty-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4db9c-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4db9c-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-extensionproperty-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4db9c-160">Java</span><span class="sxs-lookup"><span data-stu-id="4db9c-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-extensionproperty-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4db9c-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="4db9c-161">Response</span></span>

<span data-ttu-id="4db9c-162">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [екстенсионпроперти](../resources/extensionProperty.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4db9c-162">If successful, this method returns `201 Created` response code and [extensionProperty](../resources/extensionProperty.md) object in the response body.</span></span>

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
