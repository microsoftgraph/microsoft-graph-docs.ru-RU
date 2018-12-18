---
title: Создание importedWindowsAutopilotDeviceIdentityUpload
description: Создание нового объекта importedWindowsAutopilotDeviceIdentityUpload.
author: tfitzmac
ms.openlocfilehash: f4042129f33b617546e32d46435179af5c9d3282
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354812"
---
# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="b6829-103">Создание importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="b6829-103">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="b6829-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b6829-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6829-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6829-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6829-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b6829-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6829-107">Создание нового объекта [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="b6829-107">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b6829-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b6829-108">Prerequisites</span></span>
<span data-ttu-id="b6829-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6829-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6829-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6829-111">Permission type</span></span>|<span data-ttu-id="b6829-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6829-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6829-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6829-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6829-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6829-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b6829-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6829-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6829-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6829-116">Not supported.</span></span>|
|<span data-ttu-id="b6829-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6829-117">Application</span></span>|<span data-ttu-id="b6829-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6829-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6829-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6829-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="b6829-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b6829-120">Request headers</span></span>
|<span data-ttu-id="b6829-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b6829-121">Header</span></span>|<span data-ttu-id="b6829-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b6829-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6829-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b6829-123">Authorization</span></span>|<span data-ttu-id="b6829-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b6829-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6829-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b6829-125">Accept</span></span>|<span data-ttu-id="b6829-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6829-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6829-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6829-127">Request body</span></span>
<span data-ttu-id="b6829-128">В тексте запроса укажите представление JSON для объекта importedWindowsAutopilotDeviceIdentityUpload.</span><span class="sxs-lookup"><span data-stu-id="b6829-128">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentityUpload object.</span></span>

<span data-ttu-id="b6829-129">В следующей таблице показаны свойства, которые необходимы для создания importedWindowsAutopilotDeviceIdentityUpload.</span><span class="sxs-lookup"><span data-stu-id="b6829-129">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentityUpload.</span></span>

|<span data-ttu-id="b6829-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6829-130">Property</span></span>|<span data-ttu-id="b6829-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b6829-131">Type</span></span>|<span data-ttu-id="b6829-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b6829-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6829-133">id</span><span class="sxs-lookup"><span data-stu-id="b6829-133">id</span></span>|<span data-ttu-id="b6829-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b6829-134">String</span></span>|<span data-ttu-id="b6829-135">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="b6829-135">The GUID for the object</span></span>|
|<span data-ttu-id="b6829-136">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="b6829-136">createdDateTimeUtc</span></span>|<span data-ttu-id="b6829-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6829-137">DateTimeOffset</span></span>|<span data-ttu-id="b6829-138">Дата и время при создании сущности.</span><span class="sxs-lookup"><span data-stu-id="b6829-138">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="b6829-139">status</span><span class="sxs-lookup"><span data-stu-id="b6829-139">status</span></span>|[<span data-ttu-id="b6829-140">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="b6829-140">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="b6829-141">Отправьте состояние.</span><span class="sxs-lookup"><span data-stu-id="b6829-141">Upload status.</span></span> <span data-ttu-id="b6829-142">Возможные значения: `noUpload`, `pending`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="b6829-142">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="b6829-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6829-143">Response</span></span>
<span data-ttu-id="b6829-144">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b6829-144">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6829-145">Пример</span><span class="sxs-lookup"><span data-stu-id="b6829-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="b6829-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6829-146">Request</span></span>
<span data-ttu-id="b6829-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6829-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="b6829-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="b6829-148">Response</span></span>
<span data-ttu-id="b6829-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b6829-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "8d639524-9524-8d63-2495-638d2495638d",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```





