---
title: Создание externalConnection
description: Создайте новый объект externalConnection.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: d556b4925625ac929c1b13f6559c048de1b55366
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467441"
---
# <a name="create-externalconnection"></a><span data-ttu-id="88c37-103">Создание externalConnection</span><span class="sxs-lookup"><span data-stu-id="88c37-103">Create externalConnection</span></span>
<span data-ttu-id="88c37-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="88c37-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="88c37-105">Создайте новый объект externalConnection.</span><span class="sxs-lookup"><span data-stu-id="88c37-105">Create a new externalConnection object.</span></span>

## <a name="permissions"></a><span data-ttu-id="88c37-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="88c37-106">Permissions</span></span>
<span data-ttu-id="88c37-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88c37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88c37-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88c37-109">Permission type</span></span>|<span data-ttu-id="88c37-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="88c37-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88c37-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88c37-111">Delegated (work or school account)</span></span>|<span data-ttu-id="88c37-112">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="88c37-112">Not applicable</span></span>|
|<span data-ttu-id="88c37-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88c37-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88c37-114">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="88c37-114">Not applicable</span></span>|
|<span data-ttu-id="88c37-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="88c37-115">Application</span></span>| <span data-ttu-id="88c37-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="88c37-116">ExternalConnection.ReadWrite.OwnedBy</span></span>|

## <a name="http-request"></a><span data-ttu-id="88c37-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88c37-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /external/connections
```

## <a name="request-headers"></a><span data-ttu-id="88c37-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88c37-118">Request headers</span></span>
|<span data-ttu-id="88c37-119">Имя</span><span class="sxs-lookup"><span data-stu-id="88c37-119">Name</span></span>|<span data-ttu-id="88c37-120">Описание</span><span class="sxs-lookup"><span data-stu-id="88c37-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="88c37-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88c37-121">Authorization</span></span>|<span data-ttu-id="88c37-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88c37-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="88c37-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="88c37-124">Content-Type</span></span>|<span data-ttu-id="88c37-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88c37-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="88c37-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="88c37-127">Request body</span></span>
<span data-ttu-id="88c37-128">В теле запроса поставляем представление JSON объекта [externalConnection.](../resources/externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="88c37-128">In the request body, supply a JSON representation of the [externalConnection](../resources/externalconnectors-externalconnection.md) object.</span></span>

<span data-ttu-id="88c37-129">В следующей таблице показаны свойства, необходимые при создании [externalConnection.](../resources/externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="88c37-129">The following table shows the properties that are required when you create the [externalConnection](../resources/externalconnectors-externalconnection.md).</span></span>

|<span data-ttu-id="88c37-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="88c37-130">Property</span></span>|<span data-ttu-id="88c37-131">Тип</span><span class="sxs-lookup"><span data-stu-id="88c37-131">Type</span></span>|<span data-ttu-id="88c37-132">Обязательно (Y/N)</span><span class="sxs-lookup"><span data-stu-id="88c37-132">Required (Y/N)</span></span> |<span data-ttu-id="88c37-133">Описание</span><span class="sxs-lookup"><span data-stu-id="88c37-133">Description</span></span>|
|:---|:---|:---|:---|
|<span data-ttu-id="88c37-134">id</span><span class="sxs-lookup"><span data-stu-id="88c37-134">id</span></span>|<span data-ttu-id="88c37-135">String</span><span class="sxs-lookup"><span data-stu-id="88c37-135">String</span></span>|<span data-ttu-id="88c37-136">Да</span><span class="sxs-lookup"><span data-stu-id="88c37-136">Y</span></span>|<span data-ttu-id="88c37-137">ID подключения</span><span class="sxs-lookup"><span data-stu-id="88c37-137">The connection ID</span></span>|
|<span data-ttu-id="88c37-138">name</span><span class="sxs-lookup"><span data-stu-id="88c37-138">name</span></span>|<span data-ttu-id="88c37-139">String</span><span class="sxs-lookup"><span data-stu-id="88c37-139">String</span></span>|<span data-ttu-id="88c37-140">Да</span><span class="sxs-lookup"><span data-stu-id="88c37-140">Y</span></span>|<span data-ttu-id="88c37-141">Имя подключения</span><span class="sxs-lookup"><span data-stu-id="88c37-141">The connection name</span></span>|
|<span data-ttu-id="88c37-142">description</span><span class="sxs-lookup"><span data-stu-id="88c37-142">description</span></span>|<span data-ttu-id="88c37-143">String</span><span class="sxs-lookup"><span data-stu-id="88c37-143">String</span></span>|<span data-ttu-id="88c37-144">Да</span><span class="sxs-lookup"><span data-stu-id="88c37-144">Y</span></span>|<span data-ttu-id="88c37-145">Описание подключения</span><span class="sxs-lookup"><span data-stu-id="88c37-145">The connection description</span></span>|
|<span data-ttu-id="88c37-146">configuration</span><span class="sxs-lookup"><span data-stu-id="88c37-146">configuration</span></span>|[<span data-ttu-id="88c37-147">microsoft.graph.externalConnectors.configuration</span><span class="sxs-lookup"><span data-stu-id="88c37-147">microsoft.graph.externalConnectors.configuration</span></span>](../resources/externalconnectors-configuration.md)|<span data-ttu-id="88c37-148">Нет</span><span class="sxs-lookup"><span data-stu-id="88c37-148">N</span></span>|<span data-ttu-id="88c37-149">Конфигурации подключения</span><span class="sxs-lookup"><span data-stu-id="88c37-149">The connection configurations</span></span>|



## <a name="response"></a><span data-ttu-id="88c37-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="88c37-150">Response</span></span>

<span data-ttu-id="88c37-151">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект externalConnection](../resources/externalconnectors-externalconnection.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="88c37-151">If successful, this method returns a `201 Created` response code and an [externalConnection](../resources/externalconnectors-externalconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="88c37-152">Примеры</span><span class="sxs-lookup"><span data-stu-id="88c37-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="88c37-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="88c37-153">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_externalconnection_from_connections"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/external/connections
Content-Type: application/json

{
  "id": "contosohr",
  "name": "Contoso HR",
  "description": "Connection to index Contoso HR system"
}
```


### <a name="response"></a><span data-ttu-id="88c37-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="88c37-154">Response</span></span>
<span data-ttu-id="88c37-155">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="88c37-155">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalConnection"
}
-->
``` http
HTTP/1.1 200 Created
Content-Type: application/json

{
  "id": "0a4f4e74-4e74-0a4f-744e-4f0a744e4f0a",
  "name": "String",
  "description": "String",
  "state": "ready",
  "configuration": {
    "authorizedAppIds": [
      "d310d35d-72ec-47dd-92f2-fb9c40936555"
    ]
  }
}
```

