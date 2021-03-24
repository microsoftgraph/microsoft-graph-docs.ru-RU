---
title: Действие setAndroidDeviceOwnerFullyManagedEnrollmentState
description: Задает Значение AndroidManagedStoreAccountEnterpriseSettings AndroidDeviceOwnerFullyManagedEnrollmentEnabled.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 128732953ae8481dfddce30da23c3e83fa9b0fda
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144643"
---
# <a name="setandroiddeviceownerfullymanagedenrollmentstate-action"></a><span data-ttu-id="a80ee-103">Действие setAndroidDeviceOwnerFullyManagedEnrollmentState</span><span class="sxs-lookup"><span data-stu-id="a80ee-103">setAndroidDeviceOwnerFullyManagedEnrollmentState action</span></span>

<span data-ttu-id="a80ee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a80ee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a80ee-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a80ee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a80ee-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a80ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a80ee-107">Задает Значение AndroidManagedStoreAccountEnterpriseSettings AndroidDeviceOwnerFullyManagedEnrollmentEnabled.</span><span class="sxs-lookup"><span data-stu-id="a80ee-107">Sets the AndroidManagedStoreAccountEnterpriseSettings AndroidDeviceOwnerFullyManagedEnrollmentEnabled to the given value.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a80ee-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a80ee-108">Prerequisites</span></span>
<span data-ttu-id="a80ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a80ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a80ee-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a80ee-111">Permission type</span></span>|<span data-ttu-id="a80ee-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a80ee-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a80ee-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a80ee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a80ee-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a80ee-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a80ee-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a80ee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a80ee-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a80ee-116">Not supported.</span></span>|
|<span data-ttu-id="a80ee-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a80ee-117">Application</span></span>|<span data-ttu-id="a80ee-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a80ee-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a80ee-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a80ee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/setAndroidDeviceOwnerFullyManagedEnrollmentState
```

## <a name="request-headers"></a><span data-ttu-id="a80ee-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a80ee-120">Request headers</span></span>
|<span data-ttu-id="a80ee-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a80ee-121">Header</span></span>|<span data-ttu-id="a80ee-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a80ee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a80ee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a80ee-123">Authorization</span></span>|<span data-ttu-id="a80ee-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a80ee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a80ee-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a80ee-125">Accept</span></span>|<span data-ttu-id="a80ee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a80ee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a80ee-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a80ee-127">Request body</span></span>
<span data-ttu-id="a80ee-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a80ee-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a80ee-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="a80ee-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a80ee-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a80ee-130">Property</span></span>|<span data-ttu-id="a80ee-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a80ee-131">Type</span></span>|<span data-ttu-id="a80ee-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a80ee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a80ee-133">enabled</span><span class="sxs-lookup"><span data-stu-id="a80ee-133">enabled</span></span>|<span data-ttu-id="a80ee-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="a80ee-134">Boolean</span></span>|<span data-ttu-id="a80ee-135">Значение для набора AndroidDeviceOwnerFullyManagedEnrollmentEnabled.</span><span class="sxs-lookup"><span data-stu-id="a80ee-135">The value to set AndroidDeviceOwnerFullyManagedEnrollmentEnabled to.</span></span>|



## <a name="response"></a><span data-ttu-id="a80ee-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="a80ee-136">Response</span></span>
<span data-ttu-id="a80ee-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a80ee-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a80ee-138">Пример</span><span class="sxs-lookup"><span data-stu-id="a80ee-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="a80ee-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a80ee-139">Request</span></span>
<span data-ttu-id="a80ee-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a80ee-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/setAndroidDeviceOwnerFullyManagedEnrollmentState

Content-type: application/json
Content-length: 23

{
  "enabled": true
}
```

### <a name="response"></a><span data-ttu-id="a80ee-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a80ee-141">Response</span></span>
<span data-ttu-id="a80ee-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a80ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




