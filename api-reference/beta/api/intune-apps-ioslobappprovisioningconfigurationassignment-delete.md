---
title: Удаление Иослобапппровисионингконфигуратионассигнмент
description: Удаляет объект Иослобапппровисионингконфигуратионассигнмент.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c390b5c2baa9fc395e6cd0dd8a1501add10ea1db
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153111"
---
# <a name="delete-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="07f28-103">Удаление Иослобапппровисионингконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="07f28-103">Delete iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="07f28-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07f28-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07f28-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="07f28-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07f28-106">Удаляет объект [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="07f28-106">Deletes a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07f28-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="07f28-107">Prerequisites</span></span>
<span data-ttu-id="07f28-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="07f28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="07f28-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07f28-110">Permission type</span></span>|<span data-ttu-id="07f28-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="07f28-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07f28-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07f28-112">Delegated (work or school account)</span></span>|<span data-ttu-id="07f28-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07f28-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="07f28-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07f28-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07f28-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07f28-115">Not supported.</span></span>|
|<span data-ttu-id="07f28-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07f28-116">Application</span></span>|<span data-ttu-id="07f28-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07f28-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07f28-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07f28-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="07f28-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07f28-119">Request headers</span></span>
|<span data-ttu-id="07f28-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="07f28-120">Header</span></span>|<span data-ttu-id="07f28-121">Значение</span><span class="sxs-lookup"><span data-stu-id="07f28-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07f28-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="07f28-122">Authorization</span></span>|<span data-ttu-id="07f28-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="07f28-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07f28-124">Accept</span><span class="sxs-lookup"><span data-stu-id="07f28-124">Accept</span></span>|<span data-ttu-id="07f28-125">application/json</span><span class="sxs-lookup"><span data-stu-id="07f28-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07f28-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07f28-126">Request body</span></span>
<span data-ttu-id="07f28-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="07f28-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07f28-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="07f28-128">Response</span></span>
<span data-ttu-id="07f28-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="07f28-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="07f28-130">Пример</span><span class="sxs-lookup"><span data-stu-id="07f28-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="07f28-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="07f28-131">Request</span></span>
<span data-ttu-id="07f28-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07f28-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="07f28-133">Отклик
</span><span class="sxs-lookup"><span data-stu-id="07f28-133">Response</span></span>
<span data-ttu-id="07f28-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="07f28-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




