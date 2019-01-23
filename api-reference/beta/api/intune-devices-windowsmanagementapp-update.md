---
title: Обновление windowsManagementApp
description: Обновление свойства объекта windowsManagementApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 27ba9154598480972e1d7f2c9a8b5d28bb3ec4b2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412410"
---
# <a name="update-windowsmanagementapp"></a><span data-ttu-id="9baf1-103">Обновление windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="9baf1-103">Update windowsManagementApp</span></span>

> <span data-ttu-id="9baf1-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9baf1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9baf1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9baf1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9baf1-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9baf1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9baf1-107">Обновление свойства объекта [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="9baf1-107">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9baf1-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="9baf1-108">Prerequisites</span></span>
<span data-ttu-id="9baf1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9baf1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9baf1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9baf1-111">Permission type</span></span>|<span data-ttu-id="9baf1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9baf1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9baf1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9baf1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9baf1-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9baf1-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9baf1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9baf1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9baf1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9baf1-116">Not supported.</span></span>|
|<span data-ttu-id="9baf1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9baf1-117">Application</span></span>|<span data-ttu-id="9baf1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9baf1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9baf1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9baf1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp
```

## <a name="request-headers"></a><span data-ttu-id="9baf1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9baf1-120">Request headers</span></span>
|<span data-ttu-id="9baf1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9baf1-121">Header</span></span>|<span data-ttu-id="9baf1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9baf1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9baf1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9baf1-123">Authorization</span></span>|<span data-ttu-id="9baf1-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9baf1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9baf1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9baf1-125">Accept</span></span>|<span data-ttu-id="9baf1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9baf1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9baf1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9baf1-127">Request body</span></span>
<span data-ttu-id="9baf1-128">В тексте запроса укажите представление JSON для объекта [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="9baf1-128">In the request body, supply a JSON representation for the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

<span data-ttu-id="9baf1-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span><span class="sxs-lookup"><span data-stu-id="9baf1-129">The following table shows the properties that are required when you create the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span></span>

|<span data-ttu-id="9baf1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9baf1-130">Property</span></span>|<span data-ttu-id="9baf1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9baf1-131">Type</span></span>|<span data-ttu-id="9baf1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9baf1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9baf1-133">id</span><span class="sxs-lookup"><span data-stu-id="9baf1-133">id</span></span>|<span data-ttu-id="9baf1-134">String</span><span class="sxs-lookup"><span data-stu-id="9baf1-134">String</span></span>|<span data-ttu-id="9baf1-135">Уникальный идентификатор для приложения управления Windows</span><span class="sxs-lookup"><span data-stu-id="9baf1-135">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="9baf1-136">availableVersion</span><span class="sxs-lookup"><span data-stu-id="9baf1-136">availableVersion</span></span>|<span data-ttu-id="9baf1-137">String</span><span class="sxs-lookup"><span data-stu-id="9baf1-137">String</span></span>|<span data-ttu-id="9baf1-138">Управление приложения доступные версии Windows.</span><span class="sxs-lookup"><span data-stu-id="9baf1-138">Windows management app available version.</span></span>|



## <a name="response"></a><span data-ttu-id="9baf1-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="9baf1-139">Response</span></span>
<span data-ttu-id="9baf1-140">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9baf1-140">If successful, this method returns a `200 OK` response code and an updated [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9baf1-141">Пример</span><span class="sxs-lookup"><span data-stu-id="9baf1-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="9baf1-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="9baf1-142">Request</span></span>
<span data-ttu-id="9baf1-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9baf1-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp
Content-type: application/json
Content-length: 112

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "availableVersion": "Available Version value"
}
```

### <a name="response"></a><span data-ttu-id="9baf1-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="9baf1-144">Response</span></span>
<span data-ttu-id="9baf1-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9baf1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




