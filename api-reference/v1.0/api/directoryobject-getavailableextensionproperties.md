---
title: 'directoryObject: getAvailableExtensionProperties'
description: Получение полного или отфильтрованного списка свойств расширения каталога, которые зарегистрированы в каталоге.
author: sureshja
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 0464228669013360ad71eb24d214c4810bdb4c43
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434414"
---
# <a name="directoryobject-getavailableextensionproperties"></a><span data-ttu-id="aa429-103">directoryObject: getAvailableExtensionProperties</span><span class="sxs-lookup"><span data-stu-id="aa429-103">directoryObject: getAvailableExtensionProperties</span></span>
<span data-ttu-id="aa429-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa429-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aa429-105">Верни все или отфильтрованный список свойств расширения каталога, зарегистрированных в каталоге.</span><span class="sxs-lookup"><span data-stu-id="aa429-105">Return all or a filtered list of the directory extension properties that have been registered in a directory.</span></span> <span data-ttu-id="aa429-106">Следующие сущности поддерживают свойства расширения: **пользовательские,** **групповые,** **организации,** **устройства,** **приложения** и **servicePrincipal.**</span><span class="sxs-lookup"><span data-stu-id="aa429-106">The following entities support extension properties: **user**, **group**, **organization**, **device**, **application**, and **servicePrincipal**.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa429-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aa429-107">Permissions</span></span>
<span data-ttu-id="aa429-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa429-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa429-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa429-110">Permission type</span></span>|<span data-ttu-id="aa429-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa429-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa429-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa429-112">Delegated (work or school account)</span></span>| <span data-ttu-id="aa429-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa429-113">Directory.Read.All</span></span> |
|<span data-ttu-id="aa429-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa429-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="aa429-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa429-115">Not supported.</span></span> |
|<span data-ttu-id="aa429-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa429-116">Application</span></span>| <span data-ttu-id="aa429-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa429-117">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa429-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa429-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /directoryObjects/getAvailableExtensionProperties
```

## <a name="request-headers"></a><span data-ttu-id="aa429-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa429-119">Request headers</span></span>
|<span data-ttu-id="aa429-120">Имя</span><span class="sxs-lookup"><span data-stu-id="aa429-120">Name</span></span>|<span data-ttu-id="aa429-121">Описание</span><span class="sxs-lookup"><span data-stu-id="aa429-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="aa429-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aa429-122">Authorization</span></span>|<span data-ttu-id="aa429-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa429-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="aa429-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aa429-125">Content-Type</span></span>|<span data-ttu-id="aa429-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa429-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa429-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aa429-128">Request body</span></span>
<span data-ttu-id="aa429-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa429-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="aa429-130">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="aa429-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="aa429-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="aa429-131">Parameter</span></span>|<span data-ttu-id="aa429-132">Тип</span><span class="sxs-lookup"><span data-stu-id="aa429-132">Type</span></span>|<span data-ttu-id="aa429-133">Описание</span><span class="sxs-lookup"><span data-stu-id="aa429-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa429-134">isSyncedFromOnPremises</span><span class="sxs-lookup"><span data-stu-id="aa429-134">isSyncedFromOnPremises</span></span>|<span data-ttu-id="aa429-135">Логический</span><span class="sxs-lookup"><span data-stu-id="aa429-135">Boolean</span></span>|<span data-ttu-id="aa429-136">`true` указать, что должны возвращаться только свойства расширения, синхронизированные из локального каталога; чтобы указать, что возвращаются только свойства расширения, не синхронизированные из локального `false` каталога.</span><span class="sxs-lookup"><span data-stu-id="aa429-136">`true` to specify that only extension properties that are synced from the on-premises directory should be returned; `false` to specify that only extension properties that are not synced from the on-premises directory should be returned.</span></span> <span data-ttu-id="aa429-137">Если параметр опущен, возвращаются все свойства расширения (как синхронизированные, так и не синхронизированные).</span><span class="sxs-lookup"><span data-stu-id="aa429-137">If the parameter is omitted, all extension properties (both synced and non-synced) are returned.</span></span>|


## <a name="response"></a><span data-ttu-id="aa429-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa429-138">Response</span></span>

<span data-ttu-id="aa429-139">В случае успеха это действие возвращает код ответа и `200 OK` [коллекцию extensionProperty](../resources/extensionproperty.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="aa429-139">If successful, this action returns a `200 OK` response code and an [extensionProperty](../resources/extensionproperty.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aa429-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="aa429-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aa429-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa429-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="aa429-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa429-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getavailableextensionproperties"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/directoryObjects/getAvailableExtensionProperties
Content-Type: application/json
Content-length: 43

{
  "isSyncedFromOnPremises": "Boolean"
}
```
# <a name="javascript"></a>[<span data-ttu-id="aa429-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa429-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getavailableextensionproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="aa429-144">C#</span><span class="sxs-lookup"><span data-stu-id="aa429-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getavailableextensionproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aa429-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aa429-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getavailableextensionproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aa429-146">Java</span><span class="sxs-lookup"><span data-stu-id="aa429-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getavailableextensionproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="aa429-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa429-147">Response</span></span>
> <span data-ttu-id="aa429-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="aa429-148">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.extensionProperty)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.extensionProperty",
      "id": "d6a8bfec-893d-46e4-88fd-7db5fcc0fa62",
      "deletedDateTime": null,
      "appDisplayName": "SampleApp",
      "name": "extension_4d405aa8baa04fb494d3e0571fd9fd71_skypeId",
      "dataType": "String",
      "isSyncedFromOnPremises": false,
      "targetObjects": [
        "User"
      ]
    }
  ]
}
```


