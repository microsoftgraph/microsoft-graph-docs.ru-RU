---
title: Обновление объекта reportRoot
description: Обновление свойств объекта reportRoot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ca91c074e19887d889ac8bed332055f36ebed08d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694181"
---
# <a name="update-reportroot"></a><span data-ttu-id="d5a8e-103">Обновление объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="d5a8e-103">Update reportRoot</span></span>

<span data-ttu-id="d5a8e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5a8e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5a8e-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d5a8e-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d5a8e-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5a8e-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5a8e-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d5a8e-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5a8e-108">Обновление свойств объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="d5a8e-108">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d5a8e-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d5a8e-109">Prerequisites</span></span>
<span data-ttu-id="d5a8e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5a8e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5a8e-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5a8e-112">Permission type</span></span>|<span data-ttu-id="d5a8e-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5a8e-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5a8e-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5a8e-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d5a8e-115">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="d5a8e-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d5a8e-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5a8e-116">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="d5a8e-117">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="d5a8e-117">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="d5a8e-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5a8e-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d5a8e-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5a8e-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5a8e-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5a8e-120">Not supported.</span></span>|
|<span data-ttu-id="d5a8e-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5a8e-121">Application</span></span>||
| <span data-ttu-id="d5a8e-122">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="d5a8e-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d5a8e-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5a8e-123">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="d5a8e-124">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="d5a8e-124">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="d5a8e-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5a8e-125">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5a8e-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5a8e-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="d5a8e-127">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d5a8e-127">Request headers</span></span>
|<span data-ttu-id="d5a8e-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d5a8e-128">Header</span></span>|<span data-ttu-id="d5a8e-129">Значение</span><span class="sxs-lookup"><span data-stu-id="d5a8e-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5a8e-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5a8e-130">Authorization</span></span>|<span data-ttu-id="d5a8e-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5a8e-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5a8e-132">Accept</span><span class="sxs-lookup"><span data-stu-id="d5a8e-132">Accept</span></span>|<span data-ttu-id="d5a8e-133">application/json</span><span class="sxs-lookup"><span data-stu-id="d5a8e-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5a8e-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d5a8e-134">Request body</span></span>
<span data-ttu-id="d5a8e-135">В тексте запроса добавьте представление объекта [reportRoot](../resources/intune-shared-reportroot.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d5a8e-135">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="d5a8e-136">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="d5a8e-136">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="d5a8e-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="d5a8e-137">Property</span></span>|<span data-ttu-id="d5a8e-138">Тип</span><span class="sxs-lookup"><span data-stu-id="d5a8e-138">Type</span></span>|<span data-ttu-id="d5a8e-139">Описание</span><span class="sxs-lookup"><span data-stu-id="d5a8e-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5a8e-140">id</span><span class="sxs-lookup"><span data-stu-id="d5a8e-140">id</span></span>|<span data-ttu-id="d5a8e-141">Строка</span><span class="sxs-lookup"><span data-stu-id="d5a8e-141">String</span></span>|<span data-ttu-id="d5a8e-142">Уникальный идентификатор для этого объекта.</span><span class="sxs-lookup"><span data-stu-id="d5a8e-142">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="d5a8e-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5a8e-143">Response</span></span>
<span data-ttu-id="d5a8e-144">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [reportRoot](../resources/intune-shared-reportroot.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d5a8e-144">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5a8e-145">Пример</span><span class="sxs-lookup"><span data-stu-id="d5a8e-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="d5a8e-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5a8e-146">Request</span></span>
<span data-ttu-id="d5a8e-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5a8e-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="d5a8e-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5a8e-148">Response</span></span>
<span data-ttu-id="d5a8e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d5a8e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```











