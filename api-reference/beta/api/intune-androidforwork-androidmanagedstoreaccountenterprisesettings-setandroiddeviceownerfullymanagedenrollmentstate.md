---
title: Действие setAndroidDeviceOwnerFullyManagedEnrollmentState
description: Задает для ресурса androidmanagedstoreaccountenterprisesettings Андроиддевицеовнерфуллиманажеденроллментенаблед заданное значение.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4301f4b58650f13bf94f37085ed3b4b07e68f329
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977767"
---
# <a name="setandroiddeviceownerfullymanagedenrollmentstate-action"></a><span data-ttu-id="2aff3-103">Действие setAndroidDeviceOwnerFullyManagedEnrollmentState</span><span class="sxs-lookup"><span data-stu-id="2aff3-103">setAndroidDeviceOwnerFullyManagedEnrollmentState action</span></span>

> <span data-ttu-id="2aff3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2aff3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2aff3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2aff3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2aff3-106">Задает для ресурса androidmanagedstoreaccountenterprisesettings Андроиддевицеовнерфуллиманажеденроллментенаблед заданное значение.</span><span class="sxs-lookup"><span data-stu-id="2aff3-106">Sets the AndroidManagedStoreAccountEnterpriseSettings AndroidDeviceOwnerFullyManagedEnrollmentEnabled to the given value.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2aff3-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2aff3-107">Prerequisites</span></span>
<span data-ttu-id="2aff3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2aff3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2aff3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2aff3-110">Permission type</span></span>|<span data-ttu-id="2aff3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2aff3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2aff3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2aff3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2aff3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2aff3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2aff3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2aff3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2aff3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2aff3-115">Not supported.</span></span>|
|<span data-ttu-id="2aff3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2aff3-116">Application</span></span>|<span data-ttu-id="2aff3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2aff3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2aff3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2aff3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/setAndroidDeviceOwnerFullyManagedEnrollmentState
```

## <a name="request-headers"></a><span data-ttu-id="2aff3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2aff3-119">Request headers</span></span>
|<span data-ttu-id="2aff3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2aff3-120">Header</span></span>|<span data-ttu-id="2aff3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2aff3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2aff3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2aff3-122">Authorization</span></span>|<span data-ttu-id="2aff3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2aff3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2aff3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2aff3-124">Accept</span></span>|<span data-ttu-id="2aff3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2aff3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2aff3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2aff3-126">Request body</span></span>
<span data-ttu-id="2aff3-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2aff3-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2aff3-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="2aff3-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2aff3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2aff3-129">Property</span></span>|<span data-ttu-id="2aff3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2aff3-130">Type</span></span>|<span data-ttu-id="2aff3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2aff3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2aff3-132">enabled</span><span class="sxs-lookup"><span data-stu-id="2aff3-132">enabled</span></span>|<span data-ttu-id="2aff3-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="2aff3-133">Boolean</span></span>|<span data-ttu-id="2aff3-134">Значение, с которым устанавливается Андроиддевицеовнерфуллиманажеденроллментенаблед.</span><span class="sxs-lookup"><span data-stu-id="2aff3-134">The value to set AndroidDeviceOwnerFullyManagedEnrollmentEnabled to.</span></span>|



## <a name="response"></a><span data-ttu-id="2aff3-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="2aff3-135">Response</span></span>
<span data-ttu-id="2aff3-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2aff3-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2aff3-137">Пример</span><span class="sxs-lookup"><span data-stu-id="2aff3-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="2aff3-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="2aff3-138">Request</span></span>
<span data-ttu-id="2aff3-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2aff3-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/setAndroidDeviceOwnerFullyManagedEnrollmentState

Content-type: application/json
Content-length: 23

{
  "enabled": true
}
```

### <a name="response"></a><span data-ttu-id="2aff3-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="2aff3-140">Response</span></span>
<span data-ttu-id="2aff3-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2aff3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




