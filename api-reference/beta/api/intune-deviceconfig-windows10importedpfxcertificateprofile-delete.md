---
title: Удаление windows10ImportedPFXCertificateProfile
description: Удаляет объект windows10ImportedPFXCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 934a8d4de6691d44bbb456ab06cc71835971e1fc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49205344"
---
# <a name="delete-windows10importedpfxcertificateprofile"></a><span data-ttu-id="016ed-103">Удаление windows10ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="016ed-103">Delete windows10ImportedPFXCertificateProfile</span></span>

<span data-ttu-id="016ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="016ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="016ed-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="016ed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="016ed-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="016ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="016ed-107">Удаляет объект [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="016ed-107">Deletes a [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="016ed-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="016ed-108">Prerequisites</span></span>
<span data-ttu-id="016ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="016ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="016ed-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="016ed-111">Permission type</span></span>|<span data-ttu-id="016ed-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="016ed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="016ed-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="016ed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="016ed-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="016ed-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="016ed-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="016ed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="016ed-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="016ed-116">Not supported.</span></span>|
|<span data-ttu-id="016ed-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="016ed-117">Application</span></span>|<span data-ttu-id="016ed-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="016ed-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="016ed-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="016ed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="016ed-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="016ed-120">Request headers</span></span>
|<span data-ttu-id="016ed-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="016ed-121">Header</span></span>|<span data-ttu-id="016ed-122">Значение</span><span class="sxs-lookup"><span data-stu-id="016ed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="016ed-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="016ed-123">Authorization</span></span>|<span data-ttu-id="016ed-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="016ed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="016ed-125">Accept</span><span class="sxs-lookup"><span data-stu-id="016ed-125">Accept</span></span>|<span data-ttu-id="016ed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="016ed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="016ed-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="016ed-127">Request body</span></span>
<span data-ttu-id="016ed-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="016ed-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="016ed-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="016ed-129">Response</span></span>
<span data-ttu-id="016ed-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="016ed-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="016ed-131">Пример</span><span class="sxs-lookup"><span data-stu-id="016ed-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="016ed-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="016ed-132">Request</span></span>
<span data-ttu-id="016ed-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="016ed-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="016ed-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="016ed-134">Response</span></span>
<span data-ttu-id="016ed-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="016ed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




