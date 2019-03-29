---
title: Создание пользователя
description: Создание объекта user.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8f8cf0fb067c5a9cac80308f49fe07af122c1b47
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965321"
---
# <a name="create-user"></a><span data-ttu-id="73efb-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="73efb-103">Create user</span></span>

> <span data-ttu-id="73efb-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="73efb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="73efb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73efb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="73efb-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="73efb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73efb-107">Создание объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="73efb-107">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73efb-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="73efb-108">Prerequisites</span></span>

<span data-ttu-id="73efb-109">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="73efb-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="73efb-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73efb-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="73efb-111">Конкретное требуемое разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="73efb-111">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="73efb-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73efb-112">Permission type</span></span>|<span data-ttu-id="73efb-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="73efb-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73efb-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73efb-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="73efb-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="73efb-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="73efb-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73efb-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="73efb-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="73efb-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="73efb-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73efb-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="73efb-119">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="73efb-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="73efb-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73efb-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="73efb-121">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="73efb-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="73efb-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73efb-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="73efb-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73efb-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73efb-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73efb-124">Not supported.</span></span>|
|<span data-ttu-id="73efb-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73efb-125">Application</span></span>|<span data-ttu-id="73efb-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73efb-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73efb-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73efb-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="73efb-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73efb-128">Request headers</span></span>

|<span data-ttu-id="73efb-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73efb-129">Header</span></span>|<span data-ttu-id="73efb-130">Значение</span><span class="sxs-lookup"><span data-stu-id="73efb-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73efb-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73efb-131">Authorization</span></span>|<span data-ttu-id="73efb-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73efb-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73efb-133">Accept</span><span class="sxs-lookup"><span data-stu-id="73efb-133">Accept</span></span>|<span data-ttu-id="73efb-134">application/json</span><span class="sxs-lookup"><span data-stu-id="73efb-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73efb-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73efb-135">Request body</span></span>

<span data-ttu-id="73efb-136">В теле запроса добавьте представление объекта user в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73efb-136">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="73efb-137">В приведенной ниже таблице указаны свойства, необходимые при создании объекта user.</span><span class="sxs-lookup"><span data-stu-id="73efb-137">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="73efb-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="73efb-138">Property</span></span>|<span data-ttu-id="73efb-139">Тип</span><span class="sxs-lookup"><span data-stu-id="73efb-139">Type</span></span>|<span data-ttu-id="73efb-140">Описание</span><span class="sxs-lookup"><span data-stu-id="73efb-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73efb-141">id</span><span class="sxs-lookup"><span data-stu-id="73efb-141">id</span></span>|<span data-ttu-id="73efb-142">String</span><span class="sxs-lookup"><span data-stu-id="73efb-142">String</span></span>|<span data-ttu-id="73efb-143">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="73efb-143">Unique identifier of the user.</span></span>|
|<span data-ttu-id="73efb-144">**Встроенное подключение**</span><span class="sxs-lookup"><span data-stu-id="73efb-144">**On-boarding**</span></span>||
|<span data-ttu-id="73efb-145">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="73efb-145">deviceEnrollmentLimit</span></span>|<span data-ttu-id="73efb-146">Int32</span><span class="sxs-lookup"><span data-stu-id="73efb-146">Int32</span></span>|<span data-ttu-id="73efb-147">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="73efb-147">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="73efb-148">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="73efb-148">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="73efb-149">Поддержка свойств текста запроса зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="73efb-149">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="73efb-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="73efb-150">Response</span></span>

<span data-ttu-id="73efb-151">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="73efb-151">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73efb-152">Пример</span><span class="sxs-lookup"><span data-stu-id="73efb-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="73efb-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="73efb-153">Request</span></span>

<span data-ttu-id="73efb-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73efb-154">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="73efb-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="73efb-155">Response</span></span>

<span data-ttu-id="73efb-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="73efb-156">Here is an example of the response.</span></span> <span data-ttu-id="73efb-157">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="73efb-157">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="73efb-158">Свойства, возвращаемые при фактическом вызове, меняются в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="73efb-158">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



