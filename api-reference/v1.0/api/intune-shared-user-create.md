---
title: Создание пользователя
description: Создание объекта user.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 343614306136f4962f6ac1955dbe2b1ad906279d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43411495"
---
# <a name="create-user"></a><span data-ttu-id="4b365-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="4b365-103">Create user</span></span>

<span data-ttu-id="4b365-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b365-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b365-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b365-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b365-106">Создание объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="4b365-106">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b365-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4b365-107">Prerequisites</span></span>
<span data-ttu-id="4b365-108">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="4b365-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="4b365-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b365-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="4b365-110">Конкретное требуемое разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="4b365-110">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="4b365-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b365-111">Permission type</span></span>|<span data-ttu-id="4b365-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b365-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b365-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b365-113">Delegated (work or school account)</span></span>| <span data-ttu-id="4b365-114">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="4b365-114">_varies by context_</span></span> |
| <span data-ttu-id="4b365-115">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="4b365-115">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="4b365-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b365-116">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="4b365-117">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="4b365-117">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="4b365-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b365-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="4b365-119">&nbsp;&nbsp; Входящая миграция</span><span class="sxs-lookup"><span data-stu-id="4b365-119">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="4b365-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b365-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4b365-121">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="4b365-121">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="4b365-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b365-122">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="4b365-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b365-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b365-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b365-124">Not supported.</span></span>|
|<span data-ttu-id="4b365-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b365-125">Application</span></span>|<span data-ttu-id="4b365-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b365-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b365-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b365-127">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="4b365-128">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4b365-128">Request headers</span></span>
|<span data-ttu-id="4b365-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b365-129">Header</span></span>|<span data-ttu-id="4b365-130">Значение</span><span class="sxs-lookup"><span data-stu-id="4b365-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b365-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b365-131">Authorization</span></span>|<span data-ttu-id="4b365-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b365-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b365-133">Accept</span><span class="sxs-lookup"><span data-stu-id="4b365-133">Accept</span></span>|<span data-ttu-id="4b365-134">application/json</span><span class="sxs-lookup"><span data-stu-id="4b365-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b365-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4b365-135">Request body</span></span>
<span data-ttu-id="4b365-136">В теле запроса добавьте представление объекта user в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b365-136">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="4b365-137">В приведенной ниже таблице указаны свойства, необходимые при создании объекта user.</span><span class="sxs-lookup"><span data-stu-id="4b365-137">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="4b365-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b365-138">Property</span></span>|<span data-ttu-id="4b365-139">Тип</span><span class="sxs-lookup"><span data-stu-id="4b365-139">Type</span></span>|<span data-ttu-id="4b365-140">Описание</span><span class="sxs-lookup"><span data-stu-id="4b365-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b365-141">id</span><span class="sxs-lookup"><span data-stu-id="4b365-141">id</span></span>|<span data-ttu-id="4b365-142">String</span><span class="sxs-lookup"><span data-stu-id="4b365-142">String</span></span>|<span data-ttu-id="4b365-143">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="4b365-143">Unique identifier of the user.</span></span>|
|<span data-ttu-id="4b365-144">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="4b365-144">**Onboarding**</span></span>|
|<span data-ttu-id="4b365-145">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="4b365-145">deviceEnrollmentLimit</span></span>|<span data-ttu-id="4b365-146">Int32</span><span class="sxs-lookup"><span data-stu-id="4b365-146">Int32</span></span>|<span data-ttu-id="4b365-147">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="4b365-147">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="4b365-148">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="4b365-148">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="4b365-149">Поддержка свойств текста запроса зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="4b365-149">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="4b365-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b365-150">Response</span></span>
<span data-ttu-id="4b365-151">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4b365-151">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b365-152">Пример</span><span class="sxs-lookup"><span data-stu-id="4b365-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b365-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b365-153">Request</span></span>
<span data-ttu-id="4b365-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b365-154">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="4b365-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b365-155">Response</span></span>
<span data-ttu-id="4b365-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4b365-156">Here is an example of the response.</span></span> <span data-ttu-id="4b365-157">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="4b365-157">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4b365-158">Свойства, возвращаемые при фактическом вызове, меняются в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="4b365-158">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```






