---
title: Удаление Девицеманажементкомплекссеттингинстанце
description: Удаляет объект Девицеманажементкомплекссеттингинстанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e5abfa1473767379f0e7a4c7ef3eb7be34410b47
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313400"
---
# <a name="delete-devicemanagementcomplexsettinginstance"></a><span data-ttu-id="e49f3-103">Удаление Девицеманажементкомплекссеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="e49f3-103">Delete deviceManagementComplexSettingInstance</span></span>

> <span data-ttu-id="e49f3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e49f3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e49f3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e49f3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e49f3-106">Удаляет объект [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="e49f3-106">Deletes a [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e49f3-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e49f3-107">Prerequisites</span></span>
<span data-ttu-id="e49f3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e49f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e49f3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e49f3-110">Permission type</span></span>|<span data-ttu-id="e49f3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e49f3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e49f3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e49f3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e49f3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e49f3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e49f3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e49f3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e49f3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e49f3-115">Not supported.</span></span>|
|<span data-ttu-id="e49f3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e49f3-116">Application</span></span>|<span data-ttu-id="e49f3-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e49f3-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e49f3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e49f3-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="e49f3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e49f3-119">Request headers</span></span>
|<span data-ttu-id="e49f3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e49f3-120">Header</span></span>|<span data-ttu-id="e49f3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e49f3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e49f3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e49f3-122">Authorization</span></span>|<span data-ttu-id="e49f3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e49f3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e49f3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e49f3-124">Accept</span></span>|<span data-ttu-id="e49f3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e49f3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e49f3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e49f3-126">Request body</span></span>
<span data-ttu-id="e49f3-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e49f3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e49f3-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e49f3-128">Response</span></span>
<span data-ttu-id="e49f3-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e49f3-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e49f3-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e49f3-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e49f3-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e49f3-131">Request</span></span>
<span data-ttu-id="e49f3-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e49f3-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
```

### <a name="response"></a><span data-ttu-id="e49f3-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e49f3-133">Response</span></span>
<span data-ttu-id="e49f3-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e49f3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






