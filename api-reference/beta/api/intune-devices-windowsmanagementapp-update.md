---
title: Обновление WindowsManagementApp
description: Обновление свойств объекта WindowsManagementApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 15fea6f46279f96ce3d1f235b92475bdc67d0f16
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52662944"
---
# <a name="update-windowsmanagementapp"></a><span data-ttu-id="2f18b-103">Обновление WindowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="2f18b-103">Update windowsManagementApp</span></span>

<span data-ttu-id="2f18b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f18b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f18b-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f18b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f18b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f18b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f18b-107">Обновление свойств объекта [WindowsManagementApp.](../resources/intune-devices-windowsmanagementapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f18b-107">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f18b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2f18b-108">Prerequisites</span></span>
<span data-ttu-id="2f18b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f18b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f18b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f18b-111">Permission type</span></span>|<span data-ttu-id="2f18b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f18b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f18b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f18b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f18b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f18b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2f18b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f18b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f18b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f18b-116">Not supported.</span></span>|
|<span data-ttu-id="2f18b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2f18b-117">Application</span></span>|<span data-ttu-id="2f18b-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f18b-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f18b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f18b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp
```

## <a name="request-headers"></a><span data-ttu-id="2f18b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2f18b-120">Request headers</span></span>
|<span data-ttu-id="2f18b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f18b-121">Header</span></span>|<span data-ttu-id="2f18b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2f18b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f18b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f18b-123">Authorization</span></span>|<span data-ttu-id="2f18b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f18b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f18b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2f18b-125">Accept</span></span>|<span data-ttu-id="2f18b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f18b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f18b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f18b-127">Request body</span></span>
<span data-ttu-id="2f18b-128">В теле запроса поставляем представление JSON для [объекта WindowsManagementApp.](../resources/intune-devices-windowsmanagementapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f18b-128">In the request body, supply a JSON representation for the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

<span data-ttu-id="2f18b-129">В следующей таблице показаны свойства, необходимые при создании [windowsManagementApp.](../resources/intune-devices-windowsmanagementapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f18b-129">The following table shows the properties that are required when you create the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span></span>

|<span data-ttu-id="2f18b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f18b-130">Property</span></span>|<span data-ttu-id="2f18b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2f18b-131">Type</span></span>|<span data-ttu-id="2f18b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2f18b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f18b-133">id</span><span class="sxs-lookup"><span data-stu-id="2f18b-133">id</span></span>|<span data-ttu-id="2f18b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="2f18b-134">String</span></span>|<span data-ttu-id="2f18b-135">Уникальный идентификатор для приложения Windows управления</span><span class="sxs-lookup"><span data-stu-id="2f18b-135">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="2f18b-136">availableVersion</span><span class="sxs-lookup"><span data-stu-id="2f18b-136">availableVersion</span></span>|<span data-ttu-id="2f18b-137">Строка</span><span class="sxs-lookup"><span data-stu-id="2f18b-137">String</span></span>|<span data-ttu-id="2f18b-138">Windows доступной версии приложения для управления.</span><span class="sxs-lookup"><span data-stu-id="2f18b-138">Windows management app available version.</span></span>|
|<span data-ttu-id="2f18b-139">managedInstaller</span><span class="sxs-lookup"><span data-stu-id="2f18b-139">managedInstaller</span></span>|[<span data-ttu-id="2f18b-140">managedInstallerStatus</span><span class="sxs-lookup"><span data-stu-id="2f18b-140">managedInstallerStatus</span></span>](../resources/intune-devices-managedinstallerstatus.md)|<span data-ttu-id="2f18b-141">Состояние управляемого установщика.</span><span class="sxs-lookup"><span data-stu-id="2f18b-141">Managed Installer Status.</span></span> <span data-ttu-id="2f18b-142">Возможные значения: `disabled`, `enabled`.</span><span class="sxs-lookup"><span data-stu-id="2f18b-142">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="2f18b-143">managedInstallerConfiguredDateTime</span><span class="sxs-lookup"><span data-stu-id="2f18b-143">managedInstallerConfiguredDateTime</span></span>|<span data-ttu-id="2f18b-144">Строка</span><span class="sxs-lookup"><span data-stu-id="2f18b-144">String</span></span>|<span data-ttu-id="2f18b-145">Настроено время даты управляемого установщика</span><span class="sxs-lookup"><span data-stu-id="2f18b-145">Managed Installer Configured Date Time</span></span>|



## <a name="response"></a><span data-ttu-id="2f18b-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f18b-146">Response</span></span>
<span data-ttu-id="2f18b-147">В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект WindowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2f18b-147">If successful, this method returns a `200 OK` response code and an updated [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f18b-148">Пример</span><span class="sxs-lookup"><span data-stu-id="2f18b-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f18b-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f18b-149">Request</span></span>
<span data-ttu-id="2f18b-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f18b-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp
Content-type: application/json
Content-length: 235

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "availableVersion": "Available Version value",
  "managedInstaller": "enabled",
  "managedInstallerConfiguredDateTime": "Managed Installer Configured Date Time value"
}
```

### <a name="response"></a><span data-ttu-id="2f18b-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f18b-151">Response</span></span>
<span data-ttu-id="2f18b-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f18b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 284

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "5facc79c-c79c-5fac-9cc7-ac5f9cc7ac5f",
  "availableVersion": "Available Version value",
  "managedInstaller": "enabled",
  "managedInstallerConfiguredDateTime": "Managed Installer Configured Date Time value"
}
```




