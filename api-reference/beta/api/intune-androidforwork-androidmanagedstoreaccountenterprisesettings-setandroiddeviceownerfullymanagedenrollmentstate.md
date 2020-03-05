---
title: Действие setAndroidDeviceOwnerFullyManagedEnrollmentState
description: Задает для ресурса androidmanagedstoreaccountenterprisesettings Андроиддевицеовнерфуллиманажеденроллментенаблед заданное значение.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: de2ae539ad05ed67c5a7c93d98f29ebec11fa349
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446102"
---
# <a name="setandroiddeviceownerfullymanagedenrollmentstate-action"></a><span data-ttu-id="0eb45-103">Действие setAndroidDeviceOwnerFullyManagedEnrollmentState</span><span class="sxs-lookup"><span data-stu-id="0eb45-103">setAndroidDeviceOwnerFullyManagedEnrollmentState action</span></span>

<span data-ttu-id="0eb45-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0eb45-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0eb45-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0eb45-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0eb45-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0eb45-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0eb45-107">Задает для ресурса androidmanagedstoreaccountenterprisesettings Андроиддевицеовнерфуллиманажеденроллментенаблед заданное значение.</span><span class="sxs-lookup"><span data-stu-id="0eb45-107">Sets the AndroidManagedStoreAccountEnterpriseSettings AndroidDeviceOwnerFullyManagedEnrollmentEnabled to the given value.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0eb45-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0eb45-108">Prerequisites</span></span>
<span data-ttu-id="0eb45-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0eb45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0eb45-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0eb45-111">Permission type</span></span>|<span data-ttu-id="0eb45-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0eb45-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0eb45-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0eb45-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0eb45-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0eb45-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0eb45-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0eb45-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0eb45-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0eb45-116">Not supported.</span></span>|
|<span data-ttu-id="0eb45-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0eb45-117">Application</span></span>|<span data-ttu-id="0eb45-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0eb45-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0eb45-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0eb45-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/setAndroidDeviceOwnerFullyManagedEnrollmentState
```

## <a name="request-headers"></a><span data-ttu-id="0eb45-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0eb45-120">Request headers</span></span>
|<span data-ttu-id="0eb45-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0eb45-121">Header</span></span>|<span data-ttu-id="0eb45-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0eb45-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0eb45-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0eb45-123">Authorization</span></span>|<span data-ttu-id="0eb45-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0eb45-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0eb45-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0eb45-125">Accept</span></span>|<span data-ttu-id="0eb45-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0eb45-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0eb45-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0eb45-127">Request body</span></span>
<span data-ttu-id="0eb45-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0eb45-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0eb45-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="0eb45-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0eb45-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0eb45-130">Property</span></span>|<span data-ttu-id="0eb45-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0eb45-131">Type</span></span>|<span data-ttu-id="0eb45-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0eb45-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0eb45-133">enabled</span><span class="sxs-lookup"><span data-stu-id="0eb45-133">enabled</span></span>|<span data-ttu-id="0eb45-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="0eb45-134">Boolean</span></span>|<span data-ttu-id="0eb45-135">Значение, с которым устанавливается Андроиддевицеовнерфуллиманажеденроллментенаблед.</span><span class="sxs-lookup"><span data-stu-id="0eb45-135">The value to set AndroidDeviceOwnerFullyManagedEnrollmentEnabled to.</span></span>|



## <a name="response"></a><span data-ttu-id="0eb45-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="0eb45-136">Response</span></span>
<span data-ttu-id="0eb45-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0eb45-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0eb45-138">Пример</span><span class="sxs-lookup"><span data-stu-id="0eb45-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="0eb45-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="0eb45-139">Request</span></span>
<span data-ttu-id="0eb45-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0eb45-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/setAndroidDeviceOwnerFullyManagedEnrollmentState

Content-type: application/json
Content-length: 23

{
  "enabled": true
}
```

### <a name="response"></a><span data-ttu-id="0eb45-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0eb45-141">Response</span></span>
<span data-ttu-id="0eb45-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0eb45-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





