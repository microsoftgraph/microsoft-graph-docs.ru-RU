---
title: Создание пользователя
description: Создание объекта user.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d5e3fe1d4b1b2dcf27de3915ffd49cd38ccb91d0
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732805"
---
# <a name="create-user"></a><span data-ttu-id="3e698-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="3e698-103">Create user</span></span>

<span data-ttu-id="3e698-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e698-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e698-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e698-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e698-106">Создание объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="3e698-106">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e698-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3e698-107">Prerequisites</span></span>
<span data-ttu-id="3e698-108">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="3e698-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3e698-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e698-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="3e698-110">Необходимое разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="3e698-110">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="3e698-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e698-111">Permission type</span></span>|<span data-ttu-id="3e698-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e698-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e698-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e698-113">Delegated (work or school account)</span></span>| <span data-ttu-id="3e698-114">_изменяется в зависимости от контекста_</span><span class="sxs-lookup"><span data-stu-id="3e698-114">_varies by context_</span></span> |
| <span data-ttu-id="3e698-115">&nbsp;&nbsp;Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="3e698-115">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="3e698-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e698-116">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="3e698-117">&nbsp;&nbsp;MAM</span><span class="sxs-lookup"><span data-stu-id="3e698-117">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="3e698-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e698-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="3e698-119">&nbsp;&nbsp;Onboarding</span><span class="sxs-lookup"><span data-stu-id="3e698-119">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="3e698-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e698-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="3e698-121">&nbsp;&nbsp;Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="3e698-121">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="3e698-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e698-122">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="3e698-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e698-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e698-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e698-124">Not supported.</span></span>|
|<span data-ttu-id="3e698-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e698-125">Application</span></span>|<span data-ttu-id="3e698-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e698-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e698-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e698-127">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="3e698-128">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3e698-128">Request headers</span></span>
|<span data-ttu-id="3e698-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e698-129">Header</span></span>|<span data-ttu-id="3e698-130">Значение</span><span class="sxs-lookup"><span data-stu-id="3e698-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e698-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e698-131">Authorization</span></span>|<span data-ttu-id="3e698-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e698-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e698-133">Accept</span><span class="sxs-lookup"><span data-stu-id="3e698-133">Accept</span></span>|<span data-ttu-id="3e698-134">application/json</span><span class="sxs-lookup"><span data-stu-id="3e698-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e698-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e698-135">Request body</span></span>
<span data-ttu-id="3e698-136">В теле запроса добавьте представление объекта user в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e698-136">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="3e698-137">В приведенной ниже таблице указаны свойства, необходимые при создании объекта user.</span><span class="sxs-lookup"><span data-stu-id="3e698-137">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="3e698-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e698-138">Property</span></span>|<span data-ttu-id="3e698-139">Тип</span><span class="sxs-lookup"><span data-stu-id="3e698-139">Type</span></span>|<span data-ttu-id="3e698-140">Описание</span><span class="sxs-lookup"><span data-stu-id="3e698-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e698-141">id</span><span class="sxs-lookup"><span data-stu-id="3e698-141">id</span></span>|<span data-ttu-id="3e698-142">String</span><span class="sxs-lookup"><span data-stu-id="3e698-142">String</span></span>|<span data-ttu-id="3e698-143">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="3e698-143">Unique identifier of the user.</span></span>|
|<span data-ttu-id="3e698-144">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="3e698-144">**Onboarding**</span></span>|
|<span data-ttu-id="3e698-145">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="3e698-145">deviceEnrollmentLimit</span></span>|<span data-ttu-id="3e698-146">Int32</span><span class="sxs-lookup"><span data-stu-id="3e698-146">Int32</span></span>|<span data-ttu-id="3e698-147">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="3e698-147">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="3e698-148">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="3e698-148">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="3e698-149">Поддержка свойств тела запроса зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="3e698-149">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="3e698-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e698-150">Response</span></span>
<span data-ttu-id="3e698-151">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3e698-151">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e698-152">Пример</span><span class="sxs-lookup"><span data-stu-id="3e698-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e698-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e698-153">Request</span></span>
<span data-ttu-id="3e698-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e698-154">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="3e698-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e698-155">Response</span></span>
<span data-ttu-id="3e698-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3e698-156">Here is an example of the response.</span></span> <span data-ttu-id="3e698-157">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="3e698-157">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3e698-158">Свойства, возвращенные при фактическом вызове, различаются в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="3e698-158">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```









