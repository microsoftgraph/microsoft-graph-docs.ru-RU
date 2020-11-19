---
title: Удаление Девицеманажементинтежерсеттингинстанце
description: Удаляет объект Девицеманажементинтежерсеттингинстанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cec65bdc52aafa06f226c45fe748620f4ca7c69d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49291473"
---
# <a name="delete-devicemanagementintegersettinginstance"></a><span data-ttu-id="474b5-103">Удаление Девицеманажементинтежерсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="474b5-103">Delete deviceManagementIntegerSettingInstance</span></span>

<span data-ttu-id="474b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="474b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="474b5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="474b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="474b5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="474b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="474b5-107">Удаляет объект [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="474b5-107">Deletes a [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="474b5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="474b5-108">Prerequisites</span></span>
<span data-ttu-id="474b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="474b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="474b5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="474b5-111">Permission type</span></span>|<span data-ttu-id="474b5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="474b5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="474b5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="474b5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="474b5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="474b5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="474b5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="474b5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="474b5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="474b5-116">Not supported.</span></span>|
|<span data-ttu-id="474b5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="474b5-117">Application</span></span>|<span data-ttu-id="474b5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="474b5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="474b5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="474b5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
DELETE /deviceManagement/templates/{deviceManagementTemplateId}/settings/{deviceManagementSettingInstanceId}
DELETE /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings/{deviceManagementSettingInstanceId}
DELETE /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings/{deviceManagementSettingInstanceId}
```

## <a name="request-headers"></a><span data-ttu-id="474b5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="474b5-120">Request headers</span></span>
|<span data-ttu-id="474b5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="474b5-121">Header</span></span>|<span data-ttu-id="474b5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="474b5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="474b5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="474b5-123">Authorization</span></span>|<span data-ttu-id="474b5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="474b5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="474b5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="474b5-125">Accept</span></span>|<span data-ttu-id="474b5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="474b5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="474b5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="474b5-127">Request body</span></span>
<span data-ttu-id="474b5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="474b5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="474b5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="474b5-129">Response</span></span>
<span data-ttu-id="474b5-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="474b5-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="474b5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="474b5-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="474b5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="474b5-132">Request</span></span>
<span data-ttu-id="474b5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="474b5-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
```

### <a name="response"></a><span data-ttu-id="474b5-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="474b5-134">Response</span></span>
<span data-ttu-id="474b5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="474b5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




