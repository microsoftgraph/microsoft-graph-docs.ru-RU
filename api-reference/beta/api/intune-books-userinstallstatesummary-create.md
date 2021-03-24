---
title: Создание объекта userInstallStateSummary
description: Создание объекта userInstallStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5226053e0deff2508138d6448f6e089e0fad99e8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132998"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="47faa-103">Создание объекта userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="47faa-103">Create userInstallStateSummary</span></span>

<span data-ttu-id="47faa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47faa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47faa-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47faa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47faa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47faa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47faa-107">Создание объекта [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="47faa-107">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47faa-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="47faa-108">Prerequisites</span></span>
<span data-ttu-id="47faa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47faa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47faa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47faa-111">Permission type</span></span>|<span data-ttu-id="47faa-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47faa-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47faa-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47faa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47faa-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47faa-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="47faa-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47faa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47faa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47faa-116">Not supported.</span></span>|
|<span data-ttu-id="47faa-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="47faa-117">Application</span></span>|<span data-ttu-id="47faa-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47faa-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47faa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47faa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="47faa-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="47faa-120">Request headers</span></span>
|<span data-ttu-id="47faa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47faa-121">Header</span></span>|<span data-ttu-id="47faa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="47faa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47faa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="47faa-123">Authorization</span></span>|<span data-ttu-id="47faa-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47faa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47faa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="47faa-125">Accept</span></span>|<span data-ttu-id="47faa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="47faa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47faa-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47faa-127">Request body</span></span>
<span data-ttu-id="47faa-128">В тексте запроса добавьте представление объекта userInstallStateSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47faa-128">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="47faa-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта userInstallStateSummary.</span><span class="sxs-lookup"><span data-stu-id="47faa-129">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="47faa-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="47faa-130">Property</span></span>|<span data-ttu-id="47faa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="47faa-131">Type</span></span>|<span data-ttu-id="47faa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="47faa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47faa-133">id</span><span class="sxs-lookup"><span data-stu-id="47faa-133">id</span></span>|<span data-ttu-id="47faa-134">Строка</span><span class="sxs-lookup"><span data-stu-id="47faa-134">String</span></span>|<span data-ttu-id="47faa-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="47faa-135">Key of the entity.</span></span>|
|<span data-ttu-id="47faa-136">userName</span><span class="sxs-lookup"><span data-stu-id="47faa-136">userName</span></span>|<span data-ttu-id="47faa-137">String</span><span class="sxs-lookup"><span data-stu-id="47faa-137">String</span></span>|<span data-ttu-id="47faa-138">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="47faa-138">User name.</span></span>|
|<span data-ttu-id="47faa-139">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="47faa-139">installedDeviceCount</span></span>|<span data-ttu-id="47faa-140">Int32</span><span class="sxs-lookup"><span data-stu-id="47faa-140">Int32</span></span>|<span data-ttu-id="47faa-141">Количество установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="47faa-141">Installed Device Count.</span></span>|
|<span data-ttu-id="47faa-142">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="47faa-142">failedDeviceCount</span></span>|<span data-ttu-id="47faa-143">Int32</span><span class="sxs-lookup"><span data-stu-id="47faa-143">Int32</span></span>|<span data-ttu-id="47faa-144">Количество устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="47faa-144">Failed Device Count.</span></span>|
|<span data-ttu-id="47faa-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="47faa-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="47faa-146">Int32</span><span class="sxs-lookup"><span data-stu-id="47faa-146">Int32</span></span>|<span data-ttu-id="47faa-147">Количество не установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="47faa-147">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="47faa-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="47faa-148">Response</span></span>
<span data-ttu-id="47faa-149">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="47faa-149">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47faa-150">Пример</span><span class="sxs-lookup"><span data-stu-id="47faa-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="47faa-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="47faa-151">Request</span></span>
<span data-ttu-id="47faa-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47faa-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
Content-type: application/json
Content-length: 189

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="47faa-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="47faa-153">Response</span></span>
<span data-ttu-id="47faa-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47faa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 238

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```




