---
title: Удаление Граупполиципресентатионвалуебулеан
description: Удаляет объект Граупполиципресентатионвалуебулеан.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 08f911e41886bdb51b7e4c36c6b14c5819868b49
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804004"
---
# <a name="delete-grouppolicypresentationvalueboolean"></a><span data-ttu-id="97528-103">Удаление Граупполиципресентатионвалуебулеан</span><span class="sxs-lookup"><span data-stu-id="97528-103">Delete groupPolicyPresentationValueBoolean</span></span>

> <span data-ttu-id="97528-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97528-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97528-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="97528-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97528-106">Удаляет объект [граупполиципресентатионвалуебулеан](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md).</span><span class="sxs-lookup"><span data-stu-id="97528-106">Deletes a [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97528-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="97528-107">Prerequisites</span></span>
<span data-ttu-id="97528-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97528-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97528-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97528-110">Permission type</span></span>|<span data-ttu-id="97528-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="97528-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97528-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97528-112">Delegated (work or school account)</span></span>|<span data-ttu-id="97528-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97528-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="97528-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97528-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97528-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97528-115">Not supported.</span></span>|
|<span data-ttu-id="97528-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="97528-116">Application</span></span>|<span data-ttu-id="97528-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97528-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="97528-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97528-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="97528-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="97528-119">Request headers</span></span>
|<span data-ttu-id="97528-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="97528-120">Header</span></span>|<span data-ttu-id="97528-121">Значение</span><span class="sxs-lookup"><span data-stu-id="97528-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97528-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="97528-122">Authorization</span></span>|<span data-ttu-id="97528-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97528-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97528-124">Accept</span><span class="sxs-lookup"><span data-stu-id="97528-124">Accept</span></span>|<span data-ttu-id="97528-125">application/json</span><span class="sxs-lookup"><span data-stu-id="97528-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97528-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="97528-126">Request body</span></span>
<span data-ttu-id="97528-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="97528-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97528-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="97528-128">Response</span></span>
<span data-ttu-id="97528-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="97528-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="97528-130">Пример</span><span class="sxs-lookup"><span data-stu-id="97528-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="97528-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="97528-131">Request</span></span>
<span data-ttu-id="97528-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97528-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

### <a name="response"></a><span data-ttu-id="97528-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="97528-133">Response</span></span>
<span data-ttu-id="97528-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="97528-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




