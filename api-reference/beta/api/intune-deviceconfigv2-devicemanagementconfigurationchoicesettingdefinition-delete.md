---
title: Удаление deviceManagementConfigurationChoiceSettingDefinition
description: Удаляет устройствоManagementConfigurationChoiceSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ebbed94f10e1a519f6f3480cca8da2654cf1a0d0
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864447"
---
# <a name="delete-devicemanagementconfigurationchoicesettingdefinition"></a><span data-ttu-id="f86ef-103">Удаление deviceManagementConfigurationChoiceSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="f86ef-103">Delete deviceManagementConfigurationChoiceSettingDefinition</span></span>

<span data-ttu-id="f86ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f86ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f86ef-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f86ef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f86ef-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f86ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f86ef-107">Удаляет [устройствоManagementConfigurationChoiceSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f86ef-107">Deletes a [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f86ef-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f86ef-108">Prerequisites</span></span>
<span data-ttu-id="f86ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f86ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f86ef-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f86ef-111">Permission type</span></span>|<span data-ttu-id="f86ef-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f86ef-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f86ef-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f86ef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f86ef-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f86ef-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f86ef-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f86ef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f86ef-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f86ef-116">Not supported.</span></span>|
|<span data-ttu-id="f86ef-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="f86ef-117">Application</span></span>|<span data-ttu-id="f86ef-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f86ef-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f86ef-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f86ef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/reusableSettings/{deviceManagementConfigurationSettingDefinitionId}
DELETE /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
DELETE /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="f86ef-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f86ef-120">Request headers</span></span>
|<span data-ttu-id="f86ef-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f86ef-121">Header</span></span>|<span data-ttu-id="f86ef-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f86ef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f86ef-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f86ef-123">Authorization</span></span>|<span data-ttu-id="f86ef-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f86ef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f86ef-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f86ef-125">Accept</span></span>|<span data-ttu-id="f86ef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f86ef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f86ef-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f86ef-127">Request body</span></span>
<span data-ttu-id="f86ef-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f86ef-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f86ef-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f86ef-129">Response</span></span>
<span data-ttu-id="f86ef-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f86ef-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f86ef-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f86ef-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f86ef-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f86ef-132">Request</span></span>
<span data-ttu-id="f86ef-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f86ef-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/reusableSettings/{deviceManagementConfigurationSettingDefinitionId}
```

### <a name="response"></a><span data-ttu-id="f86ef-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f86ef-134">Response</span></span>
<span data-ttu-id="f86ef-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f86ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




