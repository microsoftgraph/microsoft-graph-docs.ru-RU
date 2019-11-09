---
title: Функция Експортдевицеандаппманажементдата
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b6b51402ebd4a07b80e871104eb7ab177d140e98
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085586"
---
# <a name="exportdeviceandappmanagementdata-function"></a><span data-ttu-id="116c6-103">Функция Експортдевицеандаппманажементдата</span><span class="sxs-lookup"><span data-stu-id="116c6-103">exportDeviceAndAppManagementData function</span></span>

> <span data-ttu-id="116c6-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="116c6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="116c6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="116c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="116c6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="116c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="116c6-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="116c6-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="116c6-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="116c6-108">Prerequisites</span></span>

<span data-ttu-id="116c6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="116c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="116c6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="116c6-111">Permission type</span></span>|<span data-ttu-id="116c6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="116c6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="116c6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="116c6-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="116c6-114">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="116c6-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="116c6-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="116c6-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="116c6-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="116c6-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="116c6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="116c6-117">Not supported.</span></span>|
|<span data-ttu-id="116c6-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="116c6-118">Application</span></span>||
| <span data-ttu-id="116c6-119">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="116c6-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="116c6-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="116c6-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="116c6-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="116c6-121">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/exportDeviceAndAppManagementData
```

## <a name="request-headers"></a><span data-ttu-id="116c6-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="116c6-122">Request headers</span></span>

|<span data-ttu-id="116c6-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="116c6-123">Header</span></span>|<span data-ttu-id="116c6-124">Значение</span><span class="sxs-lookup"><span data-stu-id="116c6-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="116c6-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="116c6-125">Authorization</span></span>|<span data-ttu-id="116c6-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="116c6-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="116c6-127">Accept</span><span class="sxs-lookup"><span data-stu-id="116c6-127">Accept</span></span>|<span data-ttu-id="116c6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="116c6-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="116c6-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="116c6-129">Request body</span></span>

<span data-ttu-id="116c6-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="116c6-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="116c6-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="116c6-131">Property</span></span>|<span data-ttu-id="116c6-132">Тип</span><span class="sxs-lookup"><span data-stu-id="116c6-132">Type</span></span>|<span data-ttu-id="116c6-133">Описание</span><span class="sxs-lookup"><span data-stu-id="116c6-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="116c6-134">skip</span><span class="sxs-lookup"><span data-stu-id="116c6-134">skip</span></span>|<span data-ttu-id="116c6-135">Int32</span><span class="sxs-lookup"><span data-stu-id="116c6-135">Int32</span></span>|<span data-ttu-id="116c6-136">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="116c6-136">Not yet documented</span></span>|
|<span data-ttu-id="116c6-137">top</span><span class="sxs-lookup"><span data-stu-id="116c6-137">top</span></span>|<span data-ttu-id="116c6-138">Int32</span><span class="sxs-lookup"><span data-stu-id="116c6-138">Int32</span></span>|<span data-ttu-id="116c6-139">Н/Д</span><span class="sxs-lookup"><span data-stu-id="116c6-139">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="116c6-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="116c6-140">Response</span></span>

<span data-ttu-id="116c6-141">В случае успеха эта функция возвращает код `200 OK` отклика и объект [девицеандаппманажементдата](../resources/intune-onboarding-deviceandappmanagementdata.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="116c6-141">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="116c6-142">Пример</span><span class="sxs-lookup"><span data-stu-id="116c6-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="116c6-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="116c6-143">Request</span></span>

<span data-ttu-id="116c6-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="116c6-144">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/exportDeviceAndAppManagementData(skip=4,top=3)
```

### <a name="response"></a><span data-ttu-id="116c6-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="116c6-145">Response</span></span>

<span data-ttu-id="116c6-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="116c6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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












