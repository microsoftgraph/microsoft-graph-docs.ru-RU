---
title: Обновление windowsManagementApp
description: Обновление свойств объекта windowsManagementApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 895626cdaac3f43342100c39de1845abddccc53b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49218763"
---
# <a name="update-windowsmanagementapp"></a><span data-ttu-id="78830-103">Обновление windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="78830-103">Update windowsManagementApp</span></span>

<span data-ttu-id="78830-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78830-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78830-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78830-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78830-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="78830-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78830-107">Обновление свойств объекта [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="78830-107">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78830-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="78830-108">Prerequisites</span></span>
<span data-ttu-id="78830-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78830-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78830-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="78830-111">Permission type</span></span>|<span data-ttu-id="78830-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="78830-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78830-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="78830-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78830-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78830-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="78830-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="78830-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78830-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78830-116">Not supported.</span></span>|
|<span data-ttu-id="78830-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="78830-117">Application</span></span>|<span data-ttu-id="78830-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78830-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="78830-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="78830-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp
```

## <a name="request-headers"></a><span data-ttu-id="78830-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="78830-120">Request headers</span></span>
|<span data-ttu-id="78830-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="78830-121">Header</span></span>|<span data-ttu-id="78830-122">Значение</span><span class="sxs-lookup"><span data-stu-id="78830-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78830-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="78830-123">Authorization</span></span>|<span data-ttu-id="78830-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="78830-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78830-125">Accept</span><span class="sxs-lookup"><span data-stu-id="78830-125">Accept</span></span>|<span data-ttu-id="78830-126">application/json</span><span class="sxs-lookup"><span data-stu-id="78830-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78830-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="78830-127">Request body</span></span>
<span data-ttu-id="78830-128">В тексте запроса добавьте представление объекта [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="78830-128">In the request body, supply a JSON representation for the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

<span data-ttu-id="78830-129">В следующей таблице приведены свойства, необходимые при создании [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span><span class="sxs-lookup"><span data-stu-id="78830-129">The following table shows the properties that are required when you create the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span></span>

|<span data-ttu-id="78830-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="78830-130">Property</span></span>|<span data-ttu-id="78830-131">Тип</span><span class="sxs-lookup"><span data-stu-id="78830-131">Type</span></span>|<span data-ttu-id="78830-132">Описание</span><span class="sxs-lookup"><span data-stu-id="78830-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78830-133">id</span><span class="sxs-lookup"><span data-stu-id="78830-133">id</span></span>|<span data-ttu-id="78830-134">String</span><span class="sxs-lookup"><span data-stu-id="78830-134">String</span></span>|<span data-ttu-id="78830-135">Уникальный идентификатор для приложения управления Windows</span><span class="sxs-lookup"><span data-stu-id="78830-135">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="78830-136">availableVersion</span><span class="sxs-lookup"><span data-stu-id="78830-136">availableVersion</span></span>|<span data-ttu-id="78830-137">String</span><span class="sxs-lookup"><span data-stu-id="78830-137">String</span></span>|<span data-ttu-id="78830-138">Доступная версия приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="78830-138">Windows management app available version.</span></span>|



## <a name="response"></a><span data-ttu-id="78830-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="78830-139">Response</span></span>
<span data-ttu-id="78830-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="78830-140">If successful, this method returns a `200 OK` response code and an updated [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78830-141">Пример</span><span class="sxs-lookup"><span data-stu-id="78830-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="78830-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="78830-142">Request</span></span>
<span data-ttu-id="78830-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="78830-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp
Content-type: application/json
Content-length: 112

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "availableVersion": "Available Version value"
}
```

### <a name="response"></a><span data-ttu-id="78830-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="78830-144">Response</span></span>
<span data-ttu-id="78830-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="78830-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 161

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "5facc79c-c79c-5fac-9cc7-ac5f9cc7ac5f",
  "availableVersion": "Available Version value"
}
```




