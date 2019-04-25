---
title: Удаление Граупполициконфигуратионассигнмент
description: Удаляет объект Граупполициконфигуратионассигнмент.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f2e8cd451fb6d8c1775f709b92c29d321d9cd417
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532081"
---
# <a name="delete-grouppolicyconfigurationassignment"></a><span data-ttu-id="efafb-103">Удаление Граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="efafb-103">Delete groupPolicyConfigurationAssignment</span></span>

> <span data-ttu-id="efafb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efafb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efafb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="efafb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efafb-106">Удаляет объект [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="efafb-106">Deletes a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efafb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="efafb-107">Prerequisites</span></span>
<span data-ttu-id="efafb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efafb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efafb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="efafb-110">Permission type</span></span>|<span data-ttu-id="efafb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="efafb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efafb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="efafb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="efafb-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efafb-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="efafb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="efafb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efafb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efafb-115">Not supported.</span></span>|
|<span data-ttu-id="efafb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="efafb-116">Application</span></span>|<span data-ttu-id="efafb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efafb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="efafb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="efafb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="efafb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="efafb-119">Request headers</span></span>
|<span data-ttu-id="efafb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="efafb-120">Header</span></span>|<span data-ttu-id="efafb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="efafb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efafb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="efafb-122">Authorization</span></span>|<span data-ttu-id="efafb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="efafb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efafb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="efafb-124">Accept</span></span>|<span data-ttu-id="efafb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="efafb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efafb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="efafb-126">Request body</span></span>
<span data-ttu-id="efafb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="efafb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efafb-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="efafb-128">Response</span></span>
<span data-ttu-id="efafb-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="efafb-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="efafb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="efafb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="efafb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="efafb-131">Request</span></span>
<span data-ttu-id="efafb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="efafb-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="efafb-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="efafb-133">Response</span></span>
<span data-ttu-id="efafb-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="efafb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





