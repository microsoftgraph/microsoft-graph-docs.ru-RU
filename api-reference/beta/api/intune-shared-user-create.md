---
title: Создание пользователя
description: Создание объекта user.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5c440d25e39dd9b97ed1e993476357dba3ca56a5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49223782"
---
# <a name="create-user"></a><span data-ttu-id="c89dd-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="c89dd-103">Create user</span></span>

<span data-ttu-id="c89dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c89dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c89dd-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c89dd-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c89dd-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c89dd-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c89dd-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c89dd-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c89dd-108">Создание объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="c89dd-108">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c89dd-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c89dd-109">Prerequisites</span></span>

<span data-ttu-id="c89dd-110">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="c89dd-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c89dd-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c89dd-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="c89dd-112">Конкретное требуемое разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="c89dd-112">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="c89dd-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c89dd-113">Permission type</span></span>|<span data-ttu-id="c89dd-114">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c89dd-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c89dd-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c89dd-115">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c89dd-116">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c89dd-116">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c89dd-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c89dd-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="c89dd-118">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="c89dd-118">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="c89dd-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c89dd-119">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="c89dd-120">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="c89dd-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c89dd-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c89dd-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="c89dd-122">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="c89dd-122">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="c89dd-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c89dd-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c89dd-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c89dd-124">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c89dd-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c89dd-125">Not supported.</span></span>|
|<span data-ttu-id="c89dd-126">Приложение</span><span class="sxs-lookup"><span data-stu-id="c89dd-126">Application</span></span>||
| <span data-ttu-id="c89dd-127">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c89dd-127">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c89dd-128">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c89dd-128">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="c89dd-129">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="c89dd-129">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="c89dd-130">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c89dd-130">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="c89dd-131">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="c89dd-131">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c89dd-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c89dd-132">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="c89dd-133">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="c89dd-133">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="c89dd-134">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c89dd-134">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c89dd-135">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c89dd-135">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="c89dd-136">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c89dd-136">Request headers</span></span>

|<span data-ttu-id="c89dd-137">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c89dd-137">Header</span></span>|<span data-ttu-id="c89dd-138">Значение</span><span class="sxs-lookup"><span data-stu-id="c89dd-138">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c89dd-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c89dd-139">Authorization</span></span>|<span data-ttu-id="c89dd-140">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c89dd-140">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c89dd-141">Accept</span><span class="sxs-lookup"><span data-stu-id="c89dd-141">Accept</span></span>|<span data-ttu-id="c89dd-142">application/json</span><span class="sxs-lookup"><span data-stu-id="c89dd-142">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c89dd-143">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c89dd-143">Request body</span></span>

<span data-ttu-id="c89dd-144">В теле запроса добавьте представление объекта user в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c89dd-144">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="c89dd-145">В приведенной ниже таблице указаны свойства, необходимые при создании объекта user.</span><span class="sxs-lookup"><span data-stu-id="c89dd-145">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="c89dd-146">Свойство</span><span class="sxs-lookup"><span data-stu-id="c89dd-146">Property</span></span>|<span data-ttu-id="c89dd-147">Тип</span><span class="sxs-lookup"><span data-stu-id="c89dd-147">Type</span></span>|<span data-ttu-id="c89dd-148">Описание</span><span class="sxs-lookup"><span data-stu-id="c89dd-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c89dd-149">id</span><span class="sxs-lookup"><span data-stu-id="c89dd-149">id</span></span>|<span data-ttu-id="c89dd-150">String</span><span class="sxs-lookup"><span data-stu-id="c89dd-150">String</span></span>|<span data-ttu-id="c89dd-151">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="c89dd-151">Unique identifier of the user.</span></span>|
|<span data-ttu-id="c89dd-152">**Встроенное подключение**</span><span class="sxs-lookup"><span data-stu-id="c89dd-152">**On-boarding**</span></span>||
|<span data-ttu-id="c89dd-153">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="c89dd-153">deviceEnrollmentLimit</span></span>|<span data-ttu-id="c89dd-154">Int32</span><span class="sxs-lookup"><span data-stu-id="c89dd-154">Int32</span></span>|<span data-ttu-id="c89dd-155">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="c89dd-155">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="c89dd-156">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="c89dd-156">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="c89dd-157">Поддержка свойств текста запроса зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="c89dd-157">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="c89dd-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="c89dd-158">Response</span></span>

<span data-ttu-id="c89dd-159">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c89dd-159">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c89dd-160">Пример</span><span class="sxs-lookup"><span data-stu-id="c89dd-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="c89dd-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="c89dd-161">Request</span></span>

<span data-ttu-id="c89dd-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c89dd-162">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="c89dd-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="c89dd-163">Response</span></span>

<span data-ttu-id="c89dd-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c89dd-164">Here is an example of the response.</span></span> <span data-ttu-id="c89dd-165">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="c89dd-165">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c89dd-166">Свойства, возвращаемые при фактическом вызове, меняются в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="c89dd-166">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```










