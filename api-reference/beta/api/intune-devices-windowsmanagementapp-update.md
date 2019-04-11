---
title: Обновление windowsManagementApp
description: Обновление свойств объекта windowsManagementApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f4eb4787113d6172ee3523c463191dff0948f75d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790195"
---
# <a name="update-windowsmanagementapp"></a><span data-ttu-id="bcf8b-103">Обновление windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="bcf8b-103">Update windowsManagementApp</span></span>

> <span data-ttu-id="bcf8b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcf8b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bcf8b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bcf8b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcf8b-106">Обновление свойств объекта [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="bcf8b-106">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bcf8b-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bcf8b-107">Prerequisites</span></span>
<span data-ttu-id="bcf8b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcf8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcf8b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcf8b-110">Permission type</span></span>|<span data-ttu-id="bcf8b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcf8b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bcf8b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcf8b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bcf8b-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcf8b-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bcf8b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcf8b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bcf8b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcf8b-115">Not supported.</span></span>|
|<span data-ttu-id="bcf8b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bcf8b-116">Application</span></span>|<span data-ttu-id="bcf8b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcf8b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bcf8b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcf8b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp
```

## <a name="request-headers"></a><span data-ttu-id="bcf8b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bcf8b-119">Request headers</span></span>
|<span data-ttu-id="bcf8b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bcf8b-120">Header</span></span>|<span data-ttu-id="bcf8b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bcf8b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bcf8b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bcf8b-122">Authorization</span></span>|<span data-ttu-id="bcf8b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bcf8b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bcf8b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bcf8b-124">Accept</span></span>|<span data-ttu-id="bcf8b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bcf8b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcf8b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bcf8b-126">Request body</span></span>
<span data-ttu-id="bcf8b-127">В тексте запроса добавьте представление объекта [WindowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bcf8b-127">In the request body, supply a JSON representation for the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

<span data-ttu-id="bcf8b-128">В следующей таблице приведены свойства, необходимые при создании [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span><span class="sxs-lookup"><span data-stu-id="bcf8b-128">The following table shows the properties that are required when you create the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span></span>

|<span data-ttu-id="bcf8b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bcf8b-129">Property</span></span>|<span data-ttu-id="bcf8b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bcf8b-130">Type</span></span>|<span data-ttu-id="bcf8b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bcf8b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcf8b-132">id</span><span class="sxs-lookup"><span data-stu-id="bcf8b-132">id</span></span>|<span data-ttu-id="bcf8b-133">String</span><span class="sxs-lookup"><span data-stu-id="bcf8b-133">String</span></span>|<span data-ttu-id="bcf8b-134">Уникальный идентификатор для приложения управления Windows</span><span class="sxs-lookup"><span data-stu-id="bcf8b-134">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="bcf8b-135">availableVersion</span><span class="sxs-lookup"><span data-stu-id="bcf8b-135">availableVersion</span></span>|<span data-ttu-id="bcf8b-136">String</span><span class="sxs-lookup"><span data-stu-id="bcf8b-136">String</span></span>|<span data-ttu-id="bcf8b-137">Доступная версия приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="bcf8b-137">Windows management app available version.</span></span>|



## <a name="response"></a><span data-ttu-id="bcf8b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcf8b-138">Response</span></span>
<span data-ttu-id="bcf8b-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bcf8b-139">If successful, this method returns a `200 OK` response code and an updated [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcf8b-140">Пример</span><span class="sxs-lookup"><span data-stu-id="bcf8b-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="bcf8b-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcf8b-141">Request</span></span>
<span data-ttu-id="bcf8b-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bcf8b-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp
Content-type: application/json
Content-length: 112

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "availableVersion": "Available Version value"
}
```

### <a name="response"></a><span data-ttu-id="bcf8b-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcf8b-143">Response</span></span>
<span data-ttu-id="bcf8b-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bcf8b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 161

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "5facc79c-c79c-5fac-9cc7-ac5f9cc7ac5f",
  "availableVersion": "Available Version value"
}
```





