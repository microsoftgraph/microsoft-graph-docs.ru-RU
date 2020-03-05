---
title: Создание пользователя
description: Создание объекта user.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 915e043a7ed17549dd0d5a45b5bf4703dc0a6c46
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458093"
---
# <a name="create-user"></a><span data-ttu-id="c932a-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="c932a-103">Create user</span></span>

<span data-ttu-id="c932a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c932a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c932a-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c932a-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c932a-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c932a-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c932a-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c932a-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c932a-108">Создание объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="c932a-108">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c932a-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c932a-109">Prerequisites</span></span>

<span data-ttu-id="c932a-110">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="c932a-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c932a-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c932a-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="c932a-112">Конкретное требуемое разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="c932a-112">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="c932a-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c932a-113">Permission type</span></span>|<span data-ttu-id="c932a-114">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c932a-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c932a-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c932a-115">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c932a-116">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c932a-116">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c932a-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c932a-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="c932a-118">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="c932a-118">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="c932a-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c932a-119">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="c932a-120">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="c932a-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c932a-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c932a-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="c932a-122">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="c932a-122">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="c932a-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c932a-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c932a-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c932a-124">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c932a-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c932a-125">Not supported.</span></span>|
|<span data-ttu-id="c932a-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c932a-126">Application</span></span>||
| <span data-ttu-id="c932a-127">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c932a-127">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c932a-128">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c932a-128">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="c932a-129">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="c932a-129">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="c932a-130">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c932a-130">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="c932a-131">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="c932a-131">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c932a-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c932a-132">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="c932a-133">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="c932a-133">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="c932a-134">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c932a-134">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c932a-135">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c932a-135">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="c932a-136">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c932a-136">Request headers</span></span>

|<span data-ttu-id="c932a-137">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c932a-137">Header</span></span>|<span data-ttu-id="c932a-138">Значение</span><span class="sxs-lookup"><span data-stu-id="c932a-138">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c932a-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="c932a-139">Authorization</span></span>|<span data-ttu-id="c932a-140">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c932a-140">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c932a-141">Accept</span><span class="sxs-lookup"><span data-stu-id="c932a-141">Accept</span></span>|<span data-ttu-id="c932a-142">application/json</span><span class="sxs-lookup"><span data-stu-id="c932a-142">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c932a-143">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c932a-143">Request body</span></span>

<span data-ttu-id="c932a-144">В теле запроса добавьте представление объекта user в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c932a-144">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="c932a-145">В приведенной ниже таблице указаны свойства, необходимые при создании объекта user.</span><span class="sxs-lookup"><span data-stu-id="c932a-145">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="c932a-146">Свойство</span><span class="sxs-lookup"><span data-stu-id="c932a-146">Property</span></span>|<span data-ttu-id="c932a-147">Тип</span><span class="sxs-lookup"><span data-stu-id="c932a-147">Type</span></span>|<span data-ttu-id="c932a-148">Описание</span><span class="sxs-lookup"><span data-stu-id="c932a-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c932a-149">id</span><span class="sxs-lookup"><span data-stu-id="c932a-149">id</span></span>|<span data-ttu-id="c932a-150">String</span><span class="sxs-lookup"><span data-stu-id="c932a-150">String</span></span>|<span data-ttu-id="c932a-151">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="c932a-151">Unique identifier of the user.</span></span>|
|<span data-ttu-id="c932a-152">**Встроенное подключение**</span><span class="sxs-lookup"><span data-stu-id="c932a-152">**On-boarding**</span></span>||
|<span data-ttu-id="c932a-153">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="c932a-153">deviceEnrollmentLimit</span></span>|<span data-ttu-id="c932a-154">Int32</span><span class="sxs-lookup"><span data-stu-id="c932a-154">Int32</span></span>|<span data-ttu-id="c932a-155">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="c932a-155">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="c932a-156">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="c932a-156">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="c932a-157">Поддержка свойств текста запроса зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="c932a-157">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="c932a-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="c932a-158">Response</span></span>

<span data-ttu-id="c932a-159">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c932a-159">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c932a-160">Пример</span><span class="sxs-lookup"><span data-stu-id="c932a-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="c932a-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="c932a-161">Request</span></span>

<span data-ttu-id="c932a-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c932a-162">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="c932a-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="c932a-163">Response</span></span>

<span data-ttu-id="c932a-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c932a-164">Here is an example of the response.</span></span> <span data-ttu-id="c932a-165">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="c932a-165">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c932a-166">Свойства, возвращаемые при фактическом вызове, меняются в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="c932a-166">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```











