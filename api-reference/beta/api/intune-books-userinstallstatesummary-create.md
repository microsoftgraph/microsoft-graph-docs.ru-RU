---
title: Создание объекта userInstallStateSummary
description: Создание объекта userInstallStateSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8dbae3b5271d271a9df1215382dbf08532fd1c22
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413006"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="5b5b7-103">Создание объекта userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="5b5b7-103">Create userInstallStateSummary</span></span>

> <span data-ttu-id="5b5b7-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5b5b7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5b5b7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b5b7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b5b7-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b5b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b5b7-107">Создание объекта [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="5b5b7-107">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b5b7-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5b5b7-108">Prerequisites</span></span>
<span data-ttu-id="5b5b7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5b5b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5b5b7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b5b7-111">Permission type</span></span>|<span data-ttu-id="5b5b7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b5b7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b5b7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b5b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b5b7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b5b7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5b5b7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b5b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b5b7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b5b7-116">Not supported.</span></span>|
|<span data-ttu-id="5b5b7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b5b7-117">Application</span></span>|<span data-ttu-id="5b5b7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b5b7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b5b7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b5b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="5b5b7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b5b7-120">Request headers</span></span>
|<span data-ttu-id="5b5b7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b5b7-121">Header</span></span>|<span data-ttu-id="5b5b7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5b5b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b5b7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b5b7-123">Authorization</span></span>|<span data-ttu-id="5b5b7-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5b5b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b5b7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5b5b7-125">Accept</span></span>|<span data-ttu-id="5b5b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5b5b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b5b7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b5b7-127">Request body</span></span>
<span data-ttu-id="5b5b7-128">В тексте запроса добавьте представление объекта userInstallStateSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b5b7-128">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="5b5b7-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта userInstallStateSummary.</span><span class="sxs-lookup"><span data-stu-id="5b5b7-129">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="5b5b7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b5b7-130">Property</span></span>|<span data-ttu-id="5b5b7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5b5b7-131">Type</span></span>|<span data-ttu-id="5b5b7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5b5b7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b5b7-133">id</span><span class="sxs-lookup"><span data-stu-id="5b5b7-133">id</span></span>|<span data-ttu-id="5b5b7-134">String</span><span class="sxs-lookup"><span data-stu-id="5b5b7-134">String</span></span>|<span data-ttu-id="5b5b7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5b5b7-135">Key of the entity.</span></span>|
|<span data-ttu-id="5b5b7-136">userName</span><span class="sxs-lookup"><span data-stu-id="5b5b7-136">userName</span></span>|<span data-ttu-id="5b5b7-137">String</span><span class="sxs-lookup"><span data-stu-id="5b5b7-137">String</span></span>|<span data-ttu-id="5b5b7-138">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="5b5b7-138">User name.</span></span>|
|<span data-ttu-id="5b5b7-139">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5b5b7-139">installedDeviceCount</span></span>|<span data-ttu-id="5b5b7-140">Int32</span><span class="sxs-lookup"><span data-stu-id="5b5b7-140">Int32</span></span>|<span data-ttu-id="5b5b7-141">Количество установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="5b5b7-141">Installed Device Count.</span></span>|
|<span data-ttu-id="5b5b7-142">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5b5b7-142">failedDeviceCount</span></span>|<span data-ttu-id="5b5b7-143">Int32</span><span class="sxs-lookup"><span data-stu-id="5b5b7-143">Int32</span></span>|<span data-ttu-id="5b5b7-144">Количество устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="5b5b7-144">Failed Device Count.</span></span>|
|<span data-ttu-id="5b5b7-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5b5b7-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="5b5b7-146">Int32</span><span class="sxs-lookup"><span data-stu-id="5b5b7-146">Int32</span></span>|<span data-ttu-id="5b5b7-147">Количество не установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="5b5b7-147">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="5b5b7-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b5b7-148">Response</span></span>
<span data-ttu-id="5b5b7-149">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5b5b7-149">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b5b7-150">Пример</span><span class="sxs-lookup"><span data-stu-id="5b5b7-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b5b7-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b5b7-151">Request</span></span>
<span data-ttu-id="5b5b7-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b5b7-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5b5b7-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b5b7-153">Response</span></span>
<span data-ttu-id="5b5b7-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5b5b7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




