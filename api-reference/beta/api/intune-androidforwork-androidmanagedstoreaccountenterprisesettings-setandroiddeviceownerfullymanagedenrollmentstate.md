---
title: Действие setAndroidDeviceOwnerFullyManagedEnrollmentState
description: Задает для ресурса androidmanagedstoreaccountenterprisesettings Андроиддевицеовнерфуллиманажеденроллментенаблед заданное значение.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9a2517b59705ae8f46294b521aa5132c8bd8b1f4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148918"
---
# <a name="setandroiddeviceownerfullymanagedenrollmentstate-action"></a><span data-ttu-id="290af-103">Действие setAndroidDeviceOwnerFullyManagedEnrollmentState</span><span class="sxs-lookup"><span data-stu-id="290af-103">setAndroidDeviceOwnerFullyManagedEnrollmentState action</span></span>

> <span data-ttu-id="290af-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="290af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="290af-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="290af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="290af-106">Задает для ресурса androidmanagedstoreaccountenterprisesettings Андроиддевицеовнерфуллиманажеденроллментенаблед заданное значение.</span><span class="sxs-lookup"><span data-stu-id="290af-106">Sets the AndroidManagedStoreAccountEnterpriseSettings AndroidDeviceOwnerFullyManagedEnrollmentEnabled to the given value.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="290af-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="290af-107">Prerequisites</span></span>
<span data-ttu-id="290af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="290af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="290af-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="290af-110">Permission type</span></span>|<span data-ttu-id="290af-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="290af-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="290af-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="290af-112">Delegated (work or school account)</span></span>|<span data-ttu-id="290af-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="290af-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="290af-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="290af-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="290af-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="290af-115">Not supported.</span></span>|
|<span data-ttu-id="290af-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="290af-116">Application</span></span>|<span data-ttu-id="290af-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="290af-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="290af-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="290af-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/setAndroidDeviceOwnerFullyManagedEnrollmentState
```

## <a name="request-headers"></a><span data-ttu-id="290af-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="290af-119">Request headers</span></span>
|<span data-ttu-id="290af-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="290af-120">Header</span></span>|<span data-ttu-id="290af-121">Значение</span><span class="sxs-lookup"><span data-stu-id="290af-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="290af-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="290af-122">Authorization</span></span>|<span data-ttu-id="290af-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="290af-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="290af-124">Accept</span><span class="sxs-lookup"><span data-stu-id="290af-124">Accept</span></span>|<span data-ttu-id="290af-125">application/json</span><span class="sxs-lookup"><span data-stu-id="290af-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="290af-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="290af-126">Request body</span></span>
<span data-ttu-id="290af-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="290af-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="290af-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="290af-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="290af-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="290af-129">Property</span></span>|<span data-ttu-id="290af-130">Тип</span><span class="sxs-lookup"><span data-stu-id="290af-130">Type</span></span>|<span data-ttu-id="290af-131">Описание</span><span class="sxs-lookup"><span data-stu-id="290af-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="290af-132">enabled</span><span class="sxs-lookup"><span data-stu-id="290af-132">enabled</span></span>|<span data-ttu-id="290af-133">Логический</span><span class="sxs-lookup"><span data-stu-id="290af-133">Boolean</span></span>|<span data-ttu-id="290af-134">Значение, с которым устанавливается Андроиддевицеовнерфуллиманажеденроллментенаблед.</span><span class="sxs-lookup"><span data-stu-id="290af-134">The value to set AndroidDeviceOwnerFullyManagedEnrollmentEnabled to.</span></span>|



## <a name="response"></a><span data-ttu-id="290af-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="290af-135">Response</span></span>
<span data-ttu-id="290af-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="290af-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="290af-137">Пример</span><span class="sxs-lookup"><span data-stu-id="290af-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="290af-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="290af-138">Request</span></span>
<span data-ttu-id="290af-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="290af-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/setAndroidDeviceOwnerFullyManagedEnrollmentState

Content-type: application/json
Content-length: 23

{
  "enabled": true
}
```

### <a name="response"></a><span data-ttu-id="290af-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="290af-140">Response</span></span>
<span data-ttu-id="290af-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="290af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




