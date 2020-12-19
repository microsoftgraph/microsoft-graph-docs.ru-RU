---
title: 'directoryObject: getAvailableExtensionProperties'
description: Получение полного или отфильтрованного списка свойств расширения каталога, которые зарегистрированы в каталоге.
author: sureshja
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7c37114cc7db3224eca3722e00d6334523df6226
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720030"
---
# <a name="directoryobject-getavailableextensionproperties"></a><span data-ttu-id="d5994-103">directoryObject: getAvailableExtensionProperties</span><span class="sxs-lookup"><span data-stu-id="d5994-103">directoryObject: getAvailableExtensionProperties</span></span>
<span data-ttu-id="d5994-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5994-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d5994-105">Возвращает все или отфильтрованный список свойств расширения каталога, зарегистрированных в каталоге.</span><span class="sxs-lookup"><span data-stu-id="d5994-105">Return all or a filtered list of the directory extension properties that have been registered in a directory.</span></span> <span data-ttu-id="d5994-106">Следующие сущности поддерживают свойства расширения: **user,** **group,** **organization,** **device,** **application** и **servicePrincipal.**</span><span class="sxs-lookup"><span data-stu-id="d5994-106">The following entities support extension properties: **user**, **group**, **organization**, **device**, **application**, and **servicePrincipal**.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5994-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d5994-107">Permissions</span></span>
<span data-ttu-id="d5994-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5994-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5994-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5994-110">Permission type</span></span>|<span data-ttu-id="d5994-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5994-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5994-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5994-112">Delegated (work or school account)</span></span>| <span data-ttu-id="d5994-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5994-113">Directory.Read.All</span></span> |
|<span data-ttu-id="d5994-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5994-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d5994-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5994-115">Not supported.</span></span> |
|<span data-ttu-id="d5994-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5994-116">Application</span></span>| <span data-ttu-id="d5994-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5994-117">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5994-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5994-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /directoryObjects/getAvailableExtensionProperties
```

## <a name="request-headers"></a><span data-ttu-id="d5994-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d5994-119">Request headers</span></span>
|<span data-ttu-id="d5994-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d5994-120">Name</span></span>|<span data-ttu-id="d5994-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d5994-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d5994-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5994-122">Authorization</span></span>|<span data-ttu-id="d5994-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5994-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d5994-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d5994-125">Content-Type</span></span>|<span data-ttu-id="d5994-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5994-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5994-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d5994-128">Request body</span></span>
<span data-ttu-id="d5994-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d5994-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d5994-130">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="d5994-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d5994-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="d5994-131">Parameter</span></span>|<span data-ttu-id="d5994-132">Тип</span><span class="sxs-lookup"><span data-stu-id="d5994-132">Type</span></span>|<span data-ttu-id="d5994-133">Описание</span><span class="sxs-lookup"><span data-stu-id="d5994-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5994-134">isSyncedFromOnPremises</span><span class="sxs-lookup"><span data-stu-id="d5994-134">isSyncedFromOnPremises</span></span>|<span data-ttu-id="d5994-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5994-135">Boolean</span></span>|<span data-ttu-id="d5994-136">`true` чтобы указать, что должны возвращаться только свойства расширения, синхронизированные из локального каталога; чтобы указать, что должны быть возвращены только свойства расширения, которые не синхронизируются из `false` локального каталога.</span><span class="sxs-lookup"><span data-stu-id="d5994-136">`true` to specify that only extension properties that are synced from the on-premises directory should be returned; `false` to specify that only extension properties that are not synced from the on-premises directory should be returned.</span></span> <span data-ttu-id="d5994-137">Если этот параметр опущен, возвращаются все свойства расширения (как синхронизированные, так и не синхронизированные).</span><span class="sxs-lookup"><span data-stu-id="d5994-137">If the parameter is omitted, all extension properties (both synced and non-synced) are returned.</span></span>|


## <a name="response"></a><span data-ttu-id="d5994-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5994-138">Response</span></span>

<span data-ttu-id="d5994-139">В случае успеха это действие возвращает код отклика и коллекцию `200 OK` [extensionProperty](../resources/extensionproperty.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d5994-139">If successful, this action returns a `200 OK` response code and an [extensionProperty](../resources/extensionproperty.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d5994-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="d5994-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d5994-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5994-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d5994-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5994-142">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="d5994-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5994-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getavailableextensionproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d5994-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5994-144">Response</span></span>
> <span data-ttu-id="d5994-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d5994-145">**Note:** The response object shown here might be shortened for readability.</span></span>

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


