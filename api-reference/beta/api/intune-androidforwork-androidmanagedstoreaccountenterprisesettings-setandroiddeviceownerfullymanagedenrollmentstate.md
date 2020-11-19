---
title: Действие setAndroidDeviceOwnerFullyManagedEnrollmentState
description: Задает для ресурса androidmanagedstoreaccountenterprisesettings Андроиддевицеовнерфуллиманажеденроллментенаблед заданное значение.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dca8bdc3a2c6a5a3baec94c079d2a67ed6bb25ab
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49254463"
---
# <a name="setandroiddeviceownerfullymanagedenrollmentstate-action"></a><span data-ttu-id="49179-103">Действие setAndroidDeviceOwnerFullyManagedEnrollmentState</span><span class="sxs-lookup"><span data-stu-id="49179-103">setAndroidDeviceOwnerFullyManagedEnrollmentState action</span></span>

<span data-ttu-id="49179-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49179-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49179-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49179-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49179-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49179-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49179-107">Задает для ресурса androidmanagedstoreaccountenterprisesettings Андроиддевицеовнерфуллиманажеденроллментенаблед заданное значение.</span><span class="sxs-lookup"><span data-stu-id="49179-107">Sets the AndroidManagedStoreAccountEnterpriseSettings AndroidDeviceOwnerFullyManagedEnrollmentEnabled to the given value.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49179-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="49179-108">Prerequisites</span></span>
<span data-ttu-id="49179-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49179-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49179-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49179-111">Permission type</span></span>|<span data-ttu-id="49179-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="49179-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49179-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49179-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49179-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49179-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="49179-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49179-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49179-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49179-116">Not supported.</span></span>|
|<span data-ttu-id="49179-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="49179-117">Application</span></span>|<span data-ttu-id="49179-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49179-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49179-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49179-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/setAndroidDeviceOwnerFullyManagedEnrollmentState
```

## <a name="request-headers"></a><span data-ttu-id="49179-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="49179-120">Request headers</span></span>
|<span data-ttu-id="49179-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="49179-121">Header</span></span>|<span data-ttu-id="49179-122">Значение</span><span class="sxs-lookup"><span data-stu-id="49179-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49179-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49179-123">Authorization</span></span>|<span data-ttu-id="49179-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49179-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49179-125">Accept</span><span class="sxs-lookup"><span data-stu-id="49179-125">Accept</span></span>|<span data-ttu-id="49179-126">application/json</span><span class="sxs-lookup"><span data-stu-id="49179-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49179-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49179-127">Request body</span></span>
<span data-ttu-id="49179-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49179-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="49179-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="49179-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="49179-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="49179-130">Property</span></span>|<span data-ttu-id="49179-131">Тип</span><span class="sxs-lookup"><span data-stu-id="49179-131">Type</span></span>|<span data-ttu-id="49179-132">Описание</span><span class="sxs-lookup"><span data-stu-id="49179-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49179-133">enabled</span><span class="sxs-lookup"><span data-stu-id="49179-133">enabled</span></span>|<span data-ttu-id="49179-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="49179-134">Boolean</span></span>|<span data-ttu-id="49179-135">Значение, с которым устанавливается Андроиддевицеовнерфуллиманажеденроллментенаблед.</span><span class="sxs-lookup"><span data-stu-id="49179-135">The value to set AndroidDeviceOwnerFullyManagedEnrollmentEnabled to.</span></span>|



## <a name="response"></a><span data-ttu-id="49179-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="49179-136">Response</span></span>
<span data-ttu-id="49179-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="49179-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="49179-138">Пример</span><span class="sxs-lookup"><span data-stu-id="49179-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="49179-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="49179-139">Request</span></span>
<span data-ttu-id="49179-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49179-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/setAndroidDeviceOwnerFullyManagedEnrollmentState

Content-type: application/json
Content-length: 23

{
  "enabled": true
}
```

### <a name="response"></a><span data-ttu-id="49179-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="49179-141">Response</span></span>
<span data-ttu-id="49179-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49179-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




