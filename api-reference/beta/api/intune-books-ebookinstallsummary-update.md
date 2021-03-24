---
title: Update eBookInstallSummary
description: Обновление свойств объекта eBookInstallSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 56f16314672e5b5beb8a3a7fbeee5693aca4e4ca
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126929"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="6033d-103">Update eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="6033d-103">Update eBookInstallSummary</span></span>

<span data-ttu-id="6033d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6033d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6033d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6033d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6033d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6033d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6033d-107">Обновление свойств объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="6033d-107">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6033d-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6033d-108">Prerequisites</span></span>
<span data-ttu-id="6033d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6033d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6033d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6033d-111">Permission type</span></span>|<span data-ttu-id="6033d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6033d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6033d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6033d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6033d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6033d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6033d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6033d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6033d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6033d-116">Not supported.</span></span>|
|<span data-ttu-id="6033d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="6033d-117">Application</span></span>|<span data-ttu-id="6033d-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6033d-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6033d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6033d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="6033d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6033d-120">Request headers</span></span>
|<span data-ttu-id="6033d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6033d-121">Header</span></span>|<span data-ttu-id="6033d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6033d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6033d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6033d-123">Authorization</span></span>|<span data-ttu-id="6033d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6033d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6033d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6033d-125">Accept</span></span>|<span data-ttu-id="6033d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6033d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6033d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6033d-127">Request body</span></span>
<span data-ttu-id="6033d-128">В теле запроса добавьте представление объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6033d-128">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="6033d-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="6033d-129">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="6033d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6033d-130">Property</span></span>|<span data-ttu-id="6033d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6033d-131">Type</span></span>|<span data-ttu-id="6033d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6033d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6033d-133">id</span><span class="sxs-lookup"><span data-stu-id="6033d-133">id</span></span>|<span data-ttu-id="6033d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="6033d-134">String</span></span>|<span data-ttu-id="6033d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6033d-135">Key of the entity.</span></span>|
|<span data-ttu-id="6033d-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6033d-136">installedDeviceCount</span></span>|<span data-ttu-id="6033d-137">Int32</span><span class="sxs-lookup"><span data-stu-id="6033d-137">Int32</span></span>|<span data-ttu-id="6033d-138">Количество устройств, на которых была успешно установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="6033d-138">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="6033d-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6033d-139">failedDeviceCount</span></span>|<span data-ttu-id="6033d-140">Int32</span><span class="sxs-lookup"><span data-stu-id="6033d-140">Int32</span></span>|<span data-ttu-id="6033d-141">Количество устройств, на которых не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="6033d-141">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="6033d-142">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6033d-142">notInstalledDeviceCount</span></span>|<span data-ttu-id="6033d-143">Int32</span><span class="sxs-lookup"><span data-stu-id="6033d-143">Int32</span></span>|<span data-ttu-id="6033d-144">Количество устройств, на которых не установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="6033d-144">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="6033d-145">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="6033d-145">installedUserCount</span></span>|<span data-ttu-id="6033d-146">Int32</span><span class="sxs-lookup"><span data-stu-id="6033d-146">Int32</span></span>|<span data-ttu-id="6033d-147">Количество пользователей, которым удалось установить эту книгу на всех своих устройствах.</span><span class="sxs-lookup"><span data-stu-id="6033d-147">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="6033d-148">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="6033d-148">failedUserCount</span></span>|<span data-ttu-id="6033d-149">Int32</span><span class="sxs-lookup"><span data-stu-id="6033d-149">Int32</span></span>|<span data-ttu-id="6033d-150">Количество пользователей, у которых есть одно или несколько устройств, где не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="6033d-150">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="6033d-151">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="6033d-151">notInstalledUserCount</span></span>|<span data-ttu-id="6033d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6033d-152">Int32</span></span>|<span data-ttu-id="6033d-153">Количество пользователей, не установивших эту книгу.</span><span class="sxs-lookup"><span data-stu-id="6033d-153">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="6033d-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="6033d-154">Response</span></span>
<span data-ttu-id="6033d-155">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6033d-155">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6033d-156">Пример</span><span class="sxs-lookup"><span data-stu-id="6033d-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="6033d-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="6033d-157">Request</span></span>
<span data-ttu-id="6033d-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6033d-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```

### <a name="response"></a><span data-ttu-id="6033d-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="6033d-159">Response</span></span>
<span data-ttu-id="6033d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6033d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "9708ad78-ad78-9708-78ad-089778ad0897",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```




