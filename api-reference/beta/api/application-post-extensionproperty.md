---
title: Создание Екстенсионпроперти
description: Создание нового Екстенсионпроперти.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bd4a28300d18db4ef9bf7dded1b739d0870ffa49
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996817"
---
# <a name="create-extensionproperty"></a><span data-ttu-id="d9f57-103">Создание Екстенсионпроперти</span><span class="sxs-lookup"><span data-stu-id="d9f57-103">Create extensionProperty</span></span>

<span data-ttu-id="d9f57-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9f57-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9f57-105">Создайте новое определение [екстенсионпроперти](../resources/extensionproperty.md) .</span><span class="sxs-lookup"><span data-stu-id="d9f57-105">Create a new [extensionProperty](../resources/extensionproperty.md) definition.</span></span> <span data-ttu-id="d9f57-106">Эту операцию можно использовать для добавления настраиваемого значения свойства в целевой тип объекта, определенный в Екстенсионпроперти, с помощью стандартных запросов на создание и обновление целевого объекта.</span><span class="sxs-lookup"><span data-stu-id="d9f57-106">You can use this operation to add a custom property value to the targeted object type defined in the extensionProperty, using standard creation and update requests to the target object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9f57-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9f57-107">Permissions</span></span>

<span data-ttu-id="d9f57-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9f57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9f57-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9f57-110">Permission type</span></span>      | <span data-ttu-id="d9f57-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9f57-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9f57-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9f57-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d9f57-113">Application. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="d9f57-113">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d9f57-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9f57-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9f57-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9f57-115">Not supported.</span></span>    |
|<span data-ttu-id="d9f57-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9f57-116">Application</span></span> | <span data-ttu-id="d9f57-117">Application. ReadWrite. Овнедби, Application. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d9f57-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9f57-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9f57-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/extensionProperties
```

## <a name="request-headers"></a><span data-ttu-id="d9f57-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9f57-119">Request headers</span></span>
| <span data-ttu-id="d9f57-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d9f57-120">Name</span></span>       | <span data-ttu-id="d9f57-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d9f57-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="d9f57-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d9f57-122">Authorization</span></span>  | <span data-ttu-id="d9f57-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9f57-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d9f57-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d9f57-125">Content-Type</span></span> | <span data-ttu-id="d9f57-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9f57-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9f57-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d9f57-128">Request body</span></span>

<span data-ttu-id="d9f57-129">В тексте запроса укажите объект [екстенсионпроперти](../resources/extensionproperty.md) со следующими свойствами.</span><span class="sxs-lookup"><span data-stu-id="d9f57-129">In the request body, provide an [extensionProperty](../resources/extensionproperty.md) object with the following properties.</span></span>


| <span data-ttu-id="d9f57-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9f57-130">Property</span></span>     | <span data-ttu-id="d9f57-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d9f57-131">Type</span></span>        | <span data-ttu-id="d9f57-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d9f57-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d9f57-133">dataType</span><span class="sxs-lookup"><span data-stu-id="d9f57-133">dataType</span></span>|<span data-ttu-id="d9f57-134">String</span><span class="sxs-lookup"><span data-stu-id="d9f57-134">String</span></span>| <span data-ttu-id="d9f57-135">Задает тип данных значения, которое может содержать свойство Extension.</span><span class="sxs-lookup"><span data-stu-id="d9f57-135">Specifies the data type of the value the extension property can hold.</span></span> <span data-ttu-id="d9f57-136">Поддерживаются следующие значения:</span><span class="sxs-lookup"><span data-stu-id="d9f57-136">Following values are supported.</span></span> <span data-ttu-id="d9f57-137">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="d9f57-137">Not nullable.</span></span> <ul><li><span data-ttu-id="d9f57-138">`Binary` – 256 байт (максимум)</span><span class="sxs-lookup"><span data-stu-id="d9f57-138">`Binary` - 256 bytes maximum</span></span></li><li>`Boolean`</li><li><span data-ttu-id="d9f57-139">`DateTime` -Должен быть указан в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="d9f57-139">`DateTime` - Must be specified in ISO 8601 format.</span></span> <span data-ttu-id="d9f57-140">Данные времени будут храниться в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="d9f57-140">Will be stored in UTC.</span></span></li><li><span data-ttu-id="d9f57-141">`Integer` — значение 32 — бит.</span><span class="sxs-lookup"><span data-stu-id="d9f57-141">`Integer` - 32-bit value.</span></span></li><li><span data-ttu-id="d9f57-142">`LargeInteger` — значение 64 — бит.</span><span class="sxs-lookup"><span data-stu-id="d9f57-142">`LargeInteger` - 64-bit value.</span></span></li><li><span data-ttu-id="d9f57-143">`String` – 256 символов максимум</span><span class="sxs-lookup"><span data-stu-id="d9f57-143">`String` - 256 characters maximum</span></span></li></ul>|
|<span data-ttu-id="d9f57-144">name</span><span class="sxs-lookup"><span data-stu-id="d9f57-144">name</span></span>|<span data-ttu-id="d9f57-145">String</span><span class="sxs-lookup"><span data-stu-id="d9f57-145">String</span></span>| <span data-ttu-id="d9f57-146">Имя свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="d9f57-146">Name of the extension property.</span></span> <span data-ttu-id="d9f57-147">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="d9f57-147">Not nullable.</span></span> |
|<span data-ttu-id="d9f57-148">таржетобжектс</span><span class="sxs-lookup"><span data-stu-id="d9f57-148">targetObjects</span></span>|<span data-ttu-id="d9f57-149">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d9f57-149">String collection</span></span>| <span data-ttu-id="d9f57-150">Поддерживаются следующие значения:</span><span class="sxs-lookup"><span data-stu-id="d9f57-150">Following values are supported.</span></span> <span data-ttu-id="d9f57-151">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="d9f57-151">Not nullable.</span></span> <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|


## <a name="response"></a><span data-ttu-id="d9f57-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9f57-152">Response</span></span>

<span data-ttu-id="d9f57-153">В случае успешного выполнения этот метод возвращает `201, Created` код отклика и новый объект [екстенсионпроперти](../resources/extensionproperty.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d9f57-153">If successful, this method returns `201, Created` response code and a new [extensionProperty](../resources/extensionproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d9f57-154">Примеры</span><span class="sxs-lookup"><span data-stu-id="d9f57-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d9f57-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9f57-155">Request</span></span>

<span data-ttu-id="d9f57-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9f57-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d9f57-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9f57-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d9f57-158">C#</span><span class="sxs-lookup"><span data-stu-id="d9f57-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-extensionproperty-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9f57-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9f57-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-extensionproperty-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9f57-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9f57-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-extensionproperty-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d9f57-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9f57-161">Response</span></span>

<span data-ttu-id="d9f57-162">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [екстенсионпроперти](../resources/extensionProperty.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d9f57-162">If successful, this method returns a `201 Created` response code and an [extensionProperty](../resources/extensionProperty.md) object in the response body.</span></span>

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


