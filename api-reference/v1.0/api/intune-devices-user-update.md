---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 76695bd597afb69708f454e39439220c83091f39
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753430"
---
# <a name="update-user"></a><span data-ttu-id="2656f-103">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="2656f-103">Update user</span></span>

<span data-ttu-id="2656f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2656f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2656f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2656f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2656f-106">Обновление свойств объекта [user](../resources/intune-devices-user.md).</span><span class="sxs-lookup"><span data-stu-id="2656f-106">Update the properties of a [user](../resources/intune-devices-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2656f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2656f-107">Prerequisites</span></span>
<span data-ttu-id="2656f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2656f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2656f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2656f-110">Permission type</span></span>|<span data-ttu-id="2656f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2656f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2656f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2656f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2656f-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2656f-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2656f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2656f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2656f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2656f-115">Not supported.</span></span>|
|<span data-ttu-id="2656f-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="2656f-116">Application</span></span>|<span data-ttu-id="2656f-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2656f-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2656f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2656f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="2656f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2656f-119">Request headers</span></span>
|<span data-ttu-id="2656f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2656f-120">Header</span></span>|<span data-ttu-id="2656f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2656f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2656f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2656f-122">Authorization</span></span>|<span data-ttu-id="2656f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2656f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2656f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2656f-124">Accept</span></span>|<span data-ttu-id="2656f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2656f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2656f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2656f-126">Request body</span></span>
<span data-ttu-id="2656f-127">В теле запроса добавьте представление объекта [user](../resources/intune-devices-user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2656f-127">In the request body, supply a JSON representation for the [user](../resources/intune-devices-user.md) object.</span></span>

<span data-ttu-id="2656f-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [user](../resources/intune-devices-user.md).</span><span class="sxs-lookup"><span data-stu-id="2656f-128">The following table shows the properties that are required when you create the [user](../resources/intune-devices-user.md).</span></span>

|<span data-ttu-id="2656f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2656f-129">Property</span></span>|<span data-ttu-id="2656f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2656f-130">Type</span></span>|<span data-ttu-id="2656f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2656f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2656f-132">id</span><span class="sxs-lookup"><span data-stu-id="2656f-132">id</span></span>|<span data-ttu-id="2656f-133">String</span><span class="sxs-lookup"><span data-stu-id="2656f-133">String</span></span>|<span data-ttu-id="2656f-134">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="2656f-134">Unique identifier of the user.</span></span>|



## <a name="response"></a><span data-ttu-id="2656f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2656f-135">Response</span></span>
<span data-ttu-id="2656f-136">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [user](../resources/intune-devices-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2656f-136">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-devices-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2656f-137">Пример</span><span class="sxs-lookup"><span data-stu-id="2656f-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="2656f-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="2656f-138">Request</span></span>
<span data-ttu-id="2656f-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2656f-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="2656f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="2656f-140">Response</span></span>
<span data-ttu-id="2656f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2656f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```




