---
title: Функция Експортдевицеандаппманажементдата
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e482edf33be72a2b01304b0c189ef6189428916a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447545"
---
# <a name="exportdeviceandappmanagementdata-function"></a><span data-ttu-id="4b97b-103">Функция Експортдевицеандаппманажементдата</span><span class="sxs-lookup"><span data-stu-id="4b97b-103">exportDeviceAndAppManagementData function</span></span>

<span data-ttu-id="4b97b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b97b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b97b-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4b97b-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4b97b-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b97b-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b97b-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b97b-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b97b-108">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4b97b-108">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b97b-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4b97b-109">Prerequisites</span></span>

<span data-ttu-id="4b97b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b97b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b97b-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b97b-112">Permission type</span></span>|<span data-ttu-id="4b97b-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b97b-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b97b-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b97b-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4b97b-115">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="4b97b-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="4b97b-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b97b-116">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4b97b-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b97b-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b97b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b97b-118">Not supported.</span></span>|
|<span data-ttu-id="4b97b-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b97b-119">Application</span></span>||
| <span data-ttu-id="4b97b-120">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="4b97b-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="4b97b-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b97b-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b97b-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b97b-122">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/exportDeviceAndAppManagementData
```

## <a name="request-headers"></a><span data-ttu-id="4b97b-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4b97b-123">Request headers</span></span>

|<span data-ttu-id="4b97b-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b97b-124">Header</span></span>|<span data-ttu-id="4b97b-125">Значение</span><span class="sxs-lookup"><span data-stu-id="4b97b-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b97b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b97b-126">Authorization</span></span>|<span data-ttu-id="4b97b-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b97b-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b97b-128">Accept</span><span class="sxs-lookup"><span data-stu-id="4b97b-128">Accept</span></span>|<span data-ttu-id="4b97b-129">application/json</span><span class="sxs-lookup"><span data-stu-id="4b97b-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b97b-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4b97b-130">Request body</span></span>

<span data-ttu-id="4b97b-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="4b97b-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="4b97b-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b97b-132">Property</span></span>|<span data-ttu-id="4b97b-133">Тип</span><span class="sxs-lookup"><span data-stu-id="4b97b-133">Type</span></span>|<span data-ttu-id="4b97b-134">Описание</span><span class="sxs-lookup"><span data-stu-id="4b97b-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b97b-135">skip</span><span class="sxs-lookup"><span data-stu-id="4b97b-135">skip</span></span>|<span data-ttu-id="4b97b-136">Int32</span><span class="sxs-lookup"><span data-stu-id="4b97b-136">Int32</span></span>|<span data-ttu-id="4b97b-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4b97b-137">Not yet documented</span></span>|
|<span data-ttu-id="4b97b-138">top</span><span class="sxs-lookup"><span data-stu-id="4b97b-138">top</span></span>|<span data-ttu-id="4b97b-139">Int32</span><span class="sxs-lookup"><span data-stu-id="4b97b-139">Int32</span></span>|<span data-ttu-id="4b97b-140">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4b97b-140">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="4b97b-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b97b-141">Response</span></span>

<span data-ttu-id="4b97b-142">В случае успеха эта функция возвращает код `200 OK` отклика и объект [девицеандаппманажементдата](../resources/intune-onboarding-deviceandappmanagementdata.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b97b-142">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b97b-143">Пример</span><span class="sxs-lookup"><span data-stu-id="4b97b-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b97b-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b97b-144">Request</span></span>

<span data-ttu-id="4b97b-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b97b-145">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/exportDeviceAndAppManagementData(skip=4,top=3)
```

### <a name="response"></a><span data-ttu-id="4b97b-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b97b-146">Response</span></span>

<span data-ttu-id="4b97b-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b97b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 143

{
  "value": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementData",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```









