---
title: 'cloudPcDeviceImage: перезагрузка'
description: Перезагрузите объект cloudPcDeviceImage.
author: RuiHou105
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: ab636894279317ef18b4f41eb86081ac159ded59
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/10/2021
ms.locfileid: "53367050"
---
# <a name="cloudpcdeviceimage-reupload"></a><span data-ttu-id="2b582-103">cloudPcDeviceImage: перезагрузка</span><span class="sxs-lookup"><span data-stu-id="2b582-103">cloudPcDeviceImage: reupload</span></span>

<span data-ttu-id="2b582-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b582-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b582-105">Перезагрузите [объект cloudPcDeviceImage,](../resources/cloudpcdeviceimage.md) который не удалось загрузить.</span><span class="sxs-lookup"><span data-stu-id="2b582-105">Reupload a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object that failed to upload.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="2b582-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b582-106">Permissions</span></span>

<span data-ttu-id="2b582-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b582-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b582-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b582-109">Permission type</span></span>|<span data-ttu-id="2b582-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b582-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b582-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b582-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2b582-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b582-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="2b582-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b582-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b582-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b582-114">Not supported.</span></span>|
|<span data-ttu-id="2b582-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b582-115">Application</span></span>|<span data-ttu-id="2b582-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b582-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b582-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b582-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/deviceImages/{cloudPcDeviceImageId}/reupload
```

## <a name="request-headers"></a><span data-ttu-id="2b582-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b582-118">Request headers</span></span>

|<span data-ttu-id="2b582-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2b582-119">Name</span></span>|<span data-ttu-id="2b582-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2b582-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2b582-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b582-121">Authorization</span></span>|<span data-ttu-id="2b582-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b582-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b582-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b582-124">Request body</span></span>

<span data-ttu-id="2b582-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b582-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b582-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b582-126">Response</span></span>

<span data-ttu-id="2b582-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2b582-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2b582-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="2b582-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2b582-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b582-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "reupload_deviceimages_from_virtualendpoint"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages/{cloudPcDeviceImageId}/reupload
```

### <a name="response"></a><span data-ttu-id="2b582-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b582-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
