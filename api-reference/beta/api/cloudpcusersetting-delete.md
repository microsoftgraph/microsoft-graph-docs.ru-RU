---
title: Удаление cloudPcUserSetting
description: Удаление объекта cloudPcUserSetting.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: a3a6c5b7c7c75b89d1c27adcf7b123788f5cfe51
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993706"
---
# <a name="delete-cloudpcusersetting"></a><span data-ttu-id="dc3a8-103">Удаление cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="dc3a8-103">Delete cloudPcUserSetting</span></span>

<span data-ttu-id="dc3a8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc3a8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc3a8-105">Удаление [объекта cloudPcUserSetting.](../resources/cloudpcusersetting.md)</span><span class="sxs-lookup"><span data-stu-id="dc3a8-105">Delete a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="dc3a8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dc3a8-106">Permissions</span></span>

<span data-ttu-id="dc3a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc3a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc3a8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc3a8-109">Permission type</span></span>|<span data-ttu-id="dc3a8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc3a8-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc3a8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc3a8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dc3a8-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc3a8-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="dc3a8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc3a8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc3a8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc3a8-114">Not supported.</span></span>|
|<span data-ttu-id="dc3a8-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="dc3a8-115">Application</span></span>|<span data-ttu-id="dc3a8-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc3a8-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc3a8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc3a8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/userSettings/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dc3a8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc3a8-118">Request headers</span></span>
|<span data-ttu-id="dc3a8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="dc3a8-119">Name</span></span>|<span data-ttu-id="dc3a8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dc3a8-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dc3a8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc3a8-121">Authorization</span></span>|<span data-ttu-id="dc3a8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc3a8-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc3a8-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc3a8-124">Request body</span></span>
<span data-ttu-id="dc3a8-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dc3a8-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc3a8-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc3a8-126">Response</span></span>

<span data-ttu-id="dc3a8-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dc3a8-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="dc3a8-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="dc3a8-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dc3a8-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc3a8-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_cloudpcusersetting"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff
```


### <a name="response"></a><span data-ttu-id="dc3a8-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc3a8-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
