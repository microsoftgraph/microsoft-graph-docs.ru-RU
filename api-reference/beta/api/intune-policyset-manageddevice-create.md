---
title: Create managedDevice
description: Создание объекта managedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 55dd88ff22b4498083afa695271f3c13d7cc71a6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160592"
---
# <a name="create-manageddevice"></a><span data-ttu-id="5babb-103">Create managedDevice</span><span class="sxs-lookup"><span data-stu-id="5babb-103">Create managedDevice</span></span>

<span data-ttu-id="5babb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5babb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5babb-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5babb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5babb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5babb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5babb-107">Создание объекта [managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="5babb-107">Create a new [managedDevice](../resources/intune-shared-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5babb-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5babb-108">Prerequisites</span></span>
<span data-ttu-id="5babb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5babb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5babb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5babb-111">Permission type</span></span>|<span data-ttu-id="5babb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5babb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5babb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5babb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5babb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5babb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5babb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5babb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5babb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5babb-116">Not supported.</span></span>|
|<span data-ttu-id="5babb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5babb-117">Application</span></span>|<span data-ttu-id="5babb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5babb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5babb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5babb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="5babb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5babb-120">Request headers</span></span>
|<span data-ttu-id="5babb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5babb-121">Header</span></span>|<span data-ttu-id="5babb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5babb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5babb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5babb-123">Authorization</span></span>|<span data-ttu-id="5babb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5babb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5babb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5babb-125">Accept</span></span>|<span data-ttu-id="5babb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5babb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5babb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5babb-127">Request body</span></span>
<span data-ttu-id="5babb-128">В тексте запроса добавьте представление объекта managedDevice в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5babb-128">In the request body, supply a JSON representation for the managedDevice object.</span></span>

<span data-ttu-id="5babb-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта managedDevice.</span><span class="sxs-lookup"><span data-stu-id="5babb-129">The following table shows the properties that are required when you create the managedDevice.</span></span>

|<span data-ttu-id="5babb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5babb-130">Property</span></span>|<span data-ttu-id="5babb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5babb-131">Type</span></span>|<span data-ttu-id="5babb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5babb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5babb-133">id</span><span class="sxs-lookup"><span data-stu-id="5babb-133">id</span></span>|<span data-ttu-id="5babb-134">String</span><span class="sxs-lookup"><span data-stu-id="5babb-134">String</span></span>|<span data-ttu-id="5babb-135">Ключ сущности управляемого устройства.</span><span class="sxs-lookup"><span data-stu-id="5babb-135">Key of Managed device entity.</span></span>|



## <a name="response"></a><span data-ttu-id="5babb-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="5babb-136">Response</span></span>
<span data-ttu-id="5babb-137">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedDevice](../resources/intune-shared-manageddevice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5babb-137">If successful, this method returns a `201 Created` response code and a [managedDevice](../resources/intune-shared-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5babb-138">Пример</span><span class="sxs-lookup"><span data-stu-id="5babb-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="5babb-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="5babb-139">Request</span></span>
<span data-ttu-id="5babb-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5babb-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices
Content-type: application/json
Content-length: 55

{
  "@odata.type": "#microsoft.graph.managedDevice"
}
```

### <a name="response"></a><span data-ttu-id="5babb-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="5babb-141">Response</span></span>
<span data-ttu-id="5babb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5babb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 104

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "705c034c-034c-705c-4c03-5c704c035c70"
}
```




