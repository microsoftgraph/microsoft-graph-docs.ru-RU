---
title: Создание объекта userInstallStateSummary
description: Создание объекта userInstallStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39313dc5fc67f26d4e81e3c759fa65aff108a3dd
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986217"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="a5de7-103">Создание объекта userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="a5de7-103">Create userInstallStateSummary</span></span>

> <span data-ttu-id="a5de7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5de7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5de7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a5de7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5de7-106">Создание объекта [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a5de7-106">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5de7-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a5de7-107">Prerequisites</span></span>
<span data-ttu-id="a5de7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5de7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5de7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5de7-110">Permission type</span></span>|<span data-ttu-id="a5de7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5de7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5de7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5de7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a5de7-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5de7-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a5de7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5de7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5de7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5de7-115">Not supported.</span></span>|
|<span data-ttu-id="a5de7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5de7-116">Application</span></span>|<span data-ttu-id="a5de7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5de7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5de7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5de7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="a5de7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5de7-119">Request headers</span></span>
|<span data-ttu-id="a5de7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a5de7-120">Header</span></span>|<span data-ttu-id="a5de7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a5de7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5de7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5de7-122">Authorization</span></span>|<span data-ttu-id="a5de7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5de7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5de7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a5de7-124">Accept</span></span>|<span data-ttu-id="a5de7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a5de7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5de7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a5de7-126">Request body</span></span>
<span data-ttu-id="a5de7-127">В тексте запроса добавьте представление объекта userInstallStateSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5de7-127">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="a5de7-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта userInstallStateSummary.</span><span class="sxs-lookup"><span data-stu-id="a5de7-128">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="a5de7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5de7-129">Property</span></span>|<span data-ttu-id="a5de7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a5de7-130">Type</span></span>|<span data-ttu-id="a5de7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a5de7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5de7-132">id</span><span class="sxs-lookup"><span data-stu-id="a5de7-132">id</span></span>|<span data-ttu-id="a5de7-133">String</span><span class="sxs-lookup"><span data-stu-id="a5de7-133">String</span></span>|<span data-ttu-id="a5de7-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a5de7-134">Key of the entity.</span></span>|
|<span data-ttu-id="a5de7-135">userName</span><span class="sxs-lookup"><span data-stu-id="a5de7-135">userName</span></span>|<span data-ttu-id="a5de7-136">String</span><span class="sxs-lookup"><span data-stu-id="a5de7-136">String</span></span>|<span data-ttu-id="a5de7-137">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="a5de7-137">User name.</span></span>|
|<span data-ttu-id="a5de7-138">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a5de7-138">installedDeviceCount</span></span>|<span data-ttu-id="a5de7-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a5de7-139">Int32</span></span>|<span data-ttu-id="a5de7-140">Количество установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="a5de7-140">Installed Device Count.</span></span>|
|<span data-ttu-id="a5de7-141">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a5de7-141">failedDeviceCount</span></span>|<span data-ttu-id="a5de7-142">Int32</span><span class="sxs-lookup"><span data-stu-id="a5de7-142">Int32</span></span>|<span data-ttu-id="a5de7-143">Количество устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="a5de7-143">Failed Device Count.</span></span>|
|<span data-ttu-id="a5de7-144">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a5de7-144">notInstalledDeviceCount</span></span>|<span data-ttu-id="a5de7-145">Int32</span><span class="sxs-lookup"><span data-stu-id="a5de7-145">Int32</span></span>|<span data-ttu-id="a5de7-146">Количество не установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="a5de7-146">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="a5de7-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5de7-147">Response</span></span>
<span data-ttu-id="a5de7-148">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a5de7-148">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5de7-149">Пример</span><span class="sxs-lookup"><span data-stu-id="a5de7-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5de7-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5de7-150">Request</span></span>
<span data-ttu-id="a5de7-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5de7-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a5de7-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5de7-152">Response</span></span>
<span data-ttu-id="a5de7-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a5de7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




