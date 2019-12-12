---
title: Действие assign
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 69dba313a42d0610a9b9211cdbf9f930a18f117c
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39953693"
---
# <a name="assign-action"></a><span data-ttu-id="68587-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="68587-103">assign action</span></span>

> <span data-ttu-id="68587-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68587-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68587-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="68587-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68587-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="68587-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68587-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="68587-107">Prerequisites</span></span>
<span data-ttu-id="68587-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68587-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68587-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68587-110">Permission type</span></span>|<span data-ttu-id="68587-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="68587-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68587-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68587-112">Delegated (work or school account)</span></span>|<span data-ttu-id="68587-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68587-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="68587-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68587-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68587-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68587-115">Not supported.</span></span>|
|<span data-ttu-id="68587-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68587-116">Application</span></span>|<span data-ttu-id="68587-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68587-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="68587-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68587-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="68587-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="68587-119">Request headers</span></span>
|<span data-ttu-id="68587-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68587-120">Header</span></span>|<span data-ttu-id="68587-121">Значение</span><span class="sxs-lookup"><span data-stu-id="68587-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68587-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68587-122">Authorization</span></span>|<span data-ttu-id="68587-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68587-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68587-124">Accept</span><span class="sxs-lookup"><span data-stu-id="68587-124">Accept</span></span>|<span data-ttu-id="68587-125">application/json</span><span class="sxs-lookup"><span data-stu-id="68587-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68587-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="68587-126">Request body</span></span>
<span data-ttu-id="68587-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68587-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="68587-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="68587-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="68587-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="68587-129">Property</span></span>|<span data-ttu-id="68587-130">Тип</span><span class="sxs-lookup"><span data-stu-id="68587-130">Type</span></span>|<span data-ttu-id="68587-131">Описание</span><span class="sxs-lookup"><span data-stu-id="68587-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68587-132">assignments</span><span class="sxs-lookup"><span data-stu-id="68587-132">assignments</span></span>|<span data-ttu-id="68587-133">Коллекция [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="68587-133">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="68587-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="68587-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="68587-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="68587-135">Response</span></span>
<span data-ttu-id="68587-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="68587-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="68587-137">Пример</span><span class="sxs-lookup"><span data-stu-id="68587-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="68587-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="68587-138">Request</span></span>
<span data-ttu-id="68587-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68587-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assign

Content-type: application/json
Content-length: 293

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
      "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="68587-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="68587-140">Response</span></span>
<span data-ttu-id="68587-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68587-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





