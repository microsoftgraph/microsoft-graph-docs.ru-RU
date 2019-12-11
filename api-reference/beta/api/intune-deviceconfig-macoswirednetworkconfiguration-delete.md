---
title: Удаление Макосвиреднетворкконфигуратион
description: Удаляет объект Макосвиреднетворкконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5f7c4ac01ef478a7536e2e0adb1717f42c1bcfdd
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948025"
---
# <a name="delete-macoswirednetworkconfiguration"></a><span data-ttu-id="68385-103">Удаление Макосвиреднетворкконфигуратион</span><span class="sxs-lookup"><span data-stu-id="68385-103">Delete macOSWiredNetworkConfiguration</span></span>

> <span data-ttu-id="68385-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68385-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68385-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="68385-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68385-106">Удаляет объект [макосвиреднетворкконфигуратион](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="68385-106">Deletes a [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68385-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="68385-107">Prerequisites</span></span>
<span data-ttu-id="68385-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68385-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68385-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68385-110">Permission type</span></span>|<span data-ttu-id="68385-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="68385-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68385-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68385-112">Delegated (work or school account)</span></span>|<span data-ttu-id="68385-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68385-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="68385-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68385-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68385-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68385-115">Not supported.</span></span>|
|<span data-ttu-id="68385-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68385-116">Application</span></span>|<span data-ttu-id="68385-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68385-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="68385-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68385-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="68385-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="68385-119">Request headers</span></span>
|<span data-ttu-id="68385-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68385-120">Header</span></span>|<span data-ttu-id="68385-121">Значение</span><span class="sxs-lookup"><span data-stu-id="68385-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68385-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68385-122">Authorization</span></span>|<span data-ttu-id="68385-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68385-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68385-124">Accept</span><span class="sxs-lookup"><span data-stu-id="68385-124">Accept</span></span>|<span data-ttu-id="68385-125">application/json</span><span class="sxs-lookup"><span data-stu-id="68385-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68385-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="68385-126">Request body</span></span>
<span data-ttu-id="68385-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="68385-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68385-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="68385-128">Response</span></span>
<span data-ttu-id="68385-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="68385-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="68385-130">Пример</span><span class="sxs-lookup"><span data-stu-id="68385-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="68385-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="68385-131">Request</span></span>
<span data-ttu-id="68385-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68385-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="68385-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="68385-133">Response</span></span>
<span data-ttu-id="68385-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68385-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





