---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f52e49c86e0e333fbf4f8c52b71c2850c73bc533
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861945"
---
# <a name="update-user"></a><span data-ttu-id="0bf21-103">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="0bf21-103">Update user</span></span>

> <span data-ttu-id="0bf21-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0bf21-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0bf21-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bf21-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0bf21-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0bf21-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0bf21-107">Обновление свойств объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="0bf21-107">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0bf21-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0bf21-108">Prerequisites</span></span>

<span data-ttu-id="0bf21-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bf21-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bf21-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0bf21-111">Permission type</span></span>|<span data-ttu-id="0bf21-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0bf21-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bf21-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0bf21-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0bf21-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="0bf21-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="0bf21-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bf21-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="0bf21-116">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="0bf21-116">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="0bf21-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bf21-117">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="0bf21-118">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="0bf21-118">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="0bf21-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bf21-119">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="0bf21-120">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="0bf21-120">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="0bf21-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bf21-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0bf21-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0bf21-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bf21-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bf21-123">Not supported.</span></span>|
|<span data-ttu-id="0bf21-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0bf21-124">Application</span></span>|<span data-ttu-id="0bf21-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bf21-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bf21-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0bf21-126">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="0bf21-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0bf21-127">Request headers</span></span>

|<span data-ttu-id="0bf21-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0bf21-128">Header</span></span>|<span data-ttu-id="0bf21-129">Значение</span><span class="sxs-lookup"><span data-stu-id="0bf21-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bf21-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bf21-130">Authorization</span></span>|<span data-ttu-id="0bf21-131">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0bf21-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bf21-132">Accept</span><span class="sxs-lookup"><span data-stu-id="0bf21-132">Accept</span></span>|<span data-ttu-id="0bf21-133">application/json</span><span class="sxs-lookup"><span data-stu-id="0bf21-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bf21-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0bf21-134">Request body</span></span>

<span data-ttu-id="0bf21-135">В теле запроса добавьте представление объекта [user](../resources/intune-shared-user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0bf21-135">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="0bf21-136">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="0bf21-136">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="0bf21-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="0bf21-137">Property</span></span>|<span data-ttu-id="0bf21-138">Тип</span><span class="sxs-lookup"><span data-stu-id="0bf21-138">Type</span></span>|<span data-ttu-id="0bf21-139">Описание</span><span class="sxs-lookup"><span data-stu-id="0bf21-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bf21-140">id</span><span class="sxs-lookup"><span data-stu-id="0bf21-140">id</span></span>|<span data-ttu-id="0bf21-141">String</span><span class="sxs-lookup"><span data-stu-id="0bf21-141">String</span></span>|<span data-ttu-id="0bf21-142">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="0bf21-142">Unique identifier of the user.</span></span>|
|<span data-ttu-id="0bf21-143">**Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="0bf21-143">**Onboarding**</span></span>|
|<span data-ttu-id="0bf21-144">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="0bf21-144">deviceEnrollmentLimit</span></span>|<span data-ttu-id="0bf21-145">Int32</span><span class="sxs-lookup"><span data-stu-id="0bf21-145">Int32</span></span>|<span data-ttu-id="0bf21-146">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="0bf21-146">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="0bf21-147">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="0bf21-147">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="0bf21-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bf21-148">Response</span></span>

<span data-ttu-id="0bf21-149">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0bf21-149">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bf21-150">Пример</span><span class="sxs-lookup"><span data-stu-id="0bf21-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="0bf21-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bf21-151">Request</span></span>

<span data-ttu-id="0bf21-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0bf21-152">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="0bf21-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="0bf21-153">Response</span></span>

<span data-ttu-id="0bf21-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0bf21-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



