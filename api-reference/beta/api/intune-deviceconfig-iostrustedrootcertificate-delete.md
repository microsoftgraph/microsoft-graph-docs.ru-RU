---
title: Удаление Иострустедрутцертификате
description: Удаляет объект Иострустедрутцертификате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9dbdb076fb8817e8916b47b23f92b3b343879470
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31779029"
---
# <a name="delete-iostrustedrootcertificate"></a><span data-ttu-id="2e0ac-103">Удаление Иострустедрутцертификате</span><span class="sxs-lookup"><span data-stu-id="2e0ac-103">Delete iosTrustedRootCertificate</span></span>

> <span data-ttu-id="2e0ac-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e0ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e0ac-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e0ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e0ac-106">Удаляет объект [иострустедрутцертификате](../resources/intune-deviceconfig-iostrustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="2e0ac-106">Deletes a [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e0ac-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2e0ac-107">Prerequisites</span></span>
<span data-ttu-id="2e0ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e0ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e0ac-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e0ac-110">Permission type</span></span>|<span data-ttu-id="2e0ac-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e0ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e0ac-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e0ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2e0ac-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e0ac-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2e0ac-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e0ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e0ac-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e0ac-115">Not supported.</span></span>|
|<span data-ttu-id="2e0ac-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e0ac-116">Application</span></span>|<span data-ttu-id="2e0ac-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e0ac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e0ac-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e0ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/rootCertificatesForServerValidation/{iosTrustedRootCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="2e0ac-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e0ac-119">Request headers</span></span>
|<span data-ttu-id="2e0ac-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2e0ac-120">Header</span></span>|<span data-ttu-id="2e0ac-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2e0ac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e0ac-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e0ac-122">Authorization</span></span>|<span data-ttu-id="2e0ac-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e0ac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e0ac-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2e0ac-124">Accept</span></span>|<span data-ttu-id="2e0ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2e0ac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e0ac-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e0ac-126">Request body</span></span>
<span data-ttu-id="2e0ac-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e0ac-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e0ac-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="2e0ac-128">Response</span></span>
<span data-ttu-id="2e0ac-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2e0ac-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2e0ac-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2e0ac-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e0ac-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e0ac-131">Request</span></span>
<span data-ttu-id="2e0ac-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e0ac-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate
```

### <a name="response"></a><span data-ttu-id="2e0ac-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e0ac-133">Response</span></span>
<span data-ttu-id="2e0ac-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2e0ac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





