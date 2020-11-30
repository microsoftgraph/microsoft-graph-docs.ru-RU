---
title: Удаление Клаудпкдевицеимаже
description: Удаление объекта Клаудпкдевицеимаже.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: e6b5ad15ec2bf768a9b02cb49289c8028699f3ea
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378464"
---
# <a name="delete-cloudpcdeviceimage"></a><span data-ttu-id="a95be-103">Удаление Клаудпкдевицеимаже</span><span class="sxs-lookup"><span data-stu-id="a95be-103">Delete cloudPcDeviceImage</span></span>

<span data-ttu-id="a95be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a95be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a95be-105">Удаление объекта [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md) .</span><span class="sxs-lookup"><span data-stu-id="a95be-105">Delete a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a95be-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a95be-106">Permissions</span></span>

<span data-ttu-id="a95be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a95be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a95be-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a95be-109">Permission type</span></span>|<span data-ttu-id="a95be-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a95be-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a95be-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a95be-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a95be-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a95be-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="a95be-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a95be-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a95be-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a95be-114">Not supported.</span></span>|
|<span data-ttu-id="a95be-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a95be-115">Application</span></span>|<span data-ttu-id="a95be-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a95be-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a95be-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a95be-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/deviceImages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a95be-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a95be-118">Request headers</span></span>

|<span data-ttu-id="a95be-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a95be-119">Name</span></span>|<span data-ttu-id="a95be-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a95be-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a95be-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a95be-121">Authorization</span></span>|<span data-ttu-id="a95be-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a95be-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a95be-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a95be-124">Request body</span></span>

<span data-ttu-id="a95be-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a95be-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a95be-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="a95be-126">Response</span></span>

<span data-ttu-id="a95be-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a95be-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a95be-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="a95be-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a95be-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="a95be-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_deviceimages_from_virtualendpoint"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages/{id}
```

### <a name="response"></a><span data-ttu-id="a95be-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a95be-130">Response</span></span>

<span data-ttu-id="a95be-131">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a95be-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
