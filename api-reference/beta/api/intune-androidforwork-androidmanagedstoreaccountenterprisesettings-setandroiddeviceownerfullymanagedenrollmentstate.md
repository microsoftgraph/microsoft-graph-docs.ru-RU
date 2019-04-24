---
title: Действие setAndroidDeviceOwnerFullyManagedEnrollmentState
description: Задает для ресурса androidmanagedstoreaccountenterprisesettings Андроиддевицеовнерфуллиманажеденроллментенаблед заданное значение.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f5d4ef69d4cdc2087bdbcac3d4ca34ad76036391
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32498314"
---
# <a name="setandroiddeviceownerfullymanagedenrollmentstate-action"></a><span data-ttu-id="e6398-103">Действие setAndroidDeviceOwnerFullyManagedEnrollmentState</span><span class="sxs-lookup"><span data-stu-id="e6398-103">setAndroidDeviceOwnerFullyManagedEnrollmentState action</span></span>

> <span data-ttu-id="e6398-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6398-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6398-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e6398-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6398-106">Задает для ресурса androidmanagedstoreaccountenterprisesettings Андроиддевицеовнерфуллиманажеденроллментенаблед заданное значение.</span><span class="sxs-lookup"><span data-stu-id="e6398-106">Sets the AndroidManagedStoreAccountEnterpriseSettings AndroidDeviceOwnerFullyManagedEnrollmentEnabled to the given value.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6398-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e6398-107">Prerequisites</span></span>
<span data-ttu-id="e6398-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6398-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6398-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6398-110">Permission type</span></span>|<span data-ttu-id="e6398-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6398-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6398-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6398-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e6398-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6398-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e6398-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6398-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6398-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6398-115">Not supported.</span></span>|
|<span data-ttu-id="e6398-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6398-116">Application</span></span>|<span data-ttu-id="e6398-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6398-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6398-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6398-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/setAndroidDeviceOwnerFullyManagedEnrollmentState
```

## <a name="request-headers"></a><span data-ttu-id="e6398-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6398-119">Request headers</span></span>
|<span data-ttu-id="e6398-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e6398-120">Header</span></span>|<span data-ttu-id="e6398-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e6398-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6398-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6398-122">Authorization</span></span>|<span data-ttu-id="e6398-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6398-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6398-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e6398-124">Accept</span></span>|<span data-ttu-id="e6398-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e6398-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6398-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e6398-126">Request body</span></span>
<span data-ttu-id="e6398-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6398-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e6398-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="e6398-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e6398-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6398-129">Property</span></span>|<span data-ttu-id="e6398-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e6398-130">Type</span></span>|<span data-ttu-id="e6398-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e6398-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6398-132">enabled</span><span class="sxs-lookup"><span data-stu-id="e6398-132">enabled</span></span>|<span data-ttu-id="e6398-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6398-133">Boolean</span></span>|<span data-ttu-id="e6398-134">Значение, с которым устанавливается Андроиддевицеовнерфуллиманажеденроллментенаблед.</span><span class="sxs-lookup"><span data-stu-id="e6398-134">The value to set AndroidDeviceOwnerFullyManagedEnrollmentEnabled to.</span></span>|



## <a name="response"></a><span data-ttu-id="e6398-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="e6398-135">Response</span></span>
<span data-ttu-id="e6398-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e6398-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e6398-137">Пример</span><span class="sxs-lookup"><span data-stu-id="e6398-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6398-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6398-138">Request</span></span>
<span data-ttu-id="e6398-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6398-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/setAndroidDeviceOwnerFullyManagedEnrollmentState

Content-type: application/json
Content-length: 23

{
  "enabled": true
}
```

### <a name="response"></a><span data-ttu-id="e6398-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6398-140">Response</span></span>
<span data-ttu-id="e6398-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e6398-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





