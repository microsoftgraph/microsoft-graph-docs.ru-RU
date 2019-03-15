---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0009e563e34d40e8dae434761ed4203564ce9d9b
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571986"
---
# <a name="update-user"></a><span data-ttu-id="3f455-103">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="3f455-103">Update user</span></span>

> <span data-ttu-id="3f455-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3f455-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3f455-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f455-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3f455-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3f455-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f455-107">Обновление свойств объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="3f455-107">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f455-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3f455-108">Prerequisites</span></span>

<span data-ttu-id="3f455-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3f455-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3f455-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f455-111">Permission type</span></span>|<span data-ttu-id="3f455-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f455-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f455-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f455-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3f455-114">&nbsp; &nbsp; **Управление устройством**</span><span class="sxs-lookup"><span data-stu-id="3f455-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="3f455-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f455-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="3f455-116">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="3f455-116">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="3f455-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f455-117">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="3f455-118">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="3f455-118">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="3f455-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f455-119">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="3f455-120">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="3f455-120">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="3f455-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f455-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3f455-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f455-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f455-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f455-123">Not supported.</span></span>|
|<span data-ttu-id="3f455-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3f455-124">Application</span></span>|<span data-ttu-id="3f455-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f455-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f455-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f455-126">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="3f455-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3f455-127">Request headers</span></span>

|<span data-ttu-id="3f455-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3f455-128">Header</span></span>|<span data-ttu-id="3f455-129">Значение</span><span class="sxs-lookup"><span data-stu-id="3f455-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f455-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3f455-130">Authorization</span></span>|<span data-ttu-id="3f455-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f455-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f455-132">Accept</span><span class="sxs-lookup"><span data-stu-id="3f455-132">Accept</span></span>|<span data-ttu-id="3f455-133">application/json</span><span class="sxs-lookup"><span data-stu-id="3f455-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f455-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3f455-134">Request body</span></span>

<span data-ttu-id="3f455-135">В теле запроса добавьте представление объекта [user](../resources/intune-shared-user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f455-135">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="3f455-136">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="3f455-136">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="3f455-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f455-137">Property</span></span>|<span data-ttu-id="3f455-138">Тип</span><span class="sxs-lookup"><span data-stu-id="3f455-138">Type</span></span>|<span data-ttu-id="3f455-139">Описание</span><span class="sxs-lookup"><span data-stu-id="3f455-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f455-140">id</span><span class="sxs-lookup"><span data-stu-id="3f455-140">id</span></span>|<span data-ttu-id="3f455-141">Строка</span><span class="sxs-lookup"><span data-stu-id="3f455-141">String</span></span>|<span data-ttu-id="3f455-142">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="3f455-142">Unique identifier of the user.</span></span>|
|<span data-ttu-id="3f455-143">**Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="3f455-143">**Onboarding**</span></span>|
|<span data-ttu-id="3f455-144">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="3f455-144">deviceEnrollmentLimit</span></span>|<span data-ttu-id="3f455-145">Int32</span><span class="sxs-lookup"><span data-stu-id="3f455-145">Int32</span></span>|<span data-ttu-id="3f455-146">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="3f455-146">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="3f455-147">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="3f455-147">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="3f455-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f455-148">Response</span></span>

<span data-ttu-id="3f455-149">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3f455-149">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f455-150">Пример</span><span class="sxs-lookup"><span data-stu-id="3f455-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f455-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f455-151">Request</span></span>

<span data-ttu-id="3f455-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f455-152">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="3f455-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f455-153">Response</span></span>

<span data-ttu-id="3f455-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3f455-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



