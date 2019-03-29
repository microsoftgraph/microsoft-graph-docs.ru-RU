---
title: Удаление Граупполициконфигуратионассигнмент
description: Удаляет объект Граупполициконфигуратионассигнмент.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 56088b51ca36726eaafb10080aa316c7b26e70c9
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962969"
---
# <a name="delete-grouppolicyconfigurationassignment"></a><span data-ttu-id="04657-103">Удаление Граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="04657-103">Delete groupPolicyConfigurationAssignment</span></span>

> <span data-ttu-id="04657-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04657-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04657-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04657-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04657-106">Удаляет объект [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="04657-106">Deletes a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04657-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="04657-107">Prerequisites</span></span>
<span data-ttu-id="04657-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04657-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04657-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04657-110">Permission type</span></span>|<span data-ttu-id="04657-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="04657-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04657-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04657-112">Delegated (work or school account)</span></span>|<span data-ttu-id="04657-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04657-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="04657-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04657-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04657-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04657-115">Not supported.</span></span>|
|<span data-ttu-id="04657-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04657-116">Application</span></span>|<span data-ttu-id="04657-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04657-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04657-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04657-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="04657-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04657-119">Request headers</span></span>
|<span data-ttu-id="04657-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="04657-120">Header</span></span>|<span data-ttu-id="04657-121">Значение</span><span class="sxs-lookup"><span data-stu-id="04657-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04657-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04657-122">Authorization</span></span>|<span data-ttu-id="04657-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04657-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04657-124">Accept</span><span class="sxs-lookup"><span data-stu-id="04657-124">Accept</span></span>|<span data-ttu-id="04657-125">application/json</span><span class="sxs-lookup"><span data-stu-id="04657-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04657-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04657-126">Request body</span></span>
<span data-ttu-id="04657-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="04657-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04657-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="04657-128">Response</span></span>
<span data-ttu-id="04657-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="04657-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="04657-130">Пример</span><span class="sxs-lookup"><span data-stu-id="04657-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="04657-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="04657-131">Request</span></span>
<span data-ttu-id="04657-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04657-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="04657-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="04657-133">Response</span></span>
<span data-ttu-id="04657-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04657-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




