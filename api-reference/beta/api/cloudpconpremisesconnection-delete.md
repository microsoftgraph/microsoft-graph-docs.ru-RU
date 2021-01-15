---
title: Удаление cloudPcOnPremisesConnection
description: Удаление объекта cloudPcOnPremisesConnection.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 01f9b5a7e4091492be7aa8eae0f0d3f8354169e6
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872767"
---
# <a name="delete-cloudpconpremisesconnection"></a><span data-ttu-id="59d52-103">Удаление cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="59d52-103">Delete cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="59d52-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59d52-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59d52-105">Удаление определенного [объекта cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="59d52-105">Delete a specific [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="59d52-106">При удалении подключения разрешения для службы удаляются из указанных ресурсов Azure.</span><span class="sxs-lookup"><span data-stu-id="59d52-106">When you delete a connection, permissions to the service are removed from the specified Azure resources.</span></span>

<span data-ttu-id="59d52-107">Локальное подключение невозможно удалить после того, как оно пройдет проверку на состояние, что указывает `healthCheckStatus` свойство.</span><span class="sxs-lookup"><span data-stu-id="59d52-107">You cannot delete an on-premises connection once it passes health check, which is indicated by the `healthCheckStatus` property.</span></span>

<span data-ttu-id="59d52-108">Невозможно удалить подключение, если оно используется, как указано в `inUse` свойстве.</span><span class="sxs-lookup"><span data-stu-id="59d52-108">You cannot delete a connection when it's in use either, as indicated by the `inUse` property.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="59d52-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59d52-109">Permissions</span></span>

<span data-ttu-id="59d52-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59d52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59d52-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59d52-112">Permission type</span></span>|<span data-ttu-id="59d52-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59d52-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59d52-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59d52-114">Delegated (work or school account)</span></span>|<span data-ttu-id="59d52-115">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59d52-115">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="59d52-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59d52-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59d52-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59d52-117">Not supported.</span></span>|
|<span data-ttu-id="59d52-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="59d52-118">Application</span></span>|<span data-ttu-id="59d52-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59d52-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59d52-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59d52-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="59d52-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59d52-121">Request headers</span></span>

|<span data-ttu-id="59d52-122">Имя</span><span class="sxs-lookup"><span data-stu-id="59d52-122">Name</span></span>|<span data-ttu-id="59d52-123">Описание</span><span class="sxs-lookup"><span data-stu-id="59d52-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="59d52-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59d52-124">Authorization</span></span>|<span data-ttu-id="59d52-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59d52-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59d52-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59d52-127">Request body</span></span>

<span data-ttu-id="59d52-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="59d52-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59d52-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="59d52-129">Response</span></span>

<span data-ttu-id="59d52-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="59d52-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="59d52-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="59d52-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="59d52-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="59d52-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="59d52-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="59d52-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_onpremisesconnections_from_virtualendpoint"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```
# <a name="c"></a>[<span data-ttu-id="59d52-134">C#</span><span class="sxs-lookup"><span data-stu-id="59d52-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-onpremisesconnections-from-virtualendpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59d52-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59d52-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-onpremisesconnections-from-virtualendpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59d52-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59d52-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-onpremisesconnections-from-virtualendpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="59d52-137">Java</span><span class="sxs-lookup"><span data-stu-id="59d52-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-onpremisesconnections-from-virtualendpoint-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="59d52-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="59d52-138">Response</span></span>

<span data-ttu-id="59d52-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="59d52-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
