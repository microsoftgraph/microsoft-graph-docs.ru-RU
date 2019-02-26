---
title: Действие assign
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: feb9e93247d26fedd21454d696f4566eeef4e8d0
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255467"
---
# <a name="assign-action"></a><span data-ttu-id="32146-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="32146-103">assign action</span></span>

> <span data-ttu-id="32146-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32146-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32146-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="32146-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32146-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="32146-106">Prerequisites</span></span>
<span data-ttu-id="32146-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="32146-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="32146-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32146-109">Permission type</span></span>|<span data-ttu-id="32146-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="32146-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32146-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32146-111">Delegated (work or school account)</span></span>|<span data-ttu-id="32146-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32146-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="32146-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32146-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32146-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32146-114">Not supported.</span></span>|
|<span data-ttu-id="32146-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32146-115">Application</span></span>|<span data-ttu-id="32146-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32146-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32146-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32146-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="32146-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32146-118">Request headers</span></span>
|<span data-ttu-id="32146-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="32146-119">Header</span></span>|<span data-ttu-id="32146-120">Значение</span><span class="sxs-lookup"><span data-stu-id="32146-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32146-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="32146-121">Authorization</span></span>|<span data-ttu-id="32146-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="32146-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32146-123">Accept</span><span class="sxs-lookup"><span data-stu-id="32146-123">Accept</span></span>|<span data-ttu-id="32146-124">application/json</span><span class="sxs-lookup"><span data-stu-id="32146-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32146-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="32146-125">Request body</span></span>
<span data-ttu-id="32146-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32146-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="32146-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="32146-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="32146-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="32146-128">Property</span></span>|<span data-ttu-id="32146-129">Тип</span><span class="sxs-lookup"><span data-stu-id="32146-129">Type</span></span>|<span data-ttu-id="32146-130">Описание</span><span class="sxs-lookup"><span data-stu-id="32146-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32146-131">assignments</span><span class="sxs-lookup"><span data-stu-id="32146-131">assignments</span></span>|<span data-ttu-id="32146-132">Коллекция [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="32146-132">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="32146-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="32146-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="32146-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="32146-134">Response</span></span>
<span data-ttu-id="32146-135">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="32146-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="32146-136">Пример</span><span class="sxs-lookup"><span data-stu-id="32146-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="32146-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="32146-137">Request</span></span>
<span data-ttu-id="32146-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32146-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assign

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

### <a name="response"></a><span data-ttu-id="32146-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="32146-139">Response</span></span>
<span data-ttu-id="32146-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="32146-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



