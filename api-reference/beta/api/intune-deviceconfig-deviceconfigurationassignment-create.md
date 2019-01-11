---
title: Создание объекта deviceConfigurationAssignment
description: Создание объекта deviceConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 076e8134892ac699670734255798f2297752acae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836794"
---
# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="2cbd2-103">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2cbd2-103">Create deviceConfigurationAssignment</span></span>

> <span data-ttu-id="2cbd2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2cbd2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2cbd2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cbd2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2cbd2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2cbd2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2cbd2-107">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2cbd2-107">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2cbd2-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2cbd2-108">Prerequisites</span></span>
<span data-ttu-id="2cbd2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cbd2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cbd2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2cbd2-111">Permission type</span></span>|<span data-ttu-id="2cbd2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2cbd2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cbd2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2cbd2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2cbd2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cbd2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2cbd2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2cbd2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cbd2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cbd2-116">Not supported.</span></span>|
|<span data-ttu-id="2cbd2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2cbd2-117">Application</span></span>|<span data-ttu-id="2cbd2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cbd2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cbd2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2cbd2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="2cbd2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2cbd2-120">Request headers</span></span>
|<span data-ttu-id="2cbd2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2cbd2-121">Header</span></span>|<span data-ttu-id="2cbd2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2cbd2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2cbd2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2cbd2-123">Authorization</span></span>|<span data-ttu-id="2cbd2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2cbd2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2cbd2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2cbd2-125">Accept</span></span>|<span data-ttu-id="2cbd2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2cbd2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cbd2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2cbd2-127">Request body</span></span>
<span data-ttu-id="2cbd2-128">В тексте запроса добавьте представление объекта deviceConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2cbd2-128">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="2cbd2-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="2cbd2-129">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="2cbd2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2cbd2-130">Property</span></span>|<span data-ttu-id="2cbd2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2cbd2-131">Type</span></span>|<span data-ttu-id="2cbd2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2cbd2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cbd2-133">id</span><span class="sxs-lookup"><span data-stu-id="2cbd2-133">id</span></span>|<span data-ttu-id="2cbd2-134">String</span><span class="sxs-lookup"><span data-stu-id="2cbd2-134">String</span></span>|<span data-ttu-id="2cbd2-135">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="2cbd2-135">The key of the assignment.</span></span>|
|<span data-ttu-id="2cbd2-136">target</span><span class="sxs-lookup"><span data-stu-id="2cbd2-136">target</span></span>|[<span data-ttu-id="2cbd2-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2cbd2-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2cbd2-138">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="2cbd2-138">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="2cbd2-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cbd2-139">Response</span></span>
<span data-ttu-id="2cbd2-140">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2cbd2-140">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cbd2-141">Пример</span><span class="sxs-lookup"><span data-stu-id="2cbd2-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="2cbd2-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="2cbd2-142">Request</span></span>
<span data-ttu-id="2cbd2-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2cbd2-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
Content-type: application/json
Content-length: 169

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="2cbd2-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="2cbd2-144">Response</span></span>
<span data-ttu-id="2cbd2-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2cbd2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 218

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





