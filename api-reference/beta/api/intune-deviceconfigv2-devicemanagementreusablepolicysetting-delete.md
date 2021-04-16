---
title: Удаление deviceManagementReusablePolicySetting
description: Удаляет устройствоManagementReusablePolicySetting.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ca16a5e1f980ffdea6e797fd2868110bb6a68927
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51869158"
---
# <a name="delete-devicemanagementreusablepolicysetting"></a><span data-ttu-id="c8254-103">Удаление deviceManagementReusablePolicySetting</span><span class="sxs-lookup"><span data-stu-id="c8254-103">Delete deviceManagementReusablePolicySetting</span></span>

<span data-ttu-id="c8254-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8254-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8254-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8254-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8254-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c8254-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8254-107">Удаляет [устройствоManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md).</span><span class="sxs-lookup"><span data-stu-id="c8254-107">Deletes a [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8254-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c8254-108">Prerequisites</span></span>
<span data-ttu-id="c8254-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8254-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8254-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8254-111">Permission type</span></span>|<span data-ttu-id="c8254-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8254-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8254-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8254-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c8254-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8254-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c8254-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8254-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8254-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8254-116">Not supported.</span></span>|
|<span data-ttu-id="c8254-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="c8254-117">Application</span></span>|<span data-ttu-id="c8254-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8254-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8254-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8254-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/reusablePolicySettings/{deviceManagementReusablePolicySettingId}
```

## <a name="request-headers"></a><span data-ttu-id="c8254-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c8254-120">Request headers</span></span>
|<span data-ttu-id="c8254-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c8254-121">Header</span></span>|<span data-ttu-id="c8254-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c8254-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8254-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8254-123">Authorization</span></span>|<span data-ttu-id="c8254-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8254-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8254-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c8254-125">Accept</span></span>|<span data-ttu-id="c8254-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8254-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8254-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8254-127">Request body</span></span>
<span data-ttu-id="c8254-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c8254-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8254-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8254-129">Response</span></span>
<span data-ttu-id="c8254-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c8254-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c8254-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c8254-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8254-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8254-132">Request</span></span>
<span data-ttu-id="c8254-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8254-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/reusablePolicySettings/{deviceManagementReusablePolicySettingId}
```

### <a name="response"></a><span data-ttu-id="c8254-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8254-134">Response</span></span>
<span data-ttu-id="c8254-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c8254-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




