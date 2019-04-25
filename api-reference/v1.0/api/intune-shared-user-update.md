---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8fb82586ea0fda24297179963b730a097b2d81fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576649"
---
# <a name="update-user"></a><span data-ttu-id="1d7b7-103">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="1d7b7-103">Update user</span></span>

> <span data-ttu-id="1d7b7-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1d7b7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d7b7-105">Обновление свойств объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="1d7b7-105">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d7b7-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1d7b7-106">Prerequisites</span></span>
<span data-ttu-id="1d7b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d7b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d7b7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d7b7-109">Permission type</span></span>|<span data-ttu-id="1d7b7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d7b7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d7b7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d7b7-111">Delegated (work or school account)</span></span>| <span data-ttu-id="1d7b7-112">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="1d7b7-112">_varies by context_</span></span>|
| <span data-ttu-id="1d7b7-113">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="1d7b7-113">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="1d7b7-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d7b7-114">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="1d7b7-115">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="1d7b7-115">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="1d7b7-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d7b7-116">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="1d7b7-117">&nbsp;&nbsp; Входящая миграция</span><span class="sxs-lookup"><span data-stu-id="1d7b7-117">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="1d7b7-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d7b7-118">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="1d7b7-119">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="1d7b7-119">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="1d7b7-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d7b7-120">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="1d7b7-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d7b7-121">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d7b7-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d7b7-122">Not supported.</span></span>|
|<span data-ttu-id="1d7b7-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d7b7-123">Application</span></span>|<span data-ttu-id="1d7b7-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d7b7-124">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d7b7-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d7b7-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="1d7b7-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d7b7-126">Request headers</span></span>
|<span data-ttu-id="1d7b7-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1d7b7-127">Header</span></span>|<span data-ttu-id="1d7b7-128">Значение</span><span class="sxs-lookup"><span data-stu-id="1d7b7-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d7b7-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1d7b7-129">Authorization</span></span>|<span data-ttu-id="1d7b7-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d7b7-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d7b7-131">Accept</span><span class="sxs-lookup"><span data-stu-id="1d7b7-131">Accept</span></span>|<span data-ttu-id="1d7b7-132">application/json</span><span class="sxs-lookup"><span data-stu-id="1d7b7-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d7b7-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1d7b7-133">Request body</span></span>
<span data-ttu-id="1d7b7-134">В теле запроса добавьте представление объекта [user](../resources/intune-shared-user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d7b7-134">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="1d7b7-135">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="1d7b7-135">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="1d7b7-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d7b7-136">Property</span></span>|<span data-ttu-id="1d7b7-137">Тип</span><span class="sxs-lookup"><span data-stu-id="1d7b7-137">Type</span></span>|<span data-ttu-id="1d7b7-138">Описание</span><span class="sxs-lookup"><span data-stu-id="1d7b7-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d7b7-139">id</span><span class="sxs-lookup"><span data-stu-id="1d7b7-139">id</span></span>|<span data-ttu-id="1d7b7-140">String</span><span class="sxs-lookup"><span data-stu-id="1d7b7-140">String</span></span>|<span data-ttu-id="1d7b7-141">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="1d7b7-141">Unique identifier of the user.</span></span>|
|<span data-ttu-id="1d7b7-142">**Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="1d7b7-142">**Onboarding**</span></span>|
|<span data-ttu-id="1d7b7-143">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="1d7b7-143">deviceEnrollmentLimit</span></span>|<span data-ttu-id="1d7b7-144">Int32</span><span class="sxs-lookup"><span data-stu-id="1d7b7-144">Int32</span></span>|<span data-ttu-id="1d7b7-145">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="1d7b7-145">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="1d7b7-146">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="1d7b7-146">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="1d7b7-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d7b7-147">Response</span></span>
<span data-ttu-id="1d7b7-148">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1d7b7-148">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d7b7-149">Пример</span><span class="sxs-lookup"><span data-stu-id="1d7b7-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d7b7-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d7b7-150">Request</span></span>
<span data-ttu-id="1d7b7-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d7b7-151">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="1d7b7-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d7b7-152">Response</span></span>
<span data-ttu-id="1d7b7-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1d7b7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



