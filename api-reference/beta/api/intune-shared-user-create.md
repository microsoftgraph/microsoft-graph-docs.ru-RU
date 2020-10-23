---
title: Создание пользователя
description: Создание объекта user.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: df2e10d163f415f5f36ff56cafbf0407445d2eb7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728650"
---
# <a name="create-user"></a><span data-ttu-id="c9e16-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="c9e16-103">Create user</span></span>

<span data-ttu-id="c9e16-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9e16-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c9e16-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c9e16-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c9e16-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9e16-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9e16-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c9e16-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9e16-108">Создание объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="c9e16-108">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9e16-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c9e16-109">Prerequisites</span></span>

<span data-ttu-id="c9e16-110">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="c9e16-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c9e16-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9e16-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="c9e16-112">Конкретное требуемое разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="c9e16-112">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="c9e16-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9e16-113">Permission type</span></span>|<span data-ttu-id="c9e16-114">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9e16-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9e16-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9e16-115">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c9e16-116">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c9e16-116">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c9e16-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9e16-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="c9e16-118">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="c9e16-118">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="c9e16-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9e16-119">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="c9e16-120">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="c9e16-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c9e16-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9e16-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="c9e16-122">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="c9e16-122">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="c9e16-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9e16-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c9e16-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9e16-124">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9e16-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9e16-125">Not supported.</span></span>|
|<span data-ttu-id="c9e16-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9e16-126">Application</span></span>||
| <span data-ttu-id="c9e16-127">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c9e16-127">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c9e16-128">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9e16-128">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="c9e16-129">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="c9e16-129">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="c9e16-130">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9e16-130">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="c9e16-131">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="c9e16-131">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c9e16-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9e16-132">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="c9e16-133">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="c9e16-133">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="c9e16-134">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9e16-134">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9e16-135">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9e16-135">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="c9e16-136">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c9e16-136">Request headers</span></span>

|<span data-ttu-id="c9e16-137">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9e16-137">Header</span></span>|<span data-ttu-id="c9e16-138">Значение</span><span class="sxs-lookup"><span data-stu-id="c9e16-138">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9e16-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9e16-139">Authorization</span></span>|<span data-ttu-id="c9e16-140">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9e16-140">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9e16-141">Accept</span><span class="sxs-lookup"><span data-stu-id="c9e16-141">Accept</span></span>|<span data-ttu-id="c9e16-142">application/json</span><span class="sxs-lookup"><span data-stu-id="c9e16-142">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9e16-143">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c9e16-143">Request body</span></span>

<span data-ttu-id="c9e16-144">В теле запроса добавьте представление объекта user в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9e16-144">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="c9e16-145">В приведенной ниже таблице указаны свойства, необходимые при создании объекта user.</span><span class="sxs-lookup"><span data-stu-id="c9e16-145">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="c9e16-146">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9e16-146">Property</span></span>|<span data-ttu-id="c9e16-147">Тип</span><span class="sxs-lookup"><span data-stu-id="c9e16-147">Type</span></span>|<span data-ttu-id="c9e16-148">Описание</span><span class="sxs-lookup"><span data-stu-id="c9e16-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9e16-149">id</span><span class="sxs-lookup"><span data-stu-id="c9e16-149">id</span></span>|<span data-ttu-id="c9e16-150">Строка</span><span class="sxs-lookup"><span data-stu-id="c9e16-150">String</span></span>|<span data-ttu-id="c9e16-151">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="c9e16-151">Unique identifier of the user.</span></span>|
|<span data-ttu-id="c9e16-152">**Встроенное подключение**</span><span class="sxs-lookup"><span data-stu-id="c9e16-152">**On-boarding**</span></span>||
|<span data-ttu-id="c9e16-153">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="c9e16-153">deviceEnrollmentLimit</span></span>|<span data-ttu-id="c9e16-154">Int32</span><span class="sxs-lookup"><span data-stu-id="c9e16-154">Int32</span></span>|<span data-ttu-id="c9e16-155">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="c9e16-155">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="c9e16-156">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="c9e16-156">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="c9e16-157">Поддержка свойств текста запроса зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="c9e16-157">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="c9e16-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9e16-158">Response</span></span>

<span data-ttu-id="c9e16-159">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c9e16-159">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9e16-160">Пример</span><span class="sxs-lookup"><span data-stu-id="c9e16-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9e16-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9e16-161">Request</span></span>

<span data-ttu-id="c9e16-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9e16-162">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="c9e16-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9e16-163">Response</span></span>

<span data-ttu-id="c9e16-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c9e16-164">Here is an example of the response.</span></span> <span data-ttu-id="c9e16-165">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="c9e16-165">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c9e16-166">Свойства, возвращаемые при фактическом вызове, меняются в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="c9e16-166">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```











