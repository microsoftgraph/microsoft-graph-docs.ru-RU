---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 161e76abb31c4ee569cebfa5b8e33966abcc6e25
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760638"
---
# <a name="assign-action"></a><span data-ttu-id="4dc6e-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="4dc6e-103">assign action</span></span>

<span data-ttu-id="4dc6e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4dc6e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4dc6e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4dc6e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4dc6e-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4dc6e-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4dc6e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4dc6e-107">Prerequisites</span></span>
<span data-ttu-id="4dc6e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4dc6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dc6e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4dc6e-110">Permission type</span></span>|<span data-ttu-id="4dc6e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4dc6e-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4dc6e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4dc6e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4dc6e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dc6e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4dc6e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4dc6e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4dc6e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dc6e-115">Not supported.</span></span>|
|<span data-ttu-id="4dc6e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="4dc6e-116">Application</span></span>|<span data-ttu-id="4dc6e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dc6e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4dc6e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4dc6e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="4dc6e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4dc6e-119">Request headers</span></span>
|<span data-ttu-id="4dc6e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4dc6e-120">Header</span></span>|<span data-ttu-id="4dc6e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4dc6e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4dc6e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4dc6e-122">Authorization</span></span>|<span data-ttu-id="4dc6e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4dc6e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4dc6e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4dc6e-124">Accept</span></span>|<span data-ttu-id="4dc6e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4dc6e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4dc6e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4dc6e-126">Request body</span></span>
<span data-ttu-id="4dc6e-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4dc6e-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4dc6e-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="4dc6e-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4dc6e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4dc6e-129">Property</span></span>|<span data-ttu-id="4dc6e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4dc6e-130">Type</span></span>|<span data-ttu-id="4dc6e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4dc6e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dc6e-132">assignments</span><span class="sxs-lookup"><span data-stu-id="4dc6e-132">assignments</span></span>|<span data-ttu-id="4dc6e-133">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4dc6e-133">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="4dc6e-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4dc6e-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4dc6e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4dc6e-135">Response</span></span>
<span data-ttu-id="4dc6e-136">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4dc6e-136">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4dc6e-137">Пример</span><span class="sxs-lookup"><span data-stu-id="4dc6e-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="4dc6e-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="4dc6e-138">Request</span></span>
<span data-ttu-id="4dc6e-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4dc6e-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign

Content-type: application/json
Content-length: 333

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="4dc6e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4dc6e-140">Response</span></span>
<span data-ttu-id="4dc6e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4dc6e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 327

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```




