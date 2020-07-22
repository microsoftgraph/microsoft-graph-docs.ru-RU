---
title: 'directoryObject: Жетаваилабликстенсионпропертиес'
description: Получение всех или отфильтрованных списков свойств расширения каталога, зарегистрированных в каталоге.
author: sureshja
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3276b114f3fa6370a4cc8d03b8b6607148bf3c7f
ms.sourcegitcommit: 0545b031585e605dc3a0fde481015f51f79819c4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2020
ms.locfileid: "45225009"
---
# <a name="directoryobject-getavailableextensionproperties"></a><span data-ttu-id="11e9e-103">directoryObject: Жетаваилабликстенсионпропертиес</span><span class="sxs-lookup"><span data-stu-id="11e9e-103">directoryObject: getAvailableExtensionProperties</span></span>
<span data-ttu-id="11e9e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11e9e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="11e9e-105">Возвращает все или отфильтрованный список свойств расширения каталога, зарегистрированных в каталоге.</span><span class="sxs-lookup"><span data-stu-id="11e9e-105">Return all or a filtered list of the directory extension properties that have been registered in a directory.</span></span> <span data-ttu-id="11e9e-106">Следующие объекты поддерживают свойства расширения: **User**, **Group**, **Organization**, **Device**, **Application**и **servicePrincipal**.</span><span class="sxs-lookup"><span data-stu-id="11e9e-106">The following entities support extension properties: **user**, **group**, **organization**, **device**, **application**, and **servicePrincipal**.</span></span>

## <a name="permissions"></a><span data-ttu-id="11e9e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="11e9e-107">Permissions</span></span>
<span data-ttu-id="11e9e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11e9e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11e9e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11e9e-110">Permission type</span></span>|<span data-ttu-id="11e9e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="11e9e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11e9e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11e9e-112">Delegated (work or school account)</span></span>| <span data-ttu-id="11e9e-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="11e9e-113">Directory.Read.All</span></span> |
|<span data-ttu-id="11e9e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11e9e-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="11e9e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11e9e-115">Not supported.</span></span> |
|<span data-ttu-id="11e9e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11e9e-116">Application</span></span>| <span data-ttu-id="11e9e-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="11e9e-117">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="11e9e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11e9e-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /directoryObjects/getAvailableExtensionProperties
```

## <a name="request-headers"></a><span data-ttu-id="11e9e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11e9e-119">Request headers</span></span>
|<span data-ttu-id="11e9e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="11e9e-120">Name</span></span>|<span data-ttu-id="11e9e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="11e9e-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="11e9e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="11e9e-122">Authorization</span></span>|<span data-ttu-id="11e9e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11e9e-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="11e9e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="11e9e-125">Content-Type</span></span>|<span data-ttu-id="11e9e-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11e9e-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="11e9e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="11e9e-128">Request body</span></span>
<span data-ttu-id="11e9e-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11e9e-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="11e9e-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="11e9e-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="11e9e-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="11e9e-131">Parameter</span></span>|<span data-ttu-id="11e9e-132">Тип</span><span class="sxs-lookup"><span data-stu-id="11e9e-132">Type</span></span>|<span data-ttu-id="11e9e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="11e9e-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11e9e-134">иссинцедфромонпремисес</span><span class="sxs-lookup"><span data-stu-id="11e9e-134">isSyncedFromOnPremises</span></span>|<span data-ttu-id="11e9e-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="11e9e-135">Boolean</span></span>|<span data-ttu-id="11e9e-136">`true`чтобы указать, что необходимо вернуть только свойства расширения, синхронизированные из локального каталога; `false`чтобы указать, что необходимо вернуть только свойства расширения, которые не синхронизируются из локального каталога.</span><span class="sxs-lookup"><span data-stu-id="11e9e-136">`true` to specify that only extension properties that are synced from the on-premises directory should be returned; `false` to specify that only extension properties that are not synced from the on-premises directory should be returned.</span></span> <span data-ttu-id="11e9e-137">Если параметр не задан, возвращаются все свойства расширения (синхронизированные и несинхронизированные).</span><span class="sxs-lookup"><span data-stu-id="11e9e-137">If the parameter is omitted, all extension properties (both synced and non-synced) are returned.</span></span>|


## <a name="response"></a><span data-ttu-id="11e9e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="11e9e-138">Response</span></span>

<span data-ttu-id="11e9e-139">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [екстенсионпроперти](../resources/extensionproperty.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="11e9e-139">If successful, this action returns a `200 OK` response code and an [extensionProperty](../resources/extensionproperty.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="11e9e-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="11e9e-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="11e9e-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="11e9e-141">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="11e9e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="11e9e-142">Response</span></span>
> <span data-ttu-id="11e9e-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="11e9e-143">**Note:** The response object shown here might be shortened for readability.</span></span>

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

